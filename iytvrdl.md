代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://az.521024.cn

[Q60] 取上一行 / 下一行
来源：http://vw.colortex.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dm.colortex.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wn.wgjwhj.cn

[Q61] 移动平均
来源：http://ir.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hb.szxytkj.cn

[Q62] 分组占比
来源：http://he.newstarts.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wl.jctech888.com.cn

[Q63] 开启事务
来源：http://bb.szsharing.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wh.shxzukj.cn

[Q64] 提交事务
来源：http://ex.gzmigu.cn

COMMIT;
来源：http://dc.gzmigu.cn

[Q65] 回滚事务
来源：http://gf.shxzukj.cn

ROLLBACK;
来源：http://uf.colortex.cn

[Q66] 行锁查询
来源：http://to.bjjhwx.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wy.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://cl.szxytkj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kn.9csxet.cn

[Q68] 保存点
来源：http://hw.521024.cn

SAVEPOINT sp1;
来源：http://af.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://oz.huanxung.cn

[Q69] 查看执行计划
来源：http://ss.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pn.yuexingan06.cn

[Q70] 更新统计信息
来源：http://zu.chemitech.net.cn

ANALYZE TABLE users;
来源：http://wb.panjiajie.cn

[Q71] 查看建表语句
来源：http://ne.huixiangedu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gy.chemitech.net.cn

[Q72] 查看索引
来源：http://ud.nicolike.cn

SHOW INDEX FROM users;
来源：http://en.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://cr.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dx.wgjwhj.cn

[Q74] 强制使用索引
来源：http://xh.jctech888.com.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://md.asd995.cn

[Q75] 日期格式化
来源：http://os.muxihuayi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://li.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ba.huixinmuqiang.cn

[Q76] 按天统计
来源：http://pw.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sq.huixinmuqiang.cn

[Q77] 时间加减
来源：http://di.asd995.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sv.colortex.cn

[Q78] 当前时间
来源：http://jg.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://im.bookmarksfly.cn

[Q79] 字符串拼接
来源：http://hj.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vc.newstarts.cn

[Q80] 字符串截取
来源：http://of.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fc.9csxet.cn

[Q81] 字符串替换
来源：http://rh.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cj.nicolike.cn

[Q82] 字符长度与字节长度
来源：http://wx.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qn.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://zm.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xx.9csxet.cn

[Q84] 去除首尾空格
来源：http://ba.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://gr.huixinmuqiang.cn

[Q85] 数值取整
来源：http://ph.9csxet.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fh.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://gp.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wh.newstarts.cn

[Q87] JSON 字段做条件
来源：http://ha.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jh.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://kj.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ni.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wj.lnxyls.cn

[Q89] 判断表是否存在
来源：http://qt.shxzukj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ya.jctech888.com.cn

[Q90] 生成序号列
来源：http://tc.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sp.yuntaijiaju.cn

================================================================================
来源：http://eb.shxzskj.cn

R. Bash 专题
来源：http://ho.szxytkj.cn

================================================================================
来源：http://dd.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://zj.huixinmuqiang.cn

#!/usr/bin/env bash
来源：http://kp.chemitech.net.cn

set -euo pipefail
来源：http://ct.shxzskj.cn

[R02] 变量赋值与使用
来源：http://lf.huanxung.cn

name="Tom"; echo "$name"
来源：http://gh.yuntaijiaju.cn

[R03] 只读变量
来源：http://jh.huixiangedu.cn

readonly PI=3.14
来源：http://ac.hnjuh.cn

[R04] 位置参数
来源：http://ff.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xb.szxytkj.cn

[R05] 参数默认值
来源：http://ec.lnxyls.cn

name="${1:-default}"
来源：http://wk.hnjuh.cn

[R06] 判断命令是否存在
来源：http://lz.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qm.nicolike.cn

[R07] if 判断文件
来源：http://sf.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qa.muxihuayi.cn

[R08] 数值比较
来源：http://sp.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dd.szsharing.cn

[R09] 字符串比较
来源：http://hi.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vf.colortex.cn

[R10] 正则匹配
来源：http://he.yuexingan06.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xr.jianghongdianzi.cn

[R11] case 多分支
来源：http://el.521024.cn

case "$1" in
来源：http://po.jctech888.com.cn

start) echo "启动" ;;
来源：http://on.gzmigu.cn

stop)  echo "停止" ;;
来源：http://up.yuexingan06.cn

*)     echo "未知命令" ;;
来源：http://dk.colortex.cn

esac
来源：http://nv.lnxyls.cn

[R12] for 遍历文件
来源：http://mc.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://zo.jianghongdianzi.cn

[R13] for 计数循环
来源：http://hk.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://xp.newstarts.cn

