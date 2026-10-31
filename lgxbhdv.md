代发 wailian999

[Q63] 开启事务
来源：http://au.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jd.yuexingan06.cn

[Q64] 提交事务
来源：http://al.colortex.cn

COMMIT;
来源：http://sx.lnxyls.cn

[Q65] 回滚事务
来源：http://ka.521024.cn

ROLLBACK;
来源：http://fn.nszjky.cn

[Q66] 行锁查询
来源：http://lm.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://it.huixiangedu.cn

[Q67] 设置隔离级别
来源：http://pc.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eu.9csxet.cn

[Q68] 保存点
来源：http://bo.hahajie.cn

SAVEPOINT sp1;
来源：http://bg.lnxyls.cn

ROLLBACK TO sp1;
来源：http://gw.colortex.cn

[Q69] 查看执行计划
来源：http://kg.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ft.nszjky.cn

[Q70] 更新统计信息
来源：http://ar.hahajie.cn

ANALYZE TABLE users;
来源：http://jb.shxzukj.cn

[Q71] 查看建表语句
来源：http://um.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ux.nicolike.cn

[Q72] 查看索引
来源：http://ll.gzmigu.cn

SHOW INDEX FROM users;
来源：http://fz.haigaiapp.cn

[Q73] 查看表状态
来源：http://ju.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wo.wgjwhj.cn

[Q74] 强制使用索引
来源：http://na.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gh.chemitech.net.cn

[Q75] 日期格式化
来源：http://kc.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gb.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hu.yuntaijiaju.cn

[Q76] 按天统计
来源：http://sv.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pt.lnxyls.cn

[Q77] 时间加减
来源：http://tk.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ea.szxytkj.cn

[Q78] 当前时间
来源：http://rn.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lj.szsharing.cn

[Q79] 字符串拼接
来源：http://ze.szxytkj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dz.muxihuayi.cn

[Q80] 字符串截取
来源：http://jf.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jl.lnxyls.cn

[Q81] 字符串替换
来源：http://sn.bookmarksfly.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mc.colortex.cn

[Q82] 字符长度与字节长度
来源：http://rp.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xv.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://qs.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://si.jctech888.com.cn

[Q84] 去除首尾空格
来源：http://pj.lnxyls.cn

SELECT TRIM(name) FROM users;
来源：http://re.lnxyls.cn

[Q85] 数值取整
来源：http://md.wgjwhj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yo.asd995.cn

[Q86] 读取 JSON 字段
来源：http://mz.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qd.szsharing.cn

[Q87] JSON 字段做条件
来源：http://rg.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pn.shxzskj.cn

[Q88] 行转列（条件聚合）
来源：http://ga.hnjuh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ka.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ds.szxytkj.cn

[Q89] 判断表是否存在
来源：http://py.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yy.haigaiapp.cn

[Q90] 生成序号列
来源：http://bp.nicolike.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jl.wgjwhj.cn

================================================================================
来源：http://lj.shtwfgs.cn

R. Bash 专题
来源：http://jj.lnxyls.cn

================================================================================
来源：http://jd.wgjwhj.cn

[R01] shebang 与严格模式
来源：http://os.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://pk.colortex.cn

set -euo pipefail
来源：http://vr.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://wx.nicolike.cn

name="Tom"; echo "$name"
来源：http://rr.hahajie.cn

[R03] 只读变量
来源：http://rg.hnjuh.cn

readonly PI=3.14
来源：http://et.shxzukj.cn

[R04] 位置参数
来源：http://sa.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ir.nicolike.cn

[R05] 参数默认值
来源：http://ug.bookmarksfly.cn

name="${1:-default}"
来源：http://mi.lnxyls.cn

[R06] 判断命令是否存在
来源：http://ey.chemitech.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rg.9csxet.cn

[R07] if 判断文件
来源：http://br.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yu.hahajie.cn

[R08] 数值比较
来源：http://vc.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zw.shxzskj.cn

[R09] 字符串比较
来源：http://py.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fc.chemitech.net.cn

[R10] 正则匹配
来源：http://qc.bjjhwx.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wh.shtwfgs.cn

[R11] case 多分支
来源：http://ck.asd995.cn

case "$1" in
来源：http://dm.521024.cn

start) echo "启动" ;;
来源：http://vs.asd995.cn

stop)  echo "停止" ;;
来源：http://ys.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://lk.szxytkj.cn

esac
来源：http://oz.newstarts.cn

[R12] for 遍历文件
来源：http://uy.colortex.cn

for f in *.txt; do echo "$f"; done
来源：http://kn.gzmigu.cn

[R13] for 计数循环
来源：http://vv.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://tp.szsharing.cn

[R14] C 风格 for
来源：http://vx.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yf.9csxet.cn

[R15] while 逐行读文件
来源：http://yd.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jq.newstarts.cn

