代发 wailian999

[Q63] 开启事务
来源：http://ev.panjiajie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ph.szxytkj.cn

[Q64] 提交事务
来源：http://fw.lnxyls.cn

COMMIT;
来源：http://im.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://yy.jctech888.com.cn

ROLLBACK;
来源：http://ce.colortex.cn

[Q66] 行锁查询
来源：http://pg.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ul.bookmarksfly.cn

[Q67] 设置隔离级别
来源：http://ic.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jz.wgjwhj.cn

[Q68] 保存点
来源：http://pi.panjiajie.cn

SAVEPOINT sp1;
来源：http://qw.huanxung.cn

ROLLBACK TO sp1;
来源：http://yi.nszjky.cn

[Q69] 查看执行计划
来源：http://rv.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ha.gzmigu.cn

[Q70] 更新统计信息
来源：http://hh.shxzskj.cn

ANALYZE TABLE users;
来源：http://bi.jctech888.com.cn

[Q71] 查看建表语句
来源：http://uy.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ao.colortex.cn

[Q72] 查看索引
来源：http://pq.hahajie.cn

SHOW INDEX FROM users;
来源：http://vu.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://mx.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vj.huanxung.cn

[Q74] 强制使用索引
来源：http://kp.bookmarksfly.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zt.jctech888.com.cn

[Q75] 日期格式化
来源：http://bo.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://it.bookmarksfly.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vh.521024.cn

[Q76] 按天统计
来源：http://ye.bjjhwx.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pz.asd995.cn

[Q77] 时间加减
来源：http://nr.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jc.shtwfgs.cn

[Q78] 当前时间
来源：http://cm.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ht.jctech888.com.cn

[Q79] 字符串拼接
来源：http://qy.gzmigu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vd.lnxyls.cn

[Q80] 字符串截取
来源：http://wn.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ez.lnxyls.cn

[Q81] 字符串替换
来源：http://la.gzmigu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tr.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://xd.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cm.bookmarksfly.cn

[Q83] 大小写转换
来源：http://bl.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fo.521024.cn

[Q84] 去除首尾空格
来源：http://iu.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://qk.asd995.cn

[Q85] 数值取整
来源：http://rb.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ge.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://rm.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nf.9csxet.cn

[Q87] JSON 字段做条件
来源：http://xs.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ss.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://uw.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xn.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kp.huanxung.cn

[Q89] 判断表是否存在
来源：http://kt.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://do.yuexingan06.cn

[Q90] 生成序号列
来源：http://ip.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yv.shxzskj.cn

================================================================================
来源：http://vs.haigaiapp.cn

R. Bash 专题
来源：http://xk.jianghongdianzi.cn

================================================================================
来源：http://fc.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://jq.hnjuh.cn

#!/usr/bin/env bash
来源：http://dg.hnjuh.cn

set -euo pipefail
来源：http://hj.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://dx.shxzukj.cn

name="Tom"; echo "$name"
来源：http://fj.newstarts.cn

[R03] 只读变量
来源：http://ih.jianghongdianzi.cn

readonly PI=3.14
来源：http://bf.shxzskj.cn

[R04] 位置参数
来源：http://kg.gzmigu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xq.521024.cn

[R05] 参数默认值
来源：http://zn.chemitech.net.cn

name="${1:-default}"
来源：http://gh.nszjky.cn

[R06] 判断命令是否存在
来源：http://oh.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ps.huanxung.cn

[R07] if 判断文件
来源：http://qp.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gi.bjjhwx.cn

[R08] 数值比较
来源：http://cu.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dc.hnjuh.cn

[R09] 字符串比较
来源：http://ir.jctech888.com.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ax.gzmigu.cn

[R10] 正则匹配
来源：http://re.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ul.huanxung.cn

[R11] case 多分支
来源：http://wj.nszjky.cn

case "$1" in
来源：http://ra.huanxung.cn

start) echo "启动" ;;
来源：http://dj.lnxyls.cn

stop)  echo "停止" ;;
来源：http://uo.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://xu.bookmarksfly.cn

esac
来源：http://qe.huanxung.cn

[R12] for 遍历文件
来源：http://bk.bookmarksfly.cn

for f in *.txt; do echo "$f"; done
来源：http://wp.haigaiapp.cn

[R13] for 计数循环
来源：http://tm.yuexingan06.cn

for i in {1..10}; do echo "$i"; done
来源：http://uv.nszjky.cn

[R14] C 风格 for
来源：http://kc.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xp.huixinmuqiang.cn

[R15] while 逐行读文件
来源：http://sm.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lm.hnjuh.cn

[R16] until 等待条件
来源：http://dy.asd995.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kj.szsharing.cn

[R17] 数组定义与取值
来源：http://td.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uo.szsharing.cn

