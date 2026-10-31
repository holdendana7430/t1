代发 wailian999

[Q65] 回滚事务
来源：http://un.shxzskj.cn

ROLLBACK;
来源：http://ti.huixinmuqiang.cn

[Q66] 行锁查询
来源：http://yp.shxzskj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zh.huanxung.cn

[Q67] 设置隔离级别
来源：http://bd.hahajie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ph.shtwfgs.cn

[Q68] 保存点
来源：http://dz.huixinmuqiang.cn

SAVEPOINT sp1;
来源：http://pf.szxytkj.cn

ROLLBACK TO sp1;
来源：http://re.bjjhwx.cn

[Q69] 查看执行计划
来源：http://fv.yuntaijiaju.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fd.wgjwhj.cn

[Q70] 更新统计信息
来源：http://lq.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://dz.haigaiapp.cn

[Q71] 查看建表语句
来源：http://ke.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jw.nszjky.cn

[Q72] 查看索引
来源：http://hl.lnxyls.cn

SHOW INDEX FROM users;
来源：http://fc.bjjhwx.cn

[Q73] 查看表状态
来源：http://hr.haigaiapp.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ps.colortex.cn

[Q74] 强制使用索引
来源：http://lk.yuntaijiaju.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xq.asd995.cn

[Q75] 日期格式化
来源：http://md.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uk.bjjhwx.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vv.huixiangedu.cn

[Q76] 按天统计
来源：http://zj.muxihuayi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nz.hahajie.cn

[Q77] 时间加减
来源：http://ve.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xf.colortex.cn

[Q78] 当前时间
来源：http://zk.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ny.9csxet.cn

[Q79] 字符串拼接
来源：http://qe.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sg.huanxung.cn

[Q80] 字符串截取
来源：http://ly.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ig.shxzskj.cn

[Q81] 字符串替换
来源：http://bu.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iy.colortex.cn

[Q82] 字符长度与字节长度
来源：http://aq.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kc.haigaiapp.cn

[Q83] 大小写转换
来源：http://bv.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yz.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://tc.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://yt.chemitech.net.cn

[Q85] 数值取整
来源：http://im.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tp.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://gk.shxzskj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bl.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://zk.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wy.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://wj.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hw.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kv.szxytkj.cn

[Q89] 判断表是否存在
来源：http://uo.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cg.huanxung.cn

[Q90] 生成序号列
来源：http://gb.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mi.nszjky.cn

================================================================================
来源：http://kl.shxzukj.cn

R. Bash 专题
来源：http://me.szxytkj.cn

================================================================================
来源：http://mo.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://hg.nicolike.cn

#!/usr/bin/env bash
来源：http://yu.9csxet.cn

set -euo pipefail
来源：http://cd.nszjky.cn

[R02] 变量赋值与使用
来源：http://vs.newstarts.cn

name="Tom"; echo "$name"
来源：http://oj.shtwfgs.cn

[R03] 只读变量
来源：http://wf.szsharing.cn

readonly PI=3.14
来源：http://mf.haigaiapp.cn

[R04] 位置参数
来源：http://ra.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qs.asd995.cn

[R05] 参数默认值
来源：http://uw.huixinmuqiang.cn

name="${1:-default}"
来源：http://aa.shxzukj.cn

[R06] 判断命令是否存在
来源：http://nt.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qy.muxihuayi.cn

[R07] if 判断文件
来源：http://yq.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qn.shtwfgs.cn

[R08] 数值比较
来源：http://ev.jianghongdianzi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kz.panjiajie.cn

[R09] 字符串比较
来源：http://hm.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sb.hahajie.cn

[R10] 正则匹配
来源：http://je.lnxyls.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cq.hnjuh.cn

[R11] case 多分支
来源：http://fl.gzmigu.cn

case "$1" in
来源：http://ii.bookmarksfly.cn

start) echo "启动" ;;
来源：http://ud.hnjuh.cn

stop)  echo "停止" ;;
来源：http://dz.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://zv.bjjhwx.cn

esac
来源：http://xr.bookmarksfly.cn

[R12] for 遍历文件
来源：http://nt.muxihuayi.cn

for f in *.txt; do echo "$f"; done
来源：http://sz.9csxet.cn

[R13] for 计数循环
来源：http://yj.shxzskj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ew.shxzukj.cn

[R14] C 风格 for
来源：http://dl.bjjhwx.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ix.chemitech.net.cn

[R15] while 逐行读文件
来源：http://es.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xw.haigaiapp.cn

[R16] until 等待条件
来源：http://rw.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://td.9csxet.cn

[R17] 数组定义与取值
来源：http://ga.panjiajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ou.jianghongdianzi.cn

