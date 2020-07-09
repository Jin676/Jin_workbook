### 用户评论
    *  第一版
    1. 状态在App中，给AddComment，给Listcomments和deleteComment，List再给item-deleteComment
    *  第二版
    1. 状态在List中，初始化状态在自身上解决，App给了Add一个方法commentObj，Add往里面传参数(参数就是传的数据),APP再将数据交给List，List通过componentWillReceiveProps接受到参数，然后再传给item
    