[R18] 遍历数组
来源：http://xk.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jo.wgjwhj.cn

[R19] 数组长度
来源：http://ta.muxihuayi.cn

echo "${#arr[@]}"
来源：http://xw.gzmigu.cn

[R20] 关联数组（字典）
来源：http://jy.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uj.521024.cn

[R21] 字符串长度
来源：http://vt.shxzukj.cn

echo "${#s}"
来源：http://ot.shxzskj.cn

[R22] 截取子串
来源：http://mp.jctech888.com.cn

echo "${s:0:5}"
来源：http://kh.shxzskj.cn

[R23] 字符串替换
来源：http://ff.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xc.huixiangedu.cn

[R24] 大小写转换
来源：http://bd.szsharing.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ct.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://bd.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ki.shxzskj.cn

[R26] 命令替换
来源：http://vo.haigaiapp.cn

now=$(date +%F); echo "$now"
来源：http://bv.jctech888.com.cn

[R27] 算术展开
来源：http://bz.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://hy.szxytkj.cn

[R28] 浮点运算
来源：http://kd.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://ib.bjjhwx.cn

[R29] 定义函数
来源：http://pk.nszjky.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ad.haigaiapp.cn

[R30] 函数返回状态码
来源：http://gn.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://uu.nicolike.cn

[R31] 局部变量
来源：http://uw.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://gq.hahajie.cn

[R32] 参数个数校验
来源：http://jh.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iu.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://nz.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lf.hnjuh.cn

[R34] 退出时清理
来源：http://sl.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xi.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://qe.chemitech.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tx.521024.cn

[R36] 并发执行多个任务
来源：http://qh.asd995.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ad.asd995.cn

[R37] 把输出赋给变量
来源：http://xe.panjiajie.cn

files=$(ls -1)
来源：http://lt.gzmigu.cn

[R38] 管道串联
来源：http://vt.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://xc.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://vi.huixiangedu.cn

cmd > out.log 2>&1
来源：http://az.huanxung.cn

[R40] 追加写日志
来源：http://mx.muxihuayi.cn

echo "log" >> out.log
来源：http://ki.nszjky.cn

[R41] 丢弃输出
来源：http://xp.szsharing.cn

cmd >/dev/null 2>&1
来源：http://zg.shxzskj.cn

[R42] 输入重定向
来源：http://bj.haigaiapp.cn

wc -l < a.txt
来源：http://el.shtwfgs.cn

[R43] 按名字查找文件
来源：http://pw.newstarts.cn

find . -name "*.log" -type f
来源：http://qb.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://uu.wgjwhj.cn

find . -mtime -7 -type f
来源：http://yg.nszjky.cn

[R45] 批量删除
来源：http://vl.yuntaijiaju.cn

find . -name "*.tmp" -delete
来源：http://yq.newstarts.cn

[R46] 递归替换文件内容
来源：http://hu.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sm.hahajie.cn

[R47] sed 单行替换
来源：http://pc.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cp.huixiangedu.cn

[R48] awk 取指定列
来源：http://vp.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://bg.huanxung.cn

[R49] awk 带条件
来源：http://ut.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://av.szsharing.cn

[R50] awk 求和
来源：http://vo.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lp.shtwfgs.cn

[R51] 排序去重取前几
来源：http://tu.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xl.wgjwhj.cn

[R52] 统计行数
来源：http://ok.szsharing.cn

wc -l a.txt
来源：http://rh.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://fz.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ti.szxytkj.cn

[R54] 比较两个文件
来源：http://di.hnjuh.cn

diff a.txt b.txt
来源：http://le.wgjwhj.cn

[R55] 压缩与解压
来源：http://fs.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cz.9csxet.cn

[R56] 远程拷贝
来源：http://ur.szsharing.cn

scp file user@host:/path/
来源：http://ic.szxytkj.cn

[R57] 远程执行命令
来源：http://wo.nicolike.cn

ssh user@host 'uptime'
来源：http://py.panjiajie.cn

[R58] 下载文件
来源：http://dp.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cm.hnjuh.cn

[R59] 发 POST JSON
来源：http://nq.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vw.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://td.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lj.shxzskj.cn

[R61] 磁盘占用
来源：http://ai.hnjuh.cn

df -h;  du -sh *
来源：http://te.shxzukj.cn

[R62] 找最占空间的文件
来源：http://nr.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://bk.hnjuh.cn

[R63] 内存与进程
来源：http://rh.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://ld.gzmigu.cn

[R64] 结束进程
来源：http://de.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://av.gzmigu.cn

[R65] 查看端口占用
来源：http://gd.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kp.szsharing.cn

[R66] 定时任务
来源：http://uc.colortex.cn

crontab -e;  crontab -l
来源：http://ku.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://yb.nszjky.cn

