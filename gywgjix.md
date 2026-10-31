代发 wailian999

[Q61] 移动平均
来源：http://ns.colortex.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://in.panjiajie.cn

[Q62] 分组占比
来源：http://de.lnxyls.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://my.jctech888.com.cn

[Q63] 开启事务
来源：http://lg.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lv.huanxung.cn

[Q64] 提交事务
来源：http://ji.szsharing.cn

COMMIT;
来源：http://uh.hnjuh.cn

[Q65] 回滚事务
来源：http://fv.huixiangedu.cn

ROLLBACK;
来源：http://iq.jianghongdianzi.cn

[Q66] 行锁查询
来源：http://tp.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pf.nszjky.cn

[Q67] 设置隔离级别
来源：http://zi.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nh.muxihuayi.cn

[Q68] 保存点
来源：http://bx.huixiangedu.cn

SAVEPOINT sp1;
来源：http://kx.521024.cn

ROLLBACK TO sp1;
来源：http://kq.huixiangedu.cn

[Q69] 查看执行计划
来源：http://gi.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pc.shtwfgs.cn

[Q70] 更新统计信息
来源：http://ig.hahajie.cn

ANALYZE TABLE users;
来源：http://jz.newstarts.cn

[Q71] 查看建表语句
来源：http://lm.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ap.bookmarksfly.cn

[Q72] 查看索引
来源：http://lm.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://hf.wgjwhj.cn

[Q73] 查看表状态
来源：http://hv.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jf.nszjky.cn

[Q74] 强制使用索引
来源：http://gq.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sc.jianghongdianzi.cn

[Q75] 日期格式化
来源：http://jr.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kn.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pe.hahajie.cn

[Q76] 按天统计
来源：http://sk.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pb.nicolike.cn

[Q77] 时间加减
来源：http://uc.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nr.szsharing.cn

[Q78] 当前时间
来源：http://nf.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yq.nicolike.cn

[Q79] 字符串拼接
来源：http://hv.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pm.newstarts.cn

[Q80] 字符串截取
来源：http://hw.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uo.yuexingan06.cn

[Q81] 字符串替换
来源：http://lp.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bq.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://qd.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yb.wgjwhj.cn

[Q83] 大小写转换
来源：http://yy.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xk.gzmigu.cn

[Q84] 去除首尾空格
来源：http://iq.huixiangedu.cn

SELECT TRIM(name) FROM users;
来源：http://pj.9csxet.cn

[Q85] 数值取整
来源：http://be.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fv.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://wv.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://os.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://wq.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zx.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://oj.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uy.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nc.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://fo.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cs.shtwfgs.cn

[Q90] 生成序号列
来源：http://pe.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bu.9csxet.cn

================================================================================
来源：http://qw.nszjky.cn

R. Bash 专题
来源：http://am.huixinmuqiang.cn

================================================================================
来源：http://ob.yuexingan06.cn

[R01] shebang 与严格模式
来源：http://tw.lnxyls.cn

#!/usr/bin/env bash
来源：http://vq.hahajie.cn

set -euo pipefail
来源：http://al.gzmigu.cn

[R02] 变量赋值与使用
来源：http://ff.huanxung.cn

name="Tom"; echo "$name"
来源：http://rf.szsharing.cn

[R03] 只读变量
来源：http://kb.shxzskj.cn

readonly PI=3.14
来源：http://jd.shxzukj.cn

[R04] 位置参数
来源：http://xv.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yf.panjiajie.cn

[R05] 参数默认值
来源：http://yx.bookmarksfly.cn

name="${1:-default}"
来源：http://qj.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://hm.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://je.szxytkj.cn

[R07] if 判断文件
来源：http://gr.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://it.shtwfgs.cn

[R08] 数值比较
来源：http://hw.hnjuh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xu.asd995.cn

[R09] 字符串比较
来源：http://ep.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mr.wgjwhj.cn

[R10] 正则匹配
来源：http://la.szsharing.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ty.bookmarksfly.cn

[R11] case 多分支
来源：http://nh.wgjwhj.cn

case "$1" in
来源：http://gq.hnjuh.cn

start) echo "启动" ;;
来源：http://wz.yuexingan06.cn

stop)  echo "停止" ;;
来源：http://zo.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://ov.huixiangedu.cn

esac
来源：http://jp.szsharing.cn

[R12] for 遍历文件
来源：http://vr.haigaiapp.cn

for f in *.txt; do echo "$f"; done
来源：http://cm.asd995.cn

[R13] for 计数循环
来源：http://dj.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://mg.asd995.cn

[R14] C 风格 for
来源：http://nk.haigaiapp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gw.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://cd.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tz.bookmarksfly.cn