[R16] until 等待条件
来源：http://ob.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fr.muxihuayi.cn

[R17] 数组定义与取值
来源：http://ny.chemitech.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qa.lnxyls.cn

[R18] 遍历数组
来源：http://qu.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mc.521024.cn

[R19] 数组长度
来源：http://ti.lnxyls.cn

echo "${#arr[@]}"
来源：http://hv.szsharing.cn

[R20] 关联数组（字典）
来源：http://iu.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.szsharing.cn

[R21] 字符串长度
来源：http://vt.colortex.cn

echo "${#s}"
来源：http://bg.hahajie.cn

[R22] 截取子串
来源：http://ng.huixinmuqiang.cn

echo "${s:0:5}"
来源：http://dl.chemitech.net.cn

[R23] 字符串替换
来源：http://te.shtwfgs.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ra.muxihuayi.cn

[R24] 大小写转换
来源：http://it.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tn.szxytkj.cn

[R25] 去后缀 / 去前缀
来源：http://bz.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hx.szxytkj.cn

[R26] 命令替换
来源：http://bm.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://rc.gzmigu.cn

[R27] 算术展开
来源：http://xz.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://qj.bjjhwx.cn

[R28] 浮点运算
来源：http://qq.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://gg.bookmarksfly.cn

[R29] 定义函数
来源：http://ux.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cz.hahajie.cn

[R30] 函数返回状态码
来源：http://my.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://bx.muxihuayi.cn

[R31] 局部变量
来源：http://md.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://ug.nicolike.cn

[R32] 参数个数校验
来源：http://vu.asd995.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mu.huanxung.cn

[R33] 捕获错误并提示行号
来源：http://fq.hnjuh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hs.lnxyls.cn

[R34] 退出时清理
来源：http://dm.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zp.szsharing.cn

[R35] 后台执行并等待
来源：http://pr.yuexingan06.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sw.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://pn.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xg.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://pb.nicolike.cn

files=$(ls -1)
来源：http://hs.shxzukj.cn

[R38] 管道串联
来源：http://rf.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://iq.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://vy.bjjhwx.cn

cmd > out.log 2>&1
来源：http://xu.nszjky.cn

[R40] 追加写日志
来源：http://oj.haigaiapp.cn

echo "log" >> out.log
来源：http://yt.haigaiapp.cn

[R41] 丢弃输出
来源：http://rb.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://vf.lnxyls.cn

[R42] 输入重定向
来源：http://dr.jianghongdianzi.cn

wc -l < a.txt
来源：http://ck.huixiangedu.cn

[R43] 按名字查找文件
来源：http://sw.lnxyls.cn

find . -name "*.log" -type f
来源：http://fn.asd995.cn

[R44] 按修改时间查找
来源：http://cs.panjiajie.cn

find . -mtime -7 -type f
来源：http://vw.bookmarksfly.cn

[R45] 批量删除
来源：http://fv.szxytkj.cn

find . -name "*.tmp" -delete
来源：http://ii.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://ch.wgjwhj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kz.hahajie.cn

[R47] sed 单行替换
来源：http://oe.huixiangedu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rw.asd995.cn

[R48] awk 取指定列
来源：http://pn.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://tu.lnxyls.cn

[R49] awk 带条件
来源：http://ix.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ma.shxzskj.cn

[R50] awk 求和
来源：http://tw.huanxung.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pc.hahajie.cn

[R51] 排序去重取前几
来源：http://mx.jianghongdianzi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oz.huixiangedu.cn

[R52] 统计行数
来源：http://qt.wgjwhj.cn

wc -l a.txt
来源：http://ed.nszjky.cn

[R53] 查看文件头与实时尾
来源：http://mg.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zw.shxzskj.cn

[R54] 比较两个文件
来源：http://qq.yuexingan06.cn

diff a.txt b.txt
来源：http://zn.hnjuh.cn

[R55] 压缩与解压
来源：http://xf.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ot.521024.cn

[R56] 远程拷贝
来源：http://mb.jctech888.com.cn

scp file user@host:/path/
来源：http://ou.yuexingan06.cn

[R57] 远程执行命令
来源：http://pr.521024.cn

ssh user@host 'uptime'
来源：http://ew.huanxung.cn

[R58] 下载文件
来源：http://pm.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xm.bjjhwx.cn

[R59] 发 POST JSON
来源：http://ac.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vl.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://ze.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mb.bookmarksfly.cn

[R61] 磁盘占用
来源：http://gr.szxytkj.cn

df -h;  du -sh *
来源：http://ye.nicolike.cn

[R62] 找最占空间的文件
来源：http://de.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://gi.bookmarksfly.cn

[R63] 内存与进程
来源：http://ji.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://ug.szxytkj.cn

[R64] 结束进程
来源：http://nf.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://gb.shtwfgs.cn

