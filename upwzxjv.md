代发 wailian999

[Q65] 回滚事务
来源：http://wj.haigaiapp.cn

ROLLBACK;
来源：http://ye.szsharing.cn

[Q66] 行锁查询
来源：http://eg.newstarts.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eq.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://si.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://em.gzmigu.cn

[Q68] 保存点
来源：http://ms.asd995.cn

SAVEPOINT sp1;
来源：http://zi.bookmarksfly.cn

ROLLBACK TO sp1;
来源：http://gm.panjiajie.cn

[Q69] 查看执行计划
来源：http://cr.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://du.muxihuayi.cn

[Q70] 更新统计信息
来源：http://qx.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://os.wgjwhj.cn

[Q71] 查看建表语句
来源：http://re.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rp.haigaiapp.cn

[Q72] 查看索引
来源：http://yg.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://af.hnjuh.cn

[Q73] 查看表状态
来源：http://fu.hnjuh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fq.521024.cn

[Q74] 强制使用索引
来源：http://sz.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tb.yuexingan06.cn

[Q75] 日期格式化
来源：http://nj.yuntaijiaju.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fz.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mo.huixinmuqiang.cn

[Q76] 按天统计
来源：http://uc.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rm.lnxyls.cn

[Q77] 时间加减
来源：http://dp.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bc.chemitech.net.cn

[Q78] 当前时间
来源：http://dq.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eq.szsharing.cn

[Q79] 字符串拼接
来源：http://vv.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lv.nicolike.cn

[Q80] 字符串截取
来源：http://yl.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ir.huanxung.cn

[Q81] 字符串替换
来源：http://rv.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jl.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://tv.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://az.nszjky.cn

[Q83] 大小写转换
来源：http://mg.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ad.lnxyls.cn

[Q84] 去除首尾空格
来源：http://ja.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://eb.haigaiapp.cn

[Q85] 数值取整
来源：http://tf.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sv.yuexingan06.cn

[Q86] 读取 JSON 字段
来源：http://pg.nszjky.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gl.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://rd.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dx.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://iu.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://up.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pv.huixinmuqiang.cn

[Q89] 判断表是否存在
来源：http://if.lnxyls.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oe.shxzskj.cn

[Q90] 生成序号列
来源：http://uw.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dj.haigaiapp.cn

================================================================================
来源：http://ly.huixinmuqiang.cn

R. Bash 专题
来源：http://ey.lnxyls.cn

================================================================================
来源：http://gz.asd995.cn

[R01] shebang 与严格模式
来源：http://cb.shxzukj.cn

#!/usr/bin/env bash
来源：http://ym.shxzskj.cn

set -euo pipefail
来源：http://ch.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://es.shxzskj.cn

name="Tom"; echo "$name"
来源：http://ol.shxzukj.cn

[R03] 只读变量
来源：http://un.hahajie.cn

readonly PI=3.14
来源：http://mk.bjjhwx.cn

[R04] 位置参数
来源：http://te.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vt.panjiajie.cn

[R05] 参数默认值
来源：http://ge.lnxyls.cn

name="${1:-default}"
来源：http://va.panjiajie.cn

[R06] 判断命令是否存在
来源：http://hx.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xk.shxzukj.cn

[R07] if 判断文件
来源：http://yp.hnjuh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tp.colortex.cn

[R08] 数值比较
来源：http://ne.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pb.shxzskj.cn

[R09] 字符串比较
来源：http://us.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ey.shxzukj.cn

[R10] 正则匹配
来源：http://nr.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fm.bjjhwx.cn

[R11] case 多分支
来源：http://hf.yuexingan06.cn

case "$1" in
来源：http://ln.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://ef.hahajie.cn

stop)  echo "停止" ;;
来源：http://bn.gzmigu.cn

*)     echo "未知命令" ;;
来源：http://sm.9csxet.cn

esac
来源：http://am.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ba.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://xb.hnjuh.cn

[R13] for 计数循环
来源：http://ts.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://np.panjiajie.cn

[R14] C 风格 for
来源：http://lc.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ij.shtwfgs.cn

[R15] while 逐行读文件
来源：http://jl.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://re.nszjky.cn

[R16] until 等待条件
来源：http://pq.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ck.nszjky.cn

[R17] 数组定义与取值
来源：http://sa.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ib.nicolike.cn

[R18] 遍历数组
来源：http://hd.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ga.jianghongdianzi.cn

[R19] 数组长度
来源：http://gh.nszjky.cn

echo "${#arr[@]}"
来源：http://iv.hnjuh.cn

[R20] 关联数组（字典）
来源：http://jf.szsharing.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nn.colortex.cn

[R21] 字符串长度
来源：http://zn.bjjhwx.cn