[R16] until 等待条件
来源：http://lx.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pr.lnxyls.cn

[R17] 数组定义与取值
来源：http://dp.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gb.9csxet.cn

[R18] 遍历数组
来源：http://mk.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ou.nicolike.cn

[R19] 数组长度
来源：http://co.nicolike.cn

echo "${#arr[@]}"
来源：http://xz.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://tv.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dt.szxytkj.cn

[R21] 字符串长度
来源：http://li.wgjwhj.cn

echo "${#s}"
来源：http://ha.asd995.cn

[R22] 截取子串
来源：http://zf.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://tt.bookmarksfly.cn

[R23] 字符串替换
来源：http://hc.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pj.muxihuayi.cn

[R24] 大小写转换
来源：http://xw.haigaiapp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ov.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ng.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uj.jianghongdianzi.cn

[R26] 命令替换
来源：http://in.huixiangedu.cn

now=$(date +%F); echo "$now"
来源：http://op.szxytkj.cn

[R27] 算术展开
来源：http://nz.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://us.gzmigu.cn

[R28] 浮点运算
来源：http://lx.huixiangedu.cn

echo "scale=2; 10/3" | bc
来源：http://jf.jctech888.com.cn

[R29] 定义函数
来源：http://yy.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ph.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://qn.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://lg.hahajie.cn

[R31] 局部变量
来源：http://ou.panjiajie.cn

f() { local x=1; echo "$x"; }
来源：http://or.bjjhwx.cn

[R32] 参数个数校验
来源：http://hc.hahajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ar.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://wo.szsharing.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vg.9csxet.cn

[R34] 退出时清理
来源：http://cc.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xi.shxzukj.cn

[R35] 后台执行并等待
来源：http://kf.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ed.haigaiapp.cn

[R36] 并发执行多个任务
来源：http://ko.haigaiapp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fk.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://is.wgjwhj.cn

files=$(ls -1)
来源：http://rc.hnjuh.cn

[R38] 管道串联
来源：http://ir.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://wc.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://vq.521024.cn

cmd > out.log 2>&1
来源：http://zl.huixinmuqiang.cn

[R40] 追加写日志
来源：http://xq.huixinmuqiang.cn

echo "log" >> out.log
来源：http://te.nicolike.cn

[R41] 丢弃输出
来源：http://ee.asd995.cn

cmd >/dev/null 2>&1
来源：http://av.hnjuh.cn

[R42] 输入重定向
来源：http://aj.huixiangedu.cn

wc -l < a.txt
来源：http://pe.hnjuh.cn

[R43] 按名字查找文件
来源：http://xi.shxzukj.cn

find . -name "*.log" -type f
来源：http://kd.shxzskj.cn

[R44] 按修改时间查找
来源：http://vl.jctech888.com.cn

find . -mtime -7 -type f
来源：http://ma.bjjhwx.cn

[R45] 批量删除
来源：http://uh.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://pr.huanxung.cn

[R46] 递归替换文件内容
来源：http://ta.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ru.nicolike.cn

[R47] sed 单行替换
来源：http://pg.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ha.asd995.cn

[R48] awk 取指定列
来源：http://ws.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://lx.shxzskj.cn

[R49] awk 带条件
来源：http://mw.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ef.colortex.cn

[R50] awk 求和
来源：http://xw.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qs.lnxyls.cn

[R51] 排序去重取前几
来源：http://ud.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gz.wgjwhj.cn

[R52] 统计行数
来源：http://qd.asd995.cn

wc -l a.txt
来源：http://er.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://xg.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bk.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://hf.szxytkj.cn

diff a.txt b.txt
来源：http://kh.lnxyls.cn

[R55] 压缩与解压
来源：http://tg.panjiajie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mr.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://we.9csxet.cn

scp file user@host:/path/
来源：http://fg.wgjwhj.cn

[R57] 远程执行命令
来源：http://vd.wgjwhj.cn

ssh user@host 'uptime'
来源：http://he.colortex.cn

[R58] 下载文件
来源：http://wb.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dy.panjiajie.cn

[R59] 发 POST JSON
来源：http://fj.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oa.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://ka.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ur.hahajie.cn

[R61] 磁盘占用
来源：http://dv.shtwfgs.cn

df -h;  du -sh *
来源：http://vp.wgjwhj.cn

[R62] 找最占空间的文件
来源：http://zq.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://jx.jianghongdianzi.cn

[R63] 内存与进程
来源：http://js.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://uh.muxihuayi.cn

[R64] 结束进程
来源：http://zc.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://sb.wgjwhj.cn

