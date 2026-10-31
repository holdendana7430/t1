代发 wailian999

[Q48] CTE 公用表表达式
来源：http://fa.huixiangedu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mq.szxytkj.cn

SELECT * FROM t WHERE c > 5;
来源：http://zc.chemitech.net.cn

[Q49] 更新单行
来源：http://np.hahajie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xg.9csxet.cn

[Q50] 批量更新
来源：http://gb.huixinmuqiang.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://to.nicolike.cn

[Q51] 用子查询更新
来源：http://lp.panjiajie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wx.haigaiapp.cn

[Q52] 删除指定行
来源：http://qi.bjjhwx.cn

DELETE FROM users WHERE id = 10;
来源：http://ib.nicolike.cn

[Q53] 按条件删除
来源：http://oh.shxzskj.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aj.shtwfgs.cn

[Q54] 清空表
来源：http://zt.shtwfgs.cn

TRUNCATE TABLE logs;
来源：http://xj.jianghongdianzi.cn

[Q55] 排名（并列占位）
来源：http://qh.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lx.colortex.cn

[Q56] 密集排名（并列不占位）
来源：http://it.chemitech.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fq.huixinmuqiang.cn

[Q57] 行号
来源：http://ne.yuntaijiaju.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pk.asd995.cn

[Q58] 累计求和
来源：http://iq.szxytkj.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cn.wgjwhj.cn

[Q59] 分组内累计
来源：http://zg.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://of.nicolike.cn

[Q60] 取上一行 / 下一行
来源：http://bd.panjiajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ye.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hf.jctech888.com.cn

[Q61] 移动平均
来源：http://ri.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pp.lnxyls.cn

[Q62] 分组占比
来源：http://ji.521024.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nx.szxytkj.cn

[Q63] 开启事务
来源：http://ku.huixiangedu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kh.hahajie.cn

[Q64] 提交事务
来源：http://ke.hnjuh.cn

COMMIT;
来源：http://tj.chemitech.net.cn

[Q65] 回滚事务
来源：http://fv.521024.cn

ROLLBACK;
来源：http://gb.jctech888.com.cn

[Q66] 行锁查询
来源：http://jy.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yp.muxihuayi.cn

[Q67] 设置隔离级别
来源：http://lt.huanxung.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eg.wgjwhj.cn

[Q68] 保存点
来源：http://bm.521024.cn

SAVEPOINT sp1;
来源：http://ox.nszjky.cn

ROLLBACK TO sp1;
来源：http://tu.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://qj.szxytkj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ov.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://fn.panjiajie.cn

ANALYZE TABLE users;
来源：http://sl.hnjuh.cn

[Q71] 查看建表语句
来源：http://zz.gzmigu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fm.yuntaijiaju.cn

[Q72] 查看索引
来源：http://kw.shxzskj.cn

SHOW INDEX FROM users;
来源：http://xx.yuntaijiaju.cn

[Q73] 查看表状态
来源：http://fy.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qw.newstarts.cn

[Q74] 强制使用索引
来源：http://cc.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hl.nicolike.cn

[Q75] 日期格式化
来源：http://sg.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uq.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bw.chemitech.net.cn

[Q76] 按天统计
来源：http://uh.9csxet.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ha.hnjuh.cn

[Q77] 时间加减
来源：http://rk.shtwfgs.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gb.huixiangedu.cn

[Q78] 当前时间
来源：http://jh.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jl.panjiajie.cn

[Q79] 字符串拼接
来源：http://nr.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lh.asd995.cn

[Q80] 字符串截取
来源：http://zr.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nf.nszjky.cn

[Q81] 字符串替换
来源：http://rb.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hj.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://bl.chemitech.net.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gv.bookmarksfly.cn

[Q83] 大小写转换
来源：http://bj.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sy.nicolike.cn

[Q84] 去除首尾空格
来源：http://hd.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://hr.bookmarksfly.cn

[Q85] 数值取整
来源：http://ct.nszjky.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hq.shxzukj.cn

[Q86] 读取 JSON 字段
来源：http://yd.gzmigu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qg.huanxung.cn

[Q87] JSON 字段做条件
来源：http://gq.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gl.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://yc.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hh.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bj.newstarts.cn

[Q89] 判断表是否存在
来源：http://nb.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ae.hnjuh.cn

[Q90] 生成序号列
来源：http://do.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yz.shtwfgs.cn

================================================================================
来源：http://hi.bjjhwx.cn

R. Bash 专题
来源：http://xv.huanxung.cn

================================================================================
来源：http://yw.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://jq.haigaiapp.cn

#!/usr/bin/env bash
来源：http://pa.yuexingan06.cn

set -euo pipefail
来源：http://da.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://eh.hnjuh.cn

