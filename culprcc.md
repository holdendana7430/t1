代发 wailian999

[Q61] 移动平均
来源：http://kw.panjiajie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ox.newstarts.cn

[Q62] 分组占比
来源：http://js.gzmigu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wg.shxzskj.cn

[Q63] 开启事务
来源：http://hb.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oa.szsharing.cn

[Q64] 提交事务
来源：http://bu.shxzskj.cn

COMMIT;
来源：http://kf.huanxung.cn

[Q65] 回滚事务
来源：http://sx.shxzukj.cn

ROLLBACK;
来源：http://dl.hnjuh.cn

[Q66] 行锁查询
来源：http://nr.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ll.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://sz.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lr.gzmigu.cn

[Q68] 保存点
来源：http://sp.shxzukj.cn

SAVEPOINT sp1;
来源：http://ls.shtwfgs.cn

ROLLBACK TO sp1;
来源：http://my.huanxung.cn

[Q69] 查看执行计划
来源：http://ko.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xd.asd995.cn

[Q70] 更新统计信息
来源：http://jt.haigaiapp.cn

ANALYZE TABLE users;
来源：http://yx.gzmigu.cn

[Q71] 查看建表语句
来源：http://rh.shxzskj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hl.bookmarksfly.cn

[Q72] 查看索引
来源：http://kp.muxihuayi.cn

SHOW INDEX FROM users;
来源：http://ih.shxzukj.cn

[Q73] 查看表状态
来源：http://vk.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://om.lnxyls.cn

[Q74] 强制使用索引
来源：http://qd.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qf.nszjky.cn

[Q75] 日期格式化
来源：http://cs.yuexingan06.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jc.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fj.chemitech.net.cn

[Q76] 按天统计
来源：http://sz.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ai.nicolike.cn

[Q77] 时间加减
来源：http://hw.panjiajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xg.chemitech.net.cn

[Q78] 当前时间
来源：http://sa.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://op.521024.cn

[Q79] 字符串拼接
来源：http://ye.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wo.newstarts.cn

[Q80] 字符串截取
来源：http://xc.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://er.nicolike.cn

[Q81] 字符串替换
来源：http://ls.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fi.asd995.cn

[Q82] 字符长度与字节长度
来源：http://kl.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rp.panjiajie.cn

[Q83] 大小写转换
来源：http://dg.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kw.asd995.cn

[Q84] 去除首尾空格
来源：http://tx.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://xj.szsharing.cn

[Q85] 数值取整
来源：http://if.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ha.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://cs.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://la.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://xs.wgjwhj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ld.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://hm.bookmarksfly.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://an.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ge.asd995.cn

[Q89] 判断表是否存在
来源：http://ob.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gw.szxytkj.cn

[Q90] 生成序号列
来源：http://aw.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vf.huanxung.cn

================================================================================
来源：http://xh.muxihuayi.cn

R. Bash 专题
来源：http://kr.szsharing.cn

================================================================================
来源：http://lh.panjiajie.cn

[R01] shebang 与严格模式
来源：http://sj.szsharing.cn

#!/usr/bin/env bash
来源：http://wa.shtwfgs.cn

set -euo pipefail
来源：http://zx.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://qc.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://ah.haigaiapp.cn

[R03] 只读变量
来源：http://cm.chemitech.net.cn

readonly PI=3.14
来源：http://uy.huanxung.cn

[R04] 位置参数
来源：http://ej.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://li.huixinmuqiang.cn

[R05] 参数默认值
来源：http://nv.panjiajie.cn

name="${1:-default}"
来源：http://ng.szxytkj.cn

[R06] 判断命令是否存在
来源：http://fq.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://go.hnjuh.cn

[R07] if 判断文件
来源：http://da.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ve.shxzskj.cn

[R08] 数值比较
来源：http://ew.nicolike.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bs.lnxyls.cn

[R09] 字符串比较
来源：http://ko.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eg.yuntaijiaju.cn

[R10] 正则匹配
来源：http://mp.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ne.bjjhwx.cn

[R11] case 多分支
来源：http://dm.wgjwhj.cn

case "$1" in
来源：http://pk.gzmigu.cn

start) echo "启动" ;;
来源：http://vg.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://xj.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://nt.521024.cn

esac
来源：http://ez.huanxung.cn

[R12] for 遍历文件
来源：http://cc.nszjky.cn

for f in *.txt; do echo "$f"; done
来源：http://jq.9csxet.cn

[R13] for 计数循环
来源：http://wx.521024.cn

for i in {1..10}; do echo "$i"; done
来源：http://up.yuntaijiaju.cn

[R14] C 风格 for
来源：http://vs.colortex.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ms.9csxet.cn

[R15] while 逐行读文件
来源：http://fe.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aw.wgjwhj.cn

[R16] until 等待条件
来源：http://zc.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mm.muxihuayi.cn

