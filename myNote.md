caller, callee��arguments�ֱ���ʲô
�ο���: caller,callee֮��Ĺ�ϵ������employer��employee֮��Ĺ�ϵ�����ǵ����뱻���õĹ�ϵ�����߷��صĶ��Ǻ����������ã�arguments�Ǻ��������в����б�������һ��������ı�����

������ʾ

    function parent(param1, param2, param3) {
        child(param1, param2, param3);
    }

    function child() {
        console.log(arguments); // { '0': 'mqin1', '1': 'mqin2', '2': 'mqin3' }
        console.log(arguments.callee); // [Function: child]
        console.log(child.caller); // [Function: parent]
    }

    parent('mqin1', 'mqin2', 'mqin3');