[R18] 遍历数组
来源：http://kx.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mw.szsharing.cn

[R19] 数组长度
来源：http://zp.nicolike.cn

echo "${#arr[@]}"
来源：http://mb.jianghongdianzi.cn

[R20] 关联数组（字典）
来源：http://vf.jctech888.com.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ft.gzmigu.cn

[R21] 字符串长度
来源：http://rr.shxzukj.cn

echo "${#s}"
来源：http://bd.colortex.cn

[R22] 截取子串
来源：http://yp.nicolike.cn

echo "${s:0:5}"
来源：http://iv.colortex.cn

[R23] 字符串替换
来源：http://bq.bookmarksfly.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ql.panjiajie.cn

[R24] 大小写转换
来源：http://jz.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cw.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://jm.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yk.shxzskj.cn

[R26] 命令替换
来源：http://bn.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://ax.haigaiapp.cn

[R27] 算术展开
来源：http://vl.lnxyls.cn

echo $((1 + 2 * 3))
来源：http://yu.nicolike.cn

[R28] 浮点运算
来源：http://rh.chemitech.net.cn

echo "scale=2; 10/3" | bc
来源：http://cl.bookmarksfly.cn

[R29] 定义函数
来源：http://jj.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ok.newstarts.cn

[R30] 函数返回状态码
来源：http://hk.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://dl.bookmarksfly.cn

[R31] 局部变量
来源：http://lv.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://iy.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://hu.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vn.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://tm.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ls.yuntaijiaju.cn

[R34] 退出时清理
来源：http://xy.shtwfgs.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jo.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://ux.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xt.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ti.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://so.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://sb.nicolike.cn

files=$(ls -1)
来源：http://dy.huixinmuqiang.cn

[R38] 管道串联
来源：http://pz.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://kg.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://rw.colortex.cn

cmd > out.log 2>&1
来源：http://vc.nszjky.cn

[R40] 追加写日志
来源：http://hf.hahajie.cn

echo "log" >> out.log
来源：http://ae.wgjwhj.cn

[R41] 丢弃输出
来源：http://kc.shtwfgs.cn

cmd >/dev/null 2>&1
来源：http://ri.hnjuh.cn

[R42] 输入重定向
来源：http://mm.chemitech.net.cn

wc -l < a.txt
来源：http://cm.yuexingan06.cn

[R43] 按名字查找文件
来源：http://qj.shtwfgs.cn

find . -name "*.log" -type f
来源：http://ly.nszjky.cn

[R44] 按修改时间查找
来源：http://oj.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://bf.hnjuh.cn

[R45] 批量删除
来源：http://rj.chemitech.net.cn

find . -name "*.tmp" -delete
来源：http://vn.nszjky.cn

[R46] 递归替换文件内容
来源：http://ss.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gu.521024.cn

[R47] sed 单行替换
来源：http://xj.yuntaijiaju.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yy.colortex.cn

[R48] awk 取指定列
来源：http://ce.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://il.muxihuayi.cn

[R49] awk 带条件
来源：http://yx.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rv.jctech888.com.cn

[R50] awk 求和
来源：http://lk.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xf.szsharing.cn

[R51] 排序去重取前几
来源：http://zg.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ru.hahajie.cn

[R52] 统计行数
来源：http://le.shxzskj.cn

wc -l a.txt
来源：http://cd.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://nf.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://il.szsharing.cn

[R54] 比较两个文件
来源：http://qy.nszjky.cn

diff a.txt b.txt
来源：http://tp.wgjwhj.cn

[R55] 压缩与解压
来源：http://zd.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jl.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://fz.521024.cn

scp file user@host:/path/
来源：http://qg.asd995.cn

[R57] 远程执行命令
来源：http://eu.wgjwhj.cn

ssh user@host 'uptime'
来源：http://mo.huixiangedu.cn

[R58] 下载文件
来源：http://mc.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sd.wgjwhj.cn

[R59] 发 POST JSON
来源：http://jf.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://is.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://hj.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nt.lnxyls.cn

[R61] 磁盘占用
来源：http://dh.huanxung.cn

df -h;  du -sh *
来源：http://nm.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://hr.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://fj.521024.cn

[R63] 内存与进程
来源：http://cg.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://el.bjjhwx.cn

[R64] 结束进程
来源：http://sj.yuexingan06.cn

kill -9 $(pgrep -f app.py)
来源：http://ag.hahajie.cn

[R65] 查看端口占用
来源：http://cp.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rr.szxytkj.cn

[R66] 定时任务
来源：http://yp.muxihuayi.cn

crontab -e;  crontab -l
来源：http://wa.colortex.cn

[R67] 生成随机十六进制串
来源：http://lt.jianghongdianzi.cn