[R65] 查看端口占用
来源：http://xj.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pp.szxytkj.cn

[R66] 定时任务
来源：http://yv.chemitech.net.cn

crontab -e;  crontab -l
来源：http://yv.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://gi.yuexingan06.cn

openssl rand -hex 16
来源：http://ym.huixiangedu.cn

[R68] 计算文件校验值
来源：http://ds.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ny.shtwfgs.cn

[R69] 生成随机密码
来源：http://df.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://im.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://my.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://xk.panjiajie.cn

[R71] 日期格式化
来源：http://ds.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lt.newstarts.cn

[R72] 等待端口就绪
来源：http://bw.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kz.shxzukj.cn

[R73] 分割大日志
来源：http://fp.wgjwhj.cn

split -l 1000 big.log part_
来源：http://pp.hnjuh.cn

[R74] 批量重命名
来源：http://jz.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uq.bookmarksfly.cn

[R75] 导出环境变量
来源：http://au.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://rk.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ib.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lv.521024.cn

[R77] 读取用户输入
来源：http://el.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://rw.muxihuayi.cn

[R78] 交互式菜单
来源：http://sy.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zt.bjjhwx.cn

[R79] 解析命令行选项
来源：http://es.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ad.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://bp.hnjuh.cn

time ./run.sh
来源：http://ce.huixinmuqiang.cn

================================================================================
来源：http://ax.bjjhwx.cn

S. C / C++ 专题
来源：http://df.szsharing.cn

================================================================================
来源：http://kt.hnjuh.cn

[S01] C：Hello World
来源：http://kz.hnjuh.cn

#include <stdio.h>
来源：http://sl.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yp.newstarts.cn

[S02] C：变量与格式化输出
来源：http://oh.521024.cn

int a = 10; printf("%d\n", a);
来源：http://mr.lnxyls.cn

[S03] C：读入整数
来源：http://uu.nszjky.cn

int x; scanf("%d", &x);
来源：http://cp.shxzskj.cn

[S04] C：字符串复制
来源：http://pd.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ev.shtwfgs.cn

[S05] C：字符串长度
来源：http://yc.bjjhwx.cn

strlen(s)
来源：http://uz.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://rm.yuexingan06.cn

strcmp(a, b) == 0
来源：http://cz.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://ky.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lw.521024.cn

[S08] C：动态内存分配与释放
来源：http://qy.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://li.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ma.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uv.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://vs.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://lz.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ov.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://wg.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gt.hnjuh.cn

fclose(f);
来源：http://rh.9csxet.cn

[S12] C：写文件
来源：http://va.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fs.shxzukj.cn

[S13] C：宏定义
来源：http://nw.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zo.huanxung.cn

[S14] C：枚举
来源：http://lm.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://dn.panjiajie.cn

[S15] C：类型转换
来源：http://tf.jianghongdianzi.cn

(double) a / b
来源：http://du.szsharing.cn

[S16] C：位操作置位
来源：http://op.huanxung.cn

x |= (1 << 3);
来源：http://yk.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://se.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tz.jctech888.com.cn

[S18] C：命令行参数
来源：http://ar.521024.cn

int main(int argc, char **argv)
来源：http://yh.hahajie.cn

[S19] C：快速排序
来源：http://lh.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dh.bookmarksfly.cn

[S20] C：二分查找
来源：http://rq.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sa.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://js.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sb.gzmigu.cn

[S22] C：字符串转数字
来源：http://dg.huixinmuqiang.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eh.nicolike.cn

[S23] C：随机数
来源：http://gv.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ic.yuexingan06.cn

[S24] C：获取本地时间
来源：http://ff.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://li.asd995.cn

[S25] C：内存拷贝
来源：http://dg.shtwfgs.cn

memcpy(dst, src, n);
来源：http://ij.521024.cn

[S26] C：内存清零
来源：http://ex.nszjky.cn

memset(a, 0, sizeof a);
来源：http://xk.lnxyls.cn

[S27] C：定义常量
来源：http://jm.bookmarksfly.cn

const double PI = 3.14159;
来源：http://st.hnjuh.cn

[S28] C：静态变量
来源：http://bo.haigaiapp.cn

static int counter = 0;
来源：http://cx.panjiajie.cn

[S29] C：变参函数
来源：http://dg.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zw.wgjwhj.cn

[S30] C：头文件保护
来源：http://lz.bjjhwx.cn

#ifndef X_H
来源：http://hd.asd995.cn

#define X_H
来源：http://id.huixiangedu.cn

#endif
来源：http://zt.521024.cn

[S31] C++：Hello World
来源：http://ib.521024.cn

#include <iostream>
来源：http://la.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ir.jctech888.com.cn

[S32] C++：字符串
来源：http://ms.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://vw.nszjky.cn


<!-- 参考信息 -->