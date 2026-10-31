代发 wailian999

[Q63] 开启事务
来源：http://ku.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://os.bjjhwx.cn

[Q64] 提交事务
来源：http://kv.9csxet.cn

COMMIT;
来源：http://lc.yuexingan06.cn

[Q65] 回滚事务
来源：http://ss.nszjky.cn

ROLLBACK;
来源：http://dr.9csxet.cn

[Q66] 行锁查询
来源：http://cd.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rp.newstarts.cn

[Q67] 设置隔离级别
来源：http://yj.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dz.huixinmuqiang.cn

[Q68] 保存点
来源：http://qh.yuexingan06.cn

SAVEPOINT sp1;
来源：http://ds.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://bx.colortex.cn

[Q69] 查看执行计划
来源：http://uk.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ab.gzmigu.cn

[Q70] 更新统计信息
来源：http://ad.muxihuayi.cn

ANALYZE TABLE users;
来源：http://sb.lnxyls.cn

[Q71] 查看建表语句
来源：http://tj.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rt.hnjuh.cn

[Q72] 查看索引
来源：http://zk.nicolike.cn

SHOW INDEX FROM users;
来源：http://nx.bookmarksfly.cn

[Q73] 查看表状态
来源：http://af.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ue.yuexingan06.cn

[Q74] 强制使用索引
来源：http://zc.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nf.panjiajie.cn

[Q75] 日期格式化
来源：http://qf.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ie.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fg.huixiangedu.cn

[Q76] 按天统计
来源：http://eq.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ce.nszjky.cn

[Q77] 时间加减
来源：http://oa.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fu.nicolike.cn

[Q78] 当前时间
来源：http://qy.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bb.wgjwhj.cn

[Q79] 字符串拼接
来源：http://af.jianghongdianzi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tg.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://eg.shxzukj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ap.colortex.cn

[Q81] 字符串替换
来源：http://ub.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kd.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://ic.gzmigu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://or.muxihuayi.cn

[Q83] 大小写转换
来源：http://cu.bjjhwx.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xl.panjiajie.cn

[Q84] 去除首尾空格
来源：http://rw.yuexingan06.cn

SELECT TRIM(name) FROM users;
来源：http://vs.chemitech.net.cn

[Q85] 数值取整
来源：http://kg.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nf.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://je.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zk.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://gv.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hq.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://qf.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://op.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jk.bjjhwx.cn

[Q89] 判断表是否存在
来源：http://cw.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wb.lnxyls.cn

[Q90] 生成序号列
来源：http://et.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gj.muxihuayi.cn

================================================================================
来源：http://sl.521024.cn

R. Bash 专题
来源：http://oi.lnxyls.cn

================================================================================
来源：http://zk.nicolike.cn

[R01] shebang 与严格模式
来源：http://qo.panjiajie.cn

#!/usr/bin/env bash
来源：http://lu.hahajie.cn

set -euo pipefail
来源：http://er.9csxet.cn

[R02] 变量赋值与使用
来源：http://hw.bookmarksfly.cn

name="Tom"; echo "$name"
来源：http://sq.szxytkj.cn

[R03] 只读变量
来源：http://qf.szxytkj.cn

readonly PI=3.14
来源：http://xj.hahajie.cn

[R04] 位置参数
来源：http://jx.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://db.bookmarksfly.cn

[R05] 参数默认值
来源：http://wp.huixinmuqiang.cn

name="${1:-default}"
来源：http://nn.nszjky.cn

[R06] 判断命令是否存在
来源：http://vh.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dp.nszjky.cn

[R07] if 判断文件
来源：http://uz.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uq.asd995.cn

[R08] 数值比较
来源：http://vc.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vv.szxytkj.cn

[R09] 字符串比较
来源：http://vn.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mb.lnxyls.cn

[R10] 正则匹配
来源：http://fy.huanxung.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mv.huanxung.cn

[R11] case 多分支
来源：http://kj.9csxet.cn

case "$1" in
来源：http://km.chemitech.net.cn

start) echo "启动" ;;
来源：http://of.hahajie.cn

stop)  echo "停止" ;;
来源：http://os.nicolike.cn

*)     echo "未知命令" ;;
来源：http://ps.newstarts.cn

esac
来源：http://bn.hahajie.cn

[R12] for 遍历文件
来源：http://dz.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://zi.yuntaijiaju.cn

[R13] for 计数循环
来源：http://er.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://bm.jctech888.com.cn

[R14] C 风格 for
来源：http://si.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cy.shxzskj.cn

[R15] while 逐行读文件
来源：http://gy.yuntaijiaju.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://or.hahajie.cn

[R16] until 等待条件
来源：http://et.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ht.colortex.cn