openssl rand -hex 16
来源：http://gq.bjjhwx.cn

[R68] 计算文件校验值
来源：http://gf.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gv.haigaiapp.cn

[R69] 生成随机密码
来源：http://cm.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://nr.jctech888.com.cn

[R70] 时间戳与互转
来源：http://av.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://ub.yuexingan06.cn

[R71] 日期格式化
来源：http://mj.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ku.panjiajie.cn

[R72] 等待端口就绪
来源：http://lt.chemitech.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tx.521024.cn

[R73] 分割大日志
来源：http://jf.shtwfgs.cn

split -l 1000 big.log part_
来源：http://nq.huanxung.cn

[R74] 批量重命名
来源：http://mv.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://be.muxihuayi.cn

[R75] 导出环境变量
来源：http://dw.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://qu.shxzskj.cn

[R76] 使用临时文件
来源：http://dp.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xe.asd995.cn

[R77] 读取用户输入
来源：http://iz.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ed.yuntaijiaju.cn

[R78] 交互式菜单
来源：http://af.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ey.shxzskj.cn

[R79] 解析命令行选项
来源：http://pk.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gq.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://nk.shxzskj.cn

time ./run.sh
来源：http://lp.9csxet.cn

================================================================================
来源：http://fg.colortex.cn

S. C / C++ 专题
来源：http://lj.yuexingan06.cn

================================================================================
来源：http://cz.newstarts.cn

[S01] C：Hello World
来源：http://fe.muxihuayi.cn

#include <stdio.h>
来源：http://rc.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iq.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://zv.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://hb.szsharing.cn

[S03] C：读入整数
来源：http://ti.szxytkj.cn

int x; scanf("%d", &x);
来源：http://ip.chemitech.net.cn

[S04] C：字符串复制
来源：http://vq.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ff.wgjwhj.cn

[S05] C：字符串长度
来源：http://sa.nszjky.cn

strlen(s)
来源：http://sf.huanxung.cn

[S06] C：字符串比较
来源：http://sy.asd995.cn

strcmp(a, b) == 0
来源：http://qu.nicolike.cn

[S07] C：数组遍历求和
来源：http://xf.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fo.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://yy.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ba.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ea.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sn.jctech888.com.cn

[S10] C：指针与解引用
来源：http://dm.nicolike.cn

int *p = &a;  *p = 5;
来源：http://rs.lnxyls.cn

[S11] C：逐行读文件
来源：http://od.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://hu.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://px.wgjwhj.cn

fclose(f);
来源：http://me.nszjky.cn

[S12] C：写文件
来源：http://vc.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://va.muxihuayi.cn

[S13] C：宏定义
来源：http://bf.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jc.hahajie.cn

[S14] C：枚举
来源：http://yk.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://vm.521024.cn

[S15] C：类型转换
来源：http://tt.bjjhwx.cn

(double) a / b
来源：http://vf.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://sd.chemitech.net.cn

x |= (1 << 3);
来源：http://cg.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://tc.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rj.newstarts.cn

[S18] C：命令行参数
来源：http://ax.shxzukj.cn

int main(int argc, char **argv)
来源：http://fp.nszjky.cn

[S19] C：快速排序
来源：http://wd.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nk.gzmigu.cn

[S20] C：二分查找
来源：http://dz.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wk.nicolike.cn

[S21] C：字符类别判断
来源：http://xt.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xb.nszjky.cn

[S22] C：字符串转数字
来源：http://tj.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zt.lnxyls.cn

[S23] C：随机数
来源：http://kg.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xe.panjiajie.cn

[S24] C：获取本地时间
来源：http://rd.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ca.muxihuayi.cn

[S25] C：内存拷贝
来源：http://wy.colortex.cn

memcpy(dst, src, n);
来源：http://rq.hnjuh.cn

[S26] C：内存清零
来源：http://vc.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://cl.nszjky.cn

[S27] C：定义常量
来源：http://sw.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://mu.yuexingan06.cn

[S28] C：静态变量
来源：http://ar.newstarts.cn

static int counter = 0;
来源：http://uy.521024.cn

[S29] C：变参函数
来源：http://cz.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rr.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ah.lnxyls.cn

#ifndef X_H
来源：http://ih.yuexingan06.cn

#define X_H
来源：http://ya.jctech888.com.cn

#endif
来源：http://vu.muxihuayi.cn

[S31] C++：Hello World
来源：http://hh.huanxung.cn

#include <iostream>
来源：http://gd.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://xb.haigaiapp.cn

[S32] C++：字符串
来源：http://oo.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://qt.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://dl.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rx.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://lx.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ks.panjiajie.cn


<!-- 参考信息 -->