[R17] 数组定义与取值
来源：http://rh.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vp.shxzukj.cn

[R18] 遍历数组
来源：http://ma.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nl.szxytkj.cn

[R19] 数组长度
来源：http://td.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://sa.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://ny.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ou.chemitech.net.cn

[R21] 字符串长度
来源：http://cg.bookmarksfly.cn

echo "${#s}"
来源：http://hx.nszjky.cn

[R22] 截取子串
来源：http://tt.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://qy.huixinmuqiang.cn

[R23] 字符串替换
来源：http://sp.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ws.muxihuayi.cn

[R24] 大小写转换
来源：http://oe.hnjuh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wn.huanxung.cn

[R25] 去后缀 / 去前缀
来源：http://wl.yuntaijiaju.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fg.huixiangedu.cn

[R26] 命令替换
来源：http://se.colortex.cn

now=$(date +%F); echo "$now"
来源：http://ob.gzmigu.cn

[R27] 算术展开
来源：http://ar.newstarts.cn

echo $((1 + 2 * 3))
来源：http://nf.gzmigu.cn

[R28] 浮点运算
来源：http://th.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://kp.panjiajie.cn

[R29] 定义函数
来源：http://br.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ho.haigaiapp.cn

[R30] 函数返回状态码
来源：http://rw.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ky.jctech888.com.cn

[R31] 局部变量
来源：http://ya.yuexingan06.cn

f() { local x=1; echo "$x"; }
来源：http://tp.shxzukj.cn

[R32] 参数个数校验
来源：http://dc.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rt.newstarts.cn

[R33] 捕获错误并提示行号
来源：http://wq.yuexingan06.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://es.lnxyls.cn

[R34] 退出时清理
来源：http://tt.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eu.521024.cn

[R35] 后台执行并等待
来源：http://uz.gzmigu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dd.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://ts.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://og.nszjky.cn

[R37] 把输出赋给变量
来源：http://ox.wgjwhj.cn

files=$(ls -1)
来源：http://ij.yuntaijiaju.cn

[R38] 管道串联
来源：http://no.szxytkj.cn

cat a.txt | grep -i error | wc -l
来源：http://ia.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://ja.gzmigu.cn

cmd > out.log 2>&1
来源：http://do.9csxet.cn

[R40] 追加写日志
来源：http://ef.bookmarksfly.cn

echo "log" >> out.log
来源：http://zn.haigaiapp.cn

[R41] 丢弃输出
来源：http://oz.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://wk.gzmigu.cn

[R42] 输入重定向
来源：http://qt.9csxet.cn

wc -l < a.txt
来源：http://on.asd995.cn

[R43] 按名字查找文件
来源：http://oo.haigaiapp.cn

find . -name "*.log" -type f
来源：http://it.hnjuh.cn

[R44] 按修改时间查找
来源：http://qp.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://cu.gzmigu.cn

[R45] 批量删除
来源：http://lv.colortex.cn

find . -name "*.tmp" -delete
来源：http://ft.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://dv.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qx.bjjhwx.cn

[R47] sed 单行替换
来源：http://zl.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gv.colortex.cn

[R48] awk 取指定列
来源：http://ze.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://xs.haigaiapp.cn

[R49] awk 带条件
来源：http://is.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ha.newstarts.cn

[R50] awk 求和
来源：http://li.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kc.muxihuayi.cn

[R51] 排序去重取前几
来源：http://nu.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ih.chemitech.net.cn

[R52] 统计行数
来源：http://de.szsharing.cn

wc -l a.txt
来源：http://ww.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://lq.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qh.newstarts.cn

[R54] 比较两个文件
来源：http://nv.bookmarksfly.cn

diff a.txt b.txt
来源：http://xy.9csxet.cn

[R55] 压缩与解压
来源：http://id.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cq.hnjuh.cn

[R56] 远程拷贝
来源：http://gi.521024.cn

scp file user@host:/path/
来源：http://wz.szsharing.cn

[R57] 远程执行命令
来源：http://td.jctech888.com.cn

ssh user@host 'uptime'
来源：http://uh.colortex.cn

[R58] 下载文件
来源：http://aa.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bb.gzmigu.cn

[R59] 发 POST JSON
来源：http://vg.yuntaijiaju.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wh.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://qh.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hb.bookmarksfly.cn

[R61] 磁盘占用
来源：http://xk.shxzskj.cn

df -h;  du -sh *
来源：http://rj.shxzskj.cn

[R62] 找最占空间的文件
来源：http://al.521024.cn

du -ah . | sort -rh | head -10
来源：http://vu.yuntaijiaju.cn

[R63] 内存与进程
来源：http://qa.yuexingan06.cn

free -h;  ps aux | grep nginx
来源：http://wz.yuntaijiaju.cn

[R64] 结束进程
来源：http://cw.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://wz.521024.cn

[R65] 查看端口占用
来源：http://kq.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ai.9csxet.cn

[R66] 定时任务
来源：http://vz.haigaiapp.cn

crontab -e;  crontab -l
来源：http://ri.huanxung.cn

[R67] 生成随机十六进制串
来源：http://sg.colortex.cn

openssl rand -hex 16
来源：http://xz.huixiangedu.cn

[R68] 计算文件校验值
来源：http://wp.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xj.hahajie.cn

[R69] 生成随机密码
来源：http://qb.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://gq.shtwfgs.cn

[R70] 时间戳与互转
来源：http://vb.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://sm.bookmarksfly.cn

[R71] 日期格式化
来源：http://lu.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sz.gzmigu.cn

[R72] 等待端口就绪
来源：http://if.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fa.wgjwhj.cn

[R73] 分割大日志
来源：http://qd.colortex.cn

split -l 1000 big.log part_
来源：http://xz.hahajie.cn

[R74] 批量重命名
来源：http://tb.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://go.bjjhwx.cn

[R75] 导出环境变量
来源：http://al.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ws.shtwfgs.cn

[R76] 使用临时文件
来源：http://cp.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xi.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://eu.gzmigu.cn

read -rp "请输入: " ans
来源：http://zc.jctech888.com.cn

[R78] 交互式菜单
来源：http://mv.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kp.bjjhwx.cn

[R79] 解析命令行选项
来源：http://dl.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mc.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://cz.shxzskj.cn

time ./run.sh
来源：http://fn.hahajie.cn

================================================================================
来源：http://sa.newstarts.cn

S. C / C++ 专题
来源：http://fc.lnxyls.cn

================================================================================
来源：http://aw.521024.cn

[S01] C：Hello World
来源：http://ne.nicolike.cn

#include <stdio.h>
来源：http://kg.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jy.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://up.bookmarksfly.cn

int a = 10; printf("%d\n", a);
来源：http://vs.chemitech.net.cn

[S03] C：读入整数
来源：http://oo.lnxyls.cn

int x; scanf("%d", &x);
来源：http://uh.szsharing.cn

[S04] C：字符串复制
来源：http://zo.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://my.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://zu.yuexingan06.cn

strlen(s)
来源：http://lv.wgjwhj.cn

[S06] C：字符串比较
来源：http://it.shxzukj.cn

strcmp(a, b) == 0
来源：http://cm.nszjky.cn

[S07] C：数组遍历求和
来源：http://ok.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zu.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://pa.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ou.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://xv.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ol.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://pf.nszjky.cn

int *p = &a;  *p = 5;
来源：http://xm.chemitech.net.cn

[S11] C：逐行读文件
来源：http://wb.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ce.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xz.muxihuayi.cn

fclose(f);
来源：http://qj.asd995.cn

[S12] C：写文件
来源：http://jt.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://so.521024.cn

[S13] C：宏定义
来源：http://pp.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jx.asd995.cn

[S14] C：枚举
来源：http://nb.panjiajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://rr.szsharing.cn

[S15] C：类型转换
来源：http://ji.nicolike.cn

(double) a / b
来源：http://vz.nszjky.cn

[S16] C：位操作置位
来源：http://cz.huixiangedu.cn

x |= (1 << 3);
来源：http://cd.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://nu.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rr.nszjky.cn

[S18] C：命令行参数
来源：http://xu.huixiangedu.cn

int main(int argc, char **argv)
来源：http://qu.huixiangedu.cn

[S19] C：快速排序
来源：http://it.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ft.huixinmuqiang.cn

[S20] C：二分查找
来源：http://fq.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fy.shxzukj.cn

[S21] C：字符类别判断
来源：http://ha.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dt.nicolike.cn

[S22] C：字符串转数字
来源：http://hn.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iz.9csxet.cn

[S23] C：随机数
来源：http://yv.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xs.szsharing.cn

[S24] C：获取本地时间
来源：http://lw.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wx.panjiajie.cn

[S25] C：内存拷贝
来源：http://bq.muxihuayi.cn

memcpy(dst, src, n);
来源：http://ck.asd995.cn

[S26] C：内存清零
来源：http://lv.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://cp.shxzukj.cn

[S27] C：定义常量
来源：http://sw.yuexingan06.cn

const double PI = 3.14159;
来源：http://cg.jctech888.com.cn

[S28] C：静态变量
来源：http://jj.9csxet.cn

static int counter = 0;
来源：http://xp.gzmigu.cn

[S29] C：变参函数
来源：http://qz.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pq.shxzukj.cn

[S30] C：头文件保护
来源：http://yc.colortex.cn

#ifndef X_H
来源：http://lw.wgjwhj.cn

#define X_H
来源：http://yj.lnxyls.cn

#endif
来源：http://jo.nicolike.cn

[S31] C++：Hello World
来源：http://se.nszjky.cn


<!-- 参考信息 -->