[R17] 数组定义与取值
来源：http://ew.jctech888.com.cn

arr=(a b c); echo "${arr[0]}"
来源：http://am.nszjky.cn

[R18] 遍历数组
来源：http://cp.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sm.bjjhwx.cn

[R19] 数组长度
来源：http://ms.gzmigu.cn

echo "${#arr[@]}"
来源：http://wr.huanxung.cn

[R20] 关联数组（字典）
来源：http://yu.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mg.haigaiapp.cn

[R21] 字符串长度
来源：http://ti.bookmarksfly.cn

echo "${#s}"
来源：http://os.lnxyls.cn

[R22] 截取子串
来源：http://wv.gzmigu.cn

echo "${s:0:5}"
来源：http://og.9csxet.cn

[R23] 字符串替换
来源：http://bn.huanxung.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ys.szsharing.cn

[R24] 大小写转换
来源：http://ps.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yq.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://vk.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gf.huixinmuqiang.cn

[R26] 命令替换
来源：http://xp.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ui.nszjky.cn

[R27] 算术展开
来源：http://wo.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://or.asd995.cn

[R28] 浮点运算
来源：http://hr.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://oe.newstarts.cn

[R29] 定义函数
来源：http://kz.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nz.chemitech.net.cn

[R30] 函数返回状态码
来源：http://ad.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lr.nszjky.cn

[R31] 局部变量
来源：http://uz.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://cp.jianghongdianzi.cn

[R32] 参数个数校验
来源：http://qt.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iw.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://qz.lnxyls.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://id.huanxung.cn

[R34] 退出时清理
来源：http://ps.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zq.nicolike.cn

[R35] 后台执行并等待
来源：http://fj.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fv.newstarts.cn

[R36] 并发执行多个任务
来源：http://qo.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xb.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://qp.nszjky.cn

files=$(ls -1)
来源：http://bl.shxzukj.cn

[R38] 管道串联
来源：http://fe.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://yb.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://yr.haigaiapp.cn

cmd > out.log 2>&1
来源：http://zo.wgjwhj.cn

[R40] 追加写日志
来源：http://qj.huixiangedu.cn

echo "log" >> out.log
来源：http://nj.521024.cn

[R41] 丢弃输出
来源：http://eh.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://qs.hnjuh.cn

[R42] 输入重定向
来源：http://sa.yuntaijiaju.cn

wc -l < a.txt
来源：http://fo.wgjwhj.cn

[R43] 按名字查找文件
来源：http://hz.lnxyls.cn

find . -name "*.log" -type f
来源：http://uk.shtwfgs.cn

[R44] 按修改时间查找
来源：http://ko.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://nb.chemitech.net.cn

[R45] 批量删除
来源：http://ne.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://jd.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://ui.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zr.bookmarksfly.cn

[R47] sed 单行替换
来源：http://oa.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fz.muxihuayi.cn

[R48] awk 取指定列
来源：http://jk.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://px.521024.cn

[R49] awk 带条件
来源：http://hw.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hg.muxihuayi.cn

[R50] awk 求和
来源：http://nc.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xo.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://pt.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jl.szxytkj.cn

[R52] 统计行数
来源：http://df.yuexingan06.cn

wc -l a.txt
来源：http://cv.colortex.cn

[R53] 查看文件头与实时尾
来源：http://yr.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oc.haigaiapp.cn

[R54] 比较两个文件
来源：http://qs.huixinmuqiang.cn

diff a.txt b.txt
来源：http://wj.shxzukj.cn

[R55] 压缩与解压
来源：http://kd.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://go.jctech888.com.cn

[R56] 远程拷贝
来源：http://rv.panjiajie.cn

scp file user@host:/path/
来源：http://cy.nszjky.cn

[R57] 远程执行命令
来源：http://rv.jctech888.com.cn

ssh user@host 'uptime'
来源：http://qi.bjjhwx.cn

[R58] 下载文件
来源：http://zt.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hy.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ob.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://at.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://hv.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mj.asd995.cn

[R61] 磁盘占用
来源：http://rk.chemitech.net.cn

df -h;  du -sh *
来源：http://gg.521024.cn

[R62] 找最占空间的文件
来源：http://wb.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://ev.hnjuh.cn

[R63] 内存与进程
来源：http://db.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://ts.szxytkj.cn

[R64] 结束进程
来源：http://yw.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://wg.hahajie.cn

[R65] 查看端口占用
来源：http://rp.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://id.asd995.cn

[R66] 定时任务
来源：http://ez.9csxet.cn

crontab -e;  crontab -l
来源：http://tp.szsharing.cn

[R67] 生成随机十六进制串
来源：http://en.yuntaijiaju.cn

openssl rand -hex 16
来源：http://al.huanxung.cn