name="Tom"; echo "$name"
来源：http://yf.jianghongdianzi.cn

[R03] 只读变量
来源：http://lx.newstarts.cn

readonly PI=3.14
来源：http://lo.yuexingan06.cn

[R04] 位置参数
来源：http://ia.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kb.shxzskj.cn

[R05] 参数默认值
来源：http://sb.chemitech.net.cn

name="${1:-default}"
来源：http://jm.jctech888.com.cn

[R06] 判断命令是否存在
来源：http://kx.yuntaijiaju.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ub.shxzskj.cn

[R07] if 判断文件
来源：http://am.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pz.shxzukj.cn

[R08] 数值比较
来源：http://ma.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ud.huixiangedu.cn

[R09] 字符串比较
来源：http://pt.shxzukj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cb.shxzskj.cn

[R10] 正则匹配
来源：http://qw.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fi.shtwfgs.cn

[R11] case 多分支
来源：http://ry.szxytkj.cn

case "$1" in
来源：http://tt.9csxet.cn

start) echo "启动" ;;
来源：http://yp.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://af.wgjwhj.cn

*)     echo "未知命令" ;;
来源：http://xh.521024.cn

esac
来源：http://ke.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://av.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://dj.huixinmuqiang.cn

[R13] for 计数循环
来源：http://ot.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://qw.huixiangedu.cn

[R14] C 风格 for
来源：http://kd.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sz.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://hi.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ly.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ee.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fa.lnxyls.cn

[R17] 数组定义与取值
来源：http://mc.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnjuh.cn

[R18] 遍历数组
来源：http://zs.huanxung.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://je.szsharing.cn

[R19] 数组长度
来源：http://hm.newstarts.cn

echo "${#arr[@]}"
来源：http://lq.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://xp.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ne.wgjwhj.cn

[R21] 字符串长度
来源：http://hi.haigaiapp.cn

echo "${#s}"
来源：http://qy.yuexingan06.cn

[R22] 截取子串
来源：http://qe.colortex.cn

echo "${s:0:5}"
来源：http://vt.jctech888.com.cn

[R23] 字符串替换
来源：http://bn.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://re.huixinmuqiang.cn

[R24] 大小写转换
来源：http://ka.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kw.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://xg.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ef.colortex.cn

[R26] 命令替换
来源：http://yj.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://oh.jianghongdianzi.cn

[R27] 算术展开
来源：http://fx.521024.cn

echo $((1 + 2 * 3))
来源：http://hk.muxihuayi.cn

[R28] 浮点运算
来源：http://sv.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://ac.szxytkj.cn

[R29] 定义函数
来源：http://ri.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://up.hahajie.cn

[R30] 函数返回状态码
来源：http://ip.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://fo.yuntaijiaju.cn

[R31] 局部变量
来源：http://lw.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://so.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://xy.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lb.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://bf.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zn.wgjwhj.cn

[R34] 退出时清理
来源：http://kt.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cf.yuexingan06.cn

[R35] 后台执行并等待
来源：http://dk.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nk.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://zd.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ip.huixinmuqiang.cn

[R37] 把输出赋给变量
来源：http://vg.newstarts.cn

files=$(ls -1)
来源：http://hi.newstarts.cn

[R38] 管道串联
来源：http://kf.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://jr.gzmigu.cn

[R39] 重定向标准输出与错误
来源：http://np.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://zo.haigaiapp.cn

[R40] 追加写日志
来源：http://nk.haigaiapp.cn

echo "log" >> out.log
来源：http://ej.muxihuayi.cn

[R41] 丢弃输出
来源：http://sj.shxzskj.cn

cmd >/dev/null 2>&1
来源：http://ea.huixinmuqiang.cn

[R42] 输入重定向
来源：http://bo.chemitech.net.cn

wc -l < a.txt
来源：http://dn.yuexingan06.cn

[R43] 按名字查找文件
来源：http://vb.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://tk.huixiangedu.cn

[R44] 按修改时间查找
来源：http://oo.bjjhwx.cn

find . -mtime -7 -type f
来源：http://nu.wgjwhj.cn

[R45] 批量删除
来源：http://yf.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://jd.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://bi.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sz.chemitech.net.cn

[R47] sed 单行替换
来源：http://kp.huixinmuqiang.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bv.asd995.cn

[R48] awk 取指定列
来源：http://xz.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://jh.gzmigu.cn

[R49] awk 带条件
来源：http://xe.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vt.bookmarksfly.cn

[R50] awk 求和
来源：http://sw.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://af.gzmigu.cn

[R51] 排序去重取前几
来源：http://qu.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ww.haigaiapp.cn

[R52] 统计行数
来源：http://wq.szsharing.cn

wc -l a.txt
来源：http://oj.yuntaijiaju.cn