openssl rand -hex 16
来源：http://wq.hahajie.cn

[R68] 计算文件校验值
来源：http://cz.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pk.haigaiapp.cn

[R69] 生成随机密码
来源：http://fw.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://ll.521024.cn

[R70] 时间戳与互转
来源：http://kx.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://vv.bookmarksfly.cn

[R71] 日期格式化
来源：http://ff.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://da.hnjuh.cn

[R72] 等待端口就绪
来源：http://mx.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pc.hahajie.cn

[R73] 分割大日志
来源：http://ih.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://pm.nicolike.cn

[R74] 批量重命名
来源：http://bs.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yr.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://nl.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://nm.gzmigu.cn

[R76] 使用临时文件
来源：http://co.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eq.huanxung.cn

[R77] 读取用户输入
来源：http://kt.shxzukj.cn

read -rp "请输入: " ans
来源：http://is.gzmigu.cn

[R78] 交互式菜单
来源：http://nv.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uc.lnxyls.cn

[R79] 解析命令行选项
来源：http://wk.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ji.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://wj.hahajie.cn

time ./run.sh
来源：http://xl.szxytkj.cn

================================================================================
来源：http://oe.nicolike.cn

S. C / C++ 专题
来源：http://vp.huixinmuqiang.cn

================================================================================
来源：http://bg.yuntaijiaju.cn

[S01] C：Hello World
来源：http://jl.huixiangedu.cn

#include <stdio.h>
来源：http://ta.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vm.huanxung.cn

[S02] C：变量与格式化输出
来源：http://ph.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://gk.newstarts.cn

[S03] C：读入整数
来源：http://hd.jctech888.com.cn

int x; scanf("%d", &x);
来源：http://fd.colortex.cn

[S04] C：字符串复制
来源：http://ep.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sj.shtwfgs.cn

[S05] C：字符串长度
来源：http://zd.bjjhwx.cn

strlen(s)
来源：http://gy.nszjky.cn

[S06] C：字符串比较
来源：http://fi.panjiajie.cn

strcmp(a, b) == 0
来源：http://ps.szxytkj.cn

[S07] C：数组遍历求和
来源：http://lu.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wa.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://go.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://az.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://wo.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cm.bjjhwx.cn

[S10] C：指针与解引用
来源：http://eq.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://yr.colortex.cn

[S11] C：逐行读文件
来源：http://cz.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://iu.yuntaijiaju.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dl.huixiangedu.cn

fclose(f);
来源：http://mh.nicolike.cn

[S12] C：写文件
来源：http://nh.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jg.yuexingan06.cn

[S13] C：宏定义
来源：http://ak.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ka.shtwfgs.cn

[S14] C：枚举
来源：http://sm.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://sc.nszjky.cn

[S15] C：类型转换
来源：http://qw.hahajie.cn

(double) a / b
来源：http://kq.hahajie.cn

[S16] C：位操作置位
来源：http://gh.9csxet.cn

x |= (1 << 3);
来源：http://kk.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://nf.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://li.hnjuh.cn

[S18] C：命令行参数
来源：http://dh.nszjky.cn

int main(int argc, char **argv)
来源：http://ew.huixinmuqiang.cn

[S19] C：快速排序
来源：http://mz.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ok.shtwfgs.cn

[S20] C：二分查找
来源：http://rw.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.jctech888.com.cn

[S21] C：字符类别判断
来源：http://vu.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nc.bjjhwx.cn

[S22] C：字符串转数字
来源：http://ws.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vf.hahajie.cn

[S23] C：随机数
来源：http://hd.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mz.nicolike.cn

[S24] C：获取本地时间
来源：http://cm.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://de.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://nt.wgjwhj.cn

memcpy(dst, src, n);
来源：http://lc.bookmarksfly.cn

[S26] C：内存清零
来源：http://ea.9csxet.cn

memset(a, 0, sizeof a);
来源：http://oy.shxzskj.cn

[S27] C：定义常量
来源：http://kq.lnxyls.cn

const double PI = 3.14159;
来源：http://tg.jctech888.com.cn

[S28] C：静态变量
来源：http://kb.muxihuayi.cn

static int counter = 0;
来源：http://ua.wgjwhj.cn

[S29] C：变参函数
来源：http://to.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fh.gzmigu.cn

[S30] C：头文件保护
来源：http://bq.shxzukj.cn

#ifndef X_H
来源：http://dr.lnxyls.cn

#define X_H
来源：http://ph.nicolike.cn

#endif
来源：http://vj.newstarts.cn

[S31] C++：Hello World
来源：http://nx.hnjuh.cn

#include <iostream>
来源：http://rd.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://kq.yuexingan06.cn

[S32] C++：字符串
来源：http://sp.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://xg.colortex.cn


<!-- 参考信息 -->