echo "${#s}"
来源：http://jt.panjiajie.cn

[R22] 截取子串
来源：http://cb.colortex.cn

echo "${s:0:5}"
来源：http://ju.bjjhwx.cn

[R23] 字符串替换
来源：http://di.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://to.yuexingan06.cn

[R24] 大小写转换
来源：http://fo.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zu.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://yl.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xr.jianghongdianzi.cn

[R26] 命令替换
来源：http://fo.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://kn.shxzskj.cn

[R27] 算术展开
来源：http://tl.nicolike.cn

echo $((1 + 2 * 3))
来源：http://yi.huixiangedu.cn

[R28] 浮点运算
来源：http://bx.szxytkj.cn

echo "scale=2; 10/3" | bc
来源：http://zu.9csxet.cn

[R29] 定义函数
来源：http://ke.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dt.haigaiapp.cn

[R30] 函数返回状态码
来源：http://xs.yuexingan06.cn

f() { return 0; }; f || echo "失败了"
来源：http://ee.wgjwhj.cn

[R31] 局部变量
来源：http://lt.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://fy.panjiajie.cn

[R32] 参数个数校验
来源：http://bf.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kl.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://te.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ro.yuexingan06.cn

[R34] 退出时清理
来源：http://tr.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ao.szxytkj.cn

[R35] 后台执行并等待
来源：http://ak.hahajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nq.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://nb.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ms.lnxyls.cn

[R37] 把输出赋给变量
来源：http://ck.shxzukj.cn

files=$(ls -1)
来源：http://sc.huanxung.cn

[R38] 管道串联
来源：http://wy.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://zq.521024.cn

[R39] 重定向标准输出与错误
来源：http://ci.asd995.cn

cmd > out.log 2>&1
来源：http://en.yuntaijiaju.cn

[R40] 追加写日志
来源：http://pm.asd995.cn

echo "log" >> out.log
来源：http://jb.shxzukj.cn

[R41] 丢弃输出
来源：http://qf.huixiangedu.cn

cmd >/dev/null 2>&1
来源：http://do.yuntaijiaju.cn

[R42] 输入重定向
来源：http://rf.huixinmuqiang.cn

wc -l < a.txt
来源：http://aq.asd995.cn

[R43] 按名字查找文件
来源：http://fg.9csxet.cn

find . -name "*.log" -type f
来源：http://fy.newstarts.cn

[R44] 按修改时间查找
来源：http://wp.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://nc.jianghongdianzi.cn

[R45] 批量删除
来源：http://sh.shxzskj.cn

find . -name "*.tmp" -delete
来源：http://bo.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://ct.yuntaijiaju.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bg.huixiangedu.cn

[R47] sed 单行替换
来源：http://ok.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uj.hnjuh.cn

[R48] awk 取指定列
来源：http://ya.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://ye.lnxyls.cn

[R49] awk 带条件
来源：http://po.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gy.yuexingan06.cn

[R50] awk 求和
来源：http://ao.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ow.panjiajie.cn

[R51] 排序去重取前几
来源：http://vp.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ak.hnjuh.cn

[R52] 统计行数
来源：http://tr.hnjuh.cn

wc -l a.txt
来源：http://cl.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://mh.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ib.panjiajie.cn

[R54] 比较两个文件
来源：http://dj.hnjuh.cn

diff a.txt b.txt
来源：http://dy.asd995.cn

[R55] 压缩与解压
来源：http://ru.muxihuayi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://es.gzmigu.cn

[R56] 远程拷贝
来源：http://ym.521024.cn

scp file user@host:/path/
来源：http://by.yuexingan06.cn

[R57] 远程执行命令
来源：http://op.szsharing.cn

ssh user@host 'uptime'
来源：http://fx.bookmarksfly.cn

[R58] 下载文件
来源：http://uy.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zb.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://yr.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dp.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://pb.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fo.lnxyls.cn

[R61] 磁盘占用
来源：http://dh.gzmigu.cn

df -h;  du -sh *
来源：http://xs.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://tx.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://wg.shxzskj.cn

[R63] 内存与进程
来源：http://he.colortex.cn

free -h;  ps aux | grep nginx
来源：http://rk.gzmigu.cn

[R64] 结束进程
来源：http://ry.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://jq.newstarts.cn

[R65] 查看端口占用
来源：http://mq.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kt.bjjhwx.cn

[R66] 定时任务
来源：http://lr.szxytkj.cn

crontab -e;  crontab -l
来源：http://vs.nszjky.cn

[R67] 生成随机十六进制串
来源：http://ve.wgjwhj.cn

openssl rand -hex 16
来源：http://ud.panjiajie.cn

[R68] 计算文件校验值
来源：http://pe.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fg.panjiajie.cn