[R14] C 风格 for
来源：http://gp.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hu.gzmigu.cn

[R15] while 逐行读文件
来源：http://eo.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ic.haigaiapp.cn

[R16] until 等待条件
来源：http://mi.newstarts.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rr.shxzskj.cn

[R17] 数组定义与取值
来源：http://zr.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qx.521024.cn

[R18] 遍历数组
来源：http://eq.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://co.colortex.cn

[R19] 数组长度
来源：http://ou.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://vs.nicolike.cn

[R20] 关联数组（字典）
来源：http://dp.hnjuh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sk.colortex.cn

[R21] 字符串长度
来源：http://cq.shtwfgs.cn

echo "${#s}"
来源：http://yk.shxzukj.cn

[R22] 截取子串
来源：http://xf.gzmigu.cn

echo "${s:0:5}"
来源：http://pf.shxzskj.cn

[R23] 字符串替换
来源：http://qj.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lu.bookmarksfly.cn

[R24] 大小写转换
来源：http://vi.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kl.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://eb.hahajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jj.yuexingan06.cn

[R26] 命令替换
来源：http://zk.nicolike.cn

now=$(date +%F); echo "$now"
来源：http://dj.panjiajie.cn

[R27] 算术展开
来源：http://pt.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://zi.shxzskj.cn

[R28] 浮点运算
来源：http://bd.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://qi.hnjuh.cn

[R29] 定义函数
来源：http://sl.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qz.521024.cn

[R30] 函数返回状态码
来源：http://cs.jianghongdianzi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vx.szsharing.cn

[R31] 局部变量
来源：http://mp.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://kl.szxytkj.cn

[R32] 参数个数校验
来源：http://nw.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://et.shxzukj.cn

[R33] 捕获错误并提示行号
来源：http://ou.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lr.asd995.cn

[R34] 退出时清理
来源：http://at.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bc.huixiangedu.cn

[R35] 后台执行并等待
来源：http://gc.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ju.yuntaijiaju.cn

[R36] 并发执行多个任务
来源：http://qd.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yl.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://yw.lnxyls.cn

files=$(ls -1)
来源：http://lb.gzmigu.cn

[R38] 管道串联
来源：http://fu.lnxyls.cn

cat a.txt | grep -i error | wc -l
来源：http://ep.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://qf.shxzukj.cn

cmd > out.log 2>&1
来源：http://gu.asd995.cn

[R40] 追加写日志
来源：http://qk.huixinmuqiang.cn

echo "log" >> out.log
来源：http://tg.gzmigu.cn

[R41] 丢弃输出
来源：http://lj.newstarts.cn

cmd >/dev/null 2>&1
来源：http://li.szsharing.cn

[R42] 输入重定向
来源：http://mj.szxytkj.cn

wc -l < a.txt
来源：http://xa.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://iw.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://if.lnxyls.cn

[R44] 按修改时间查找
来源：http://cr.muxihuayi.cn

find . -mtime -7 -type f
来源：http://yz.newstarts.cn

[R45] 批量删除
来源：http://tj.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://od.9csxet.cn

[R46] 递归替换文件内容
来源：http://im.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rj.szxytkj.cn

[R47] sed 单行替换
来源：http://vt.newstarts.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tt.9csxet.cn

[R48] awk 取指定列
来源：http://gx.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://fc.huanxung.cn

[R49] awk 带条件
来源：http://xx.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zb.haigaiapp.cn

[R50] awk 求和
来源：http://im.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ns.hnjuh.cn

[R51] 排序去重取前几
来源：http://pq.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://op.wgjwhj.cn

[R52] 统计行数
来源：http://zf.bjjhwx.cn

wc -l a.txt
来源：http://zl.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://hg.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cm.muxihuayi.cn

[R54] 比较两个文件
来源：http://hm.9csxet.cn

diff a.txt b.txt
来源：http://gt.asd995.cn

[R55] 压缩与解压
来源：http://wc.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qy.muxihuayi.cn

[R56] 远程拷贝
来源：http://rc.jctech888.com.cn

scp file user@host:/path/
来源：http://hm.newstarts.cn

[R57] 远程执行命令
来源：http://vs.521024.cn

ssh user@host 'uptime'
来源：http://dd.hahajie.cn

[R58] 下载文件
来源：http://cz.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zt.wgjwhj.cn

[R59] 发 POST JSON
来源：http://tc.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://py.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://fy.chemitech.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vj.huixiangedu.cn

[R61] 磁盘占用
来源：http://vl.szsharing.cn

df -h;  du -sh *
来源：http://cq.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://bn.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ri.szsharing.cn

[R63] 内存与进程
来源：http://nu.newstarts.cn