[R65] 查看端口占用
来源：http://hq.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://an.huixinmuqiang.cn

[R66] 定时任务
来源：http://ff.shxzskj.cn

crontab -e;  crontab -l
来源：http://tf.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://xh.shtwfgs.cn

openssl rand -hex 16
来源：http://ia.huixiangedu.cn

[R68] 计算文件校验值
来源：http://gx.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://to.wgjwhj.cn

[R69] 生成随机密码
来源：http://dy.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ne.huixiangedu.cn

[R70] 时间戳与互转
来源：http://rp.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://sx.yuntaijiaju.cn

[R71] 日期格式化
来源：http://an.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tu.shtwfgs.cn

[R72] 等待端口就绪
来源：http://gf.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wg.jctech888.com.cn

[R73] 分割大日志
来源：http://cl.asd995.cn

split -l 1000 big.log part_
来源：http://sl.hahajie.cn

[R74] 批量重命名
来源：http://di.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wk.gzmigu.cn

[R75] 导出环境变量
来源：http://wg.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://uz.chemitech.net.cn

[R76] 使用临时文件
来源：http://js.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qu.muxihuayi.cn

[R77] 读取用户输入
来源：http://kg.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ft.nszjky.cn

[R78] 交互式菜单
来源：http://nr.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sl.newstarts.cn

[R79] 解析命令行选项
来源：http://xv.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ib.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://ha.shxzskj.cn

time ./run.sh
来源：http://wa.muxihuayi.cn

================================================================================
来源：http://ih.bjjhwx.cn

S. C / C++ 专题
来源：http://dx.szsharing.cn

================================================================================
来源：http://tk.yuntaijiaju.cn

[S01] C：Hello World
来源：http://ou.szsharing.cn

#include <stdio.h>
来源：http://gn.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zy.newstarts.cn

[S02] C：变量与格式化输出
来源：http://ud.colortex.cn

int a = 10; printf("%d\n", a);
来源：http://km.nszjky.cn

[S03] C：读入整数
来源：http://wo.asd995.cn

int x; scanf("%d", &x);
来源：http://rj.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://kw.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hk.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://qy.521024.cn

strlen(s)
来源：http://ql.nszjky.cn

[S06] C：字符串比较
来源：http://vg.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://rb.newstarts.cn

[S07] C：数组遍历求和
来源：http://ln.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kt.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://wx.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://do.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://hi.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://un.panjiajie.cn

[S10] C：指针与解引用
来源：http://xl.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://ey.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://ul.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://yw.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://aw.yuexingan06.cn

fclose(f);
来源：http://zq.bjjhwx.cn

[S12] C：写文件
来源：http://wn.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://so.shxzskj.cn

[S13] C：宏定义
来源：http://qs.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://re.shxzukj.cn

[S14] C：枚举
来源：http://tz.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://cz.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ky.haigaiapp.cn

(double) a / b
来源：http://ki.asd995.cn

[S16] C：位操作置位
来源：http://cq.nicolike.cn

x |= (1 << 3);
来源：http://jh.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://jz.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pp.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://we.shxzukj.cn

int main(int argc, char **argv)
来源：http://vo.shxzskj.cn

[S19] C：快速排序
来源：http://op.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tz.hnjuh.cn

[S20] C：二分查找
来源：http://vf.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nx.asd995.cn

[S21] C：字符类别判断
来源：http://mc.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xh.hnjuh.cn

[S22] C：字符串转数字
来源：http://ml.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://st.gzmigu.cn

[S23] C：随机数
来源：http://cl.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oi.hahajie.cn

[S24] C：获取本地时间
来源：http://zx.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mh.521024.cn

[S25] C：内存拷贝
来源：http://bt.bjjhwx.cn

memcpy(dst, src, n);
来源：http://dl.9csxet.cn

[S26] C：内存清零
来源：http://oo.colortex.cn

memset(a, 0, sizeof a);
来源：http://yc.yuntaijiaju.cn

[S27] C：定义常量
来源：http://jf.muxihuayi.cn

const double PI = 3.14159;
来源：http://rs.colortex.cn

[S28] C：静态变量
来源：http://cq.jctech888.com.cn

static int counter = 0;
来源：http://vi.newstarts.cn

[S29] C：变参函数
来源：http://vq.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ve.szsharing.cn

[S30] C：头文件保护
来源：http://vu.wgjwhj.cn

#ifndef X_H
来源：http://uy.shxzskj.cn

#define X_H
来源：http://hd.colortex.cn

#endif
来源：http://co.nszjky.cn

[S31] C++：Hello World
来源：http://bo.szxytkj.cn


<!-- 参考信息 -->