[R69] 生成随机密码
来源：http://aa.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://bn.haigaiapp.cn

[R70] 时间戳与互转
来源：http://tk.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://qn.szxytkj.cn

[R71] 日期格式化
来源：http://vj.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vp.nszjky.cn

[R72] 等待端口就绪
来源：http://ns.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ug.panjiajie.cn

[R73] 分割大日志
来源：http://vf.shtwfgs.cn

split -l 1000 big.log part_
来源：http://rg.nszjky.cn

[R74] 批量重命名
来源：http://ob.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qw.hnjuh.cn

[R75] 导出环境变量
来源：http://yt.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://nt.newstarts.cn

[R76] 使用临时文件
来源：http://hq.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://za.panjiajie.cn

[R77] 读取用户输入
来源：http://pj.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://fj.nszjky.cn

[R78] 交互式菜单
来源：http://cl.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://if.szxytkj.cn

[R79] 解析命令行选项
来源：http://ps.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lv.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://va.shxzskj.cn

time ./run.sh
来源：http://bc.wgjwhj.cn

================================================================================
来源：http://ku.newstarts.cn

S. C / C++ 专题
来源：http://ne.panjiajie.cn

================================================================================
来源：http://db.panjiajie.cn

[S01] C：Hello World
来源：http://cx.nicolike.cn

#include <stdio.h>
来源：http://km.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nw.szsharing.cn

[S02] C：变量与格式化输出
来源：http://jk.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://cj.huixinmuqiang.cn

[S03] C：读入整数
来源：http://wb.szsharing.cn

int x; scanf("%d", &x);
来源：http://cc.shtwfgs.cn

[S04] C：字符串复制
来源：http://ei.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zo.9csxet.cn

[S05] C：字符串长度
来源：http://br.asd995.cn

strlen(s)
来源：http://gj.newstarts.cn

[S06] C：字符串比较
来源：http://bm.shtwfgs.cn

strcmp(a, b) == 0
来源：http://kh.shxzskj.cn

[S07] C：数组遍历求和
来源：http://yk.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pp.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://zi.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xk.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://fq.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vz.521024.cn

[S10] C：指针与解引用
来源：http://dr.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://px.panjiajie.cn

[S11] C：逐行读文件
来源：http://xn.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://kb.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qk.huixiangedu.cn

fclose(f);
来源：http://mn.bjjhwx.cn

[S12] C：写文件
来源：http://pd.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wq.gzmigu.cn

[S13] C：宏定义
来源：http://od.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uu.bjjhwx.cn

[S14] C：枚举
来源：http://bk.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://af.colortex.cn

[S15] C：类型转换
来源：http://qp.bjjhwx.cn

(double) a / b
来源：http://qv.jctech888.com.cn

[S16] C：位操作置位
来源：http://fw.szsharing.cn

x |= (1 << 3);
来源：http://qd.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://ps.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rk.szxytkj.cn

[S18] C：命令行参数
来源：http://jn.wgjwhj.cn

int main(int argc, char **argv)
来源：http://td.szxytkj.cn

[S19] C：快速排序
来源：http://ty.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://im.nicolike.cn

[S20] C：二分查找
来源：http://jy.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://za.panjiajie.cn

[S21] C：字符类别判断
来源：http://uk.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mm.yuexingan06.cn

[S22] C：字符串转数字
来源：http://yw.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://th.panjiajie.cn

[S23] C：随机数
来源：http://sj.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://je.asd995.cn

[S24] C：获取本地时间
来源：http://nv.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cq.szxytkj.cn

[S25] C：内存拷贝
来源：http://km.asd995.cn

memcpy(dst, src, n);
来源：http://oo.wgjwhj.cn

[S26] C：内存清零
来源：http://nr.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://sf.colortex.cn

[S27] C：定义常量
来源：http://dn.shxzskj.cn

const double PI = 3.14159;
来源：http://xs.szsharing.cn

[S28] C：静态变量
来源：http://iv.yuntaijiaju.cn

static int counter = 0;
来源：http://tc.lnxyls.cn

[S29] C：变参函数
来源：http://jb.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ig.nszjky.cn

[S30] C：头文件保护
来源：http://ni.szxytkj.cn

#ifndef X_H
来源：http://nm.bookmarksfly.cn

#define X_H
来源：http://fv.szsharing.cn

#endif
来源：http://ug.hahajie.cn

[S31] C++：Hello World
来源：http://kz.wgjwhj.cn

#include <iostream>
来源：http://xd.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://kh.lnxyls.cn

[S32] C++：字符串
来源：http://ax.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ok.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ls.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aa.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://or.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://xo.521024.cn


<!-- 参考信息 -->