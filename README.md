java从数据库读取菜单，递归生成菜单树
https://blog.csdn.net/frankcheng5143/article/details/52958486
primeng-tree-demo

echo "# Note" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/shangshanruoshui77/Note.git
git push -u origin master

git remote add origin https://github.com/shangshanruoshui77/Note.git
git push -u origin master

<div class="container login-screen">
    <div class="row">
        <div class="col-sm-6 col-sm-offset-3">
            <div class="login-form-container">
                <h3 class="center-block sys-title">NiceFish-Admin</h3>
                <form #form="ngForm" (ngSubmit)="form.form.valid" novalidate class="form-horizontal" role="form">
                    <div class="form-group" [ngClass]="{ 'has-error': form.submitted && !userName.valid }">
                        <label class="col-sm-2 control-label">用户名：</label>
                        <div class="col-sm-10">
                            <input required name="userName" [(ngModel)]="user.userName" #userName="ngModel" type="text" class="form-control" placeholder="请输入用户名...">
                            <div *ngIf="form.submitted && !userName.valid" class="text-danger">用户名必须输入！</div>
                        </div>
                    </div>
                    <div class="form-group" [ngClass]="{ 'has-error': form.submitted && !password.valid }">
                        <label class="col-sm-2 control-label">密码：</label>
                        <div class="col-sm-10">
                            <input required minlength="8" [(ngModel)]="user.password" name="password" #password="ngModel" type="password" class="form-control"
                                placeholder="请输入密码...">
                            <div *ngIf="form.submitted && !password.valid" class="text-danger">密码必须输入,至少要8位！</div>
                        </div>
                    </div>
                    <div class="form-group">
                        <div class="col-sm-offset-2 col-sm-10">
                            <div class="checkbox">
                                <label>
                                <input name="remeberMe" type="checkbox" [(ngModel)]="user.remeberMe" #remeberMe="ngModel">记住我
                            </label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <div class="col-sm-offset-2 col-sm-10">
                            <button type="submit" class="btn btn-success" (click)="login()">登录</button>
                            <button type="button" class="btn btn-danger" (click)="forgetPwd()">忘记密码？</button>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </div>
</div>
