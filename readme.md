### http://www.icelery.fun
public enum StatusEnum {
    LOGIN_USER_NAME_IS_WRONG(4001,"用户名不存在!"),
    LOGIN_USER_PHONE_IS_WRONG(4009,"手机号不存在!"),
    LOGIN_USER_PWD_IS_WRONG(4002,"密码错误!"),
    LOGIN_SUCCESS(200,"通过!"),
    GET_DATA_SUCCESS(200,"获取数据成功!"),
    SENDMSG_SUCCESS(200,"获取数据成功!"),
    DATA_IS_WRONG(4003,"数据不合法!"),
    DELETE_SUCCESS(200,"删除成功!"),
    DELETE_FAILED(4004,"删除失败!"),
    NO_DATA(4005,"没有对应的数据!"),
    ADD_DATA_SUCCESS(200,"添加数据成功!"),
    EDIT_SUCCESS(200,"编辑成功!"),
    NO_ACCESS(4007,"没有权限!"),
    SENDMSG_FAIL(4008,"发送验证码失败!"),
    VCODE_WRONG(4010,"验证码错误!"),
    ;


    /**
     * 状态码
     */
    private Integer code;

    /**
     * 提示信息
     */
    private String msg;

    /**
     * 构造器
     * @param code
     * @param msg
     */
    StatusEnum(Integer code, String msg) {
        this.code = code;
        this.msg = msg;
    }

    public Integer getCode() {
        return code;
    }

    public void setCode(Integer code) {
        this.code = code;
    }

    public String getMsg() {
        return msg;
    }

    public void setMsg(String msg) {
        this.msg = msg;
    }
}