[R53] 查看文件头与实时尾
来源：http://um.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wm.lnxyls.cn

[R54] 比较两个文件
来源：http://up.9csxet.cn

diff a.txt b.txt
来源：http://pg.nicolike.cn

[R55] 压缩与解压
来源：http://nt.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wa.muxihuayi.cn

[R56] 远程拷贝
来源：http://nt.muxihuayi.cn

scp file user@host:/path/
来源：http://an.yuexingan06.cn

[R57] 远程执行命令
来源：http://dt.gzmigu.cn

ssh user@host 'uptime'
来源：http://kk.huanxung.cn

[R58] 下载文件
来源：http://cq.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lz.colortex.cn

[R59] 发 POST JSON
来源：http://sp.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hv.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://dl.panjiajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://di.hnjuh.cn

[R61] 磁盘占用
来源：http://bo.szsharing.cn

df -h;  du -sh *
来源：http://ei.bookmarksfly.cn

[R62] 找最占空间的文件
来源：http://bj.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://kw.chemitech.net.cn

[R63] 内存与进程
来源：http://yw.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://ae.huixinmuqiang.cn

[R64] 结束进程
来源：http://ei.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://cj.shtwfgs.cn

[R65] 查看端口占用
来源：http://ev.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oq.hnjuh.cn

[R66] 定时任务
来源：http://na.nszjky.cn

crontab -e;  crontab -l
来源：http://wz.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ka.shxzskj.cn

openssl rand -hex 16
来源：http://zv.colortex.cn

[R68] 计算文件校验值
来源：http://hf.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xe.shtwfgs.cn

[R69] 生成随机密码
来源：http://qc.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://zs.wgjwhj.cn

[R70] 时间戳与互转
来源：http://vu.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://tg.nicolike.cn

[R71] 日期格式化
来源：http://da.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://op.nszjky.cn

[R72] 等待端口就绪
来源：http://nz.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gj.muxihuayi.cn

[R73] 分割大日志
来源：http://bm.521024.cn

split -l 1000 big.log part_
来源：http://bc.shtwfgs.cn

[R74] 批量重命名
来源：http://wk.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fg.shtwfgs.cn

[R75] 导出环境变量
来源：http://tr.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://ay.panjiajie.cn

[R76] 使用临时文件
来源：http://zv.panjiajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wu.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://wt.newstarts.cn

read -rp "请输入: " ans
来源：http://zv.bookmarksfly.cn

[R78] 交互式菜单
来源：http://ou.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fa.yuexingan06.cn

[R79] 解析命令行选项
来源：http://rk.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vp.colortex.cn

[R80] 查看脚本执行耗时
来源：http://xp.jctech888.com.cn

time ./run.sh
来源：http://cy.panjiajie.cn

================================================================================
来源：http://ji.haigaiapp.cn

S. C / C++ 专题
来源：http://nt.shxzskj.cn

================================================================================
来源：http://is.huixiangedu.cn

[S01] C：Hello World
来源：http://wm.jctech888.com.cn

#include <stdio.h>
来源：http://ux.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lc.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://mm.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://bs.muxihuayi.cn

[S03] C：读入整数
来源：http://or.nszjky.cn

int x; scanf("%d", &x);
来源：http://pv.shxzskj.cn

[S04] C：字符串复制
来源：http://wt.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://us.szxytkj.cn

[S05] C：字符串长度
来源：http://lg.shxzukj.cn

strlen(s)
来源：http://oe.lnxyls.cn

[S06] C：字符串比较
来源：http://mt.lnxyls.cn

strcmp(a, b) == 0
来源：http://pz.szsharing.cn

[S07] C：数组遍历求和
来源：http://fm.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zk.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://mj.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dd.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://dj.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fp.colortex.cn

[S10] C：指针与解引用
来源：http://hr.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://te.nszjky.cn

[S11] C：逐行读文件
来源：http://nc.lnxyls.cn

FILE *f = fopen("a.txt", "r");
来源：http://am.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qm.szsharing.cn

fclose(f);
来源：http://tb.haigaiapp.cn

[S12] C：写文件
来源：http://tv.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gn.wgjwhj.cn

[S13] C：宏定义
来源：http://iy.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pe.chemitech.net.cn

[S14] C：枚举
来源：http://ov.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://in.shxzukj.cn

[S15] C：类型转换
来源：http://rt.yuntaijiaju.cn

(double) a / b
来源：http://yj.nszjky.cn

[S16] C：位操作置位
来源：http://jh.panjiajie.cn

x |= (1 << 3);
来源：http://ff.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://rx.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aj.jctech888.com.cn

[S18] C：命令行参数
来源：http://go.gzmigu.cn


<!-- 参考信息 -->