[R68] 计算文件校验值
来源：http://rc.bjjhwx.cn

sha256sum a.txt;  md5sum a.txt
来源：http://do.shxzukj.cn

[R69] 生成随机密码
来源：http://dd.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://mm.nszjky.cn

[R70] 时间戳与互转
来源：http://pb.huanxung.cn

date +%s;  date -d @1700000000
来源：http://gh.newstarts.cn

[R71] 日期格式化
来源：http://is.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tm.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://nv.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qy.shxzukj.cn

[R73] 分割大日志
来源：http://sr.bjjhwx.cn

split -l 1000 big.log part_
来源：http://al.huixinmuqiang.cn

[R74] 批量重命名
来源：http://yv.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qx.panjiajie.cn

[R75] 导出环境变量
来源：http://la.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://yo.huixiangedu.cn

[R76] 使用临时文件
来源：http://bo.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qa.hahajie.cn

[R77] 读取用户输入
来源：http://tr.panjiajie.cn

read -rp "请输入: " ans
来源：http://km.shxzskj.cn

[R78] 交互式菜单
来源：http://vu.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ck.szsharing.cn

[R79] 解析命令行选项
来源：http://zj.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tn.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://qk.colortex.cn

time ./run.sh
来源：http://ye.szxytkj.cn

================================================================================
来源：http://vc.nszjky.cn

S. C / C++ 专题
来源：http://ss.haigaiapp.cn

================================================================================
来源：http://hy.jianghongdianzi.cn

[S01] C：Hello World
来源：http://yj.bookmarksfly.cn

#include <stdio.h>
来源：http://iv.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://or.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://hn.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://ql.newstarts.cn

[S03] C：读入整数
来源：http://jp.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://fw.lnxyls.cn

[S04] C：字符串复制
来源：http://yz.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tb.newstarts.cn

[S05] C：字符串长度
来源：http://tl.shxzukj.cn

strlen(s)
来源：http://ts.szsharing.cn

[S06] C：字符串比较
来源：http://eb.newstarts.cn

strcmp(a, b) == 0
来源：http://bo.hahajie.cn

[S07] C：数组遍历求和
来源：http://sz.yuexingan06.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qi.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://kk.wgjwhj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://su.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://qd.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://db.szxytkj.cn

[S10] C：指针与解引用
来源：http://bu.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://su.yuexingan06.cn

[S11] C：逐行读文件
来源：http://df.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://it.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yn.szsharing.cn

fclose(f);
来源：http://ez.shxzukj.cn

[S12] C：写文件
来源：http://pj.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ae.haigaiapp.cn

[S13] C：宏定义
来源：http://tk.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uz.9csxet.cn

[S14] C：枚举
来源：http://er.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://tk.szsharing.cn

[S15] C：类型转换
来源：http://cs.wgjwhj.cn

(double) a / b
来源：http://ct.gzmigu.cn

[S16] C：位操作置位
来源：http://dh.hahajie.cn

x |= (1 << 3);
来源：http://vt.521024.cn

[S17] C：安全拼接字符串
来源：http://wh.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nw.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://cx.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://pt.9csxet.cn

[S19] C：快速排序
来源：http://sz.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wd.newstarts.cn

[S20] C：二分查找
来源：http://gv.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qr.szsharing.cn

[S21] C：字符类别判断
来源：http://pm.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dy.szxytkj.cn

[S22] C：字符串转数字
来源：http://iu.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qw.bookmarksfly.cn

[S23] C：随机数
来源：http://gq.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ki.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://uz.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vy.chemitech.net.cn

[S25] C：内存拷贝
来源：http://vk.newstarts.cn

memcpy(dst, src, n);
来源：http://ip.yuexingan06.cn

[S26] C：内存清零
来源：http://rx.newstarts.cn

memset(a, 0, sizeof a);
来源：http://lm.bookmarksfly.cn

[S27] C：定义常量
来源：http://oq.lnxyls.cn

const double PI = 3.14159;
来源：http://aw.muxihuayi.cn

[S28] C：静态变量
来源：http://aw.nicolike.cn

static int counter = 0;
来源：http://qw.panjiajie.cn

[S29] C：变参函数
来源：http://on.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ep.asd995.cn

[S30] C：头文件保护
来源：http://ae.shxzskj.cn

#ifndef X_H
来源：http://tu.521024.cn

#define X_H
来源：http://sw.haigaiapp.cn

#endif
来源：http://yl.haigaiapp.cn

[S31] C++：Hello World
来源：http://ac.9csxet.cn

#include <iostream>
来源：http://ek.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://gy.huixinmuqiang.cn

[S32] C++：字符串
来源：http://np.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://yj.nszjky.cn


<!-- 参考信息 -->