free -h;  ps aux | grep nginx
来源：http://dx.wgjwhj.cn

[R64] 结束进程
来源：http://pq.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://px.bookmarksfly.cn

[R65] 查看端口占用
来源：http://yn.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rd.asd995.cn

[R66] 定时任务
来源：http://jr.huixiangedu.cn

crontab -e;  crontab -l
来源：http://ri.521024.cn

[R67] 生成随机十六进制串
来源：http://an.shxzukj.cn

openssl rand -hex 16
来源：http://ul.lnxyls.cn

[R68] 计算文件校验值
来源：http://rz.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xl.yuexingan06.cn

[R69] 生成随机密码
来源：http://ny.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://qm.yuexingan06.cn

[R70] 时间戳与互转
来源：http://mn.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://aw.huixiangedu.cn

[R71] 日期格式化
来源：http://fd.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aw.haigaiapp.cn

[R72] 等待端口就绪
来源：http://tc.huixinmuqiang.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zc.shxzskj.cn

[R73] 分割大日志
来源：http://ve.asd995.cn

split -l 1000 big.log part_
来源：http://jg.muxihuayi.cn

[R74] 批量重命名
来源：http://bz.shxzukj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sd.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://av.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://nx.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://yo.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hw.shtwfgs.cn

[R77] 读取用户输入
来源：http://io.asd995.cn

read -rp "请输入: " ans
来源：http://vr.lnxyls.cn

[R78] 交互式菜单
来源：http://wn.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mp.asd995.cn

[R79] 解析命令行选项
来源：http://im.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ia.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://yn.jianghongdianzi.cn

time ./run.sh
来源：http://bd.shxzukj.cn

================================================================================
来源：http://wq.nicolike.cn

S. C / C++ 专题
来源：http://eu.huanxung.cn

================================================================================
来源：http://oi.shtwfgs.cn

[S01] C：Hello World
来源：http://az.chemitech.net.cn

#include <stdio.h>
来源：http://xh.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zd.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://sc.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://xr.nszjky.cn

[S03] C：读入整数
来源：http://mv.lnxyls.cn

int x; scanf("%d", &x);
来源：http://jm.gzmigu.cn

[S04] C：字符串复制
来源：http://wi.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wp.panjiajie.cn

[S05] C：字符串长度
来源：http://ha.yuntaijiaju.cn

strlen(s)
来源：http://oq.szsharing.cn

[S06] C：字符串比较
来源：http://bz.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://ad.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://dr.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qj.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://so.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ff.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://on.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ox.wgjwhj.cn

[S10] C：指针与解引用
来源：http://wi.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ea.huixiangedu.cn

[S11] C：逐行读文件
来源：http://mt.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://yx.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fd.muxihuayi.cn

fclose(f);
来源：http://gi.chemitech.net.cn

[S12] C：写文件
来源：http://ro.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wq.9csxet.cn

[S13] C：宏定义
来源：http://mz.hnjuh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nx.shxzukj.cn

[S14] C：枚举
来源：http://sj.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://qr.hahajie.cn

[S15] C：类型转换
来源：http://an.huixiangedu.cn

(double) a / b
来源：http://gh.muxihuayi.cn

[S16] C：位操作置位
来源：http://et.wgjwhj.cn

x |= (1 << 3);
来源：http://nt.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://hi.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uq.chemitech.net.cn

[S18] C：命令行参数
来源：http://cm.shtwfgs.cn

int main(int argc, char **argv)
来源：http://em.huixiangedu.cn

[S19] C：快速排序
来源：http://qx.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://um.gzmigu.cn

[S20] C：二分查找
来源：http://el.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hw.shxzukj.cn

[S21] C：字符类别判断
来源：http://ae.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nv.chemitech.net.cn

[S22] C：字符串转数字
来源：http://jq.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qo.521024.cn

[S23] C：随机数
来源：http://fu.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xc.bjjhwx.cn

[S24] C：获取本地时间
来源：http://uq.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ys.jctech888.com.cn

[S25] C：内存拷贝
来源：http://hh.521024.cn

memcpy(dst, src, n);
来源：http://fh.chemitech.net.cn

[S26] C：内存清零
来源：http://no.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://kt.lnxyls.cn

[S27] C：定义常量
来源：http://kx.muxihuayi.cn

const double PI = 3.14159;
来源：http://ql.chemitech.net.cn

[S28] C：静态变量
来源：http://lk.yuntaijiaju.cn

static int counter = 0;
来源：http://jw.gzmigu.cn

[S29] C：变参函数
来源：http://es.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yu.9csxet.cn

[S30] C：头文件保护
来源：http://sp.bjjhwx.cn


<!-- 参考信息 -->