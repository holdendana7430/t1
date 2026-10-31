代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://sn.huanxung.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xy.shxzukj.cn

[Q43] 标量子查询
来源：http://hj.huanxung.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nd.yuntaijiaju.cn

[Q44] IN 子查询
来源：http://xj.nicolike.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pr.szsharing.cn

[Q45] EXISTS 判断存在
来源：http://ix.jctech888.com.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kg.haigaiapp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gb.szsharing.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lb.nicolike.cn

[Q47] 与平均值比较
来源：http://fx.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vu.wgjwhj.cn

[Q48] CTE 公用表表达式
来源：http://mr.nszjky.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dh.nszjky.cn

SELECT * FROM t WHERE c > 5;
来源：http://ns.colortex.cn

[Q49] 更新单行
来源：http://jp.huanxung.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ru.panjiajie.cn

[Q50] 批量更新
来源：http://gv.nicolike.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tf.muxihuayi.cn

[Q51] 用子查询更新
来源：http://tr.shxzskj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ri.gzmigu.cn

[Q52] 删除指定行
来源：http://wq.haigaiapp.cn

DELETE FROM users WHERE id = 10;
来源：http://ft.panjiajie.cn

[Q53] 按条件删除
来源：http://yz.huixiangedu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ej.lnxyls.cn

[Q54] 清空表
来源：http://vh.asd995.cn

TRUNCATE TABLE logs;
来源：http://ln.bjjhwx.cn

[Q55] 排名（并列占位）
来源：http://dx.haigaiapp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mo.jianghongdianzi.cn

[Q56] 密集排名（并列不占位）
来源：http://al.bjjhwx.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://py.szxytkj.cn

[Q57] 行号
来源：http://ub.hahajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zp.shxzukj.cn

[Q58] 累计求和
来源：http://vj.yuntaijiaju.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wc.bjjhwx.cn

[Q59] 分组内累计
来源：http://ru.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jt.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://bi.szsharing.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cz.521024.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ed.szsharing.cn

[Q61] 移动平均
来源：http://wd.9csxet.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://he.hahajie.cn

[Q62] 分组占比
来源：http://cw.szxytkj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ql.yuntaijiaju.cn

[Q63] 开启事务
来源：http://zh.yuexingan06.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hg.521024.cn

[Q64] 提交事务
来源：http://xy.bookmarksfly.cn

COMMIT;
来源：http://tq.yuntaijiaju.cn

[Q65] 回滚事务
来源：http://st.chemitech.net.cn

ROLLBACK;
来源：http://gs.colortex.cn

[Q66] 行锁查询
来源：http://hu.shxzukj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lf.shxzukj.cn

[Q67] 设置隔离级别
来源：http://lb.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zm.muxihuayi.cn

[Q68] 保存点
来源：http://aw.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://my.shxzukj.cn

ROLLBACK TO sp1;
来源：http://aw.chemitech.net.cn

[Q69] 查看执行计划
来源：http://rj.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ch.shxzukj.cn

[Q70] 更新统计信息
来源：http://rw.jctech888.com.cn

ANALYZE TABLE users;
来源：http://nh.jctech888.com.cn

[Q71] 查看建表语句
来源：http://wu.szxytkj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kd.hnjuh.cn

[Q72] 查看索引
来源：http://ql.colortex.cn

SHOW INDEX FROM users;
来源：http://vz.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://qc.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mz.lnxyls.cn

[Q74] 强制使用索引
来源：http://xl.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zb.bookmarksfly.cn

[Q75] 日期格式化
来源：http://ui.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qk.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bp.521024.cn

[Q76] 按天统计
来源：http://bj.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hj.yuexingan06.cn

[Q77] 时间加减
来源：http://he.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ym.szxytkj.cn

[Q78] 当前时间
来源：http://zr.jctech888.com.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ip.chemitech.net.cn

[Q79] 字符串拼接
来源：http://jf.jctech888.com.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lt.huanxung.cn

[Q80] 字符串截取
来源：http://au.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pf.chemitech.net.cn

[Q81] 字符串替换
来源：http://bg.jctech888.com.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bm.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ux.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sy.nicolike.cn

[Q83] 大小写转换
来源：http://ve.newstarts.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wm.szsharing.cn

[Q84] 去除首尾空格
来源：http://qh.chemitech.net.cn

SELECT TRIM(name) FROM users;
来源：http://nw.gzmigu.cn

[Q85] 数值取整
来源：http://hu.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pn.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://kp.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iz.wgjwhj.cn

[Q87] JSON 字段做条件
来源：http://ru.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://au.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://ej.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bm.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ek.colortex.cn

[Q89] 判断表是否存在
来源：http://on.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qd.chemitech.net.cn

[Q90] 生成序号列
来源：http://jl.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://up.bookmarksfly.cn

================================================================================
来源：http://ln.asd995.cn

R. Bash 专题
来源：http://ap.shxzskj.cn

================================================================================
来源：http://me.szsharing.cn

[R01] shebang 与严格模式
来源：http://op.shxzukj.cn

#!/usr/bin/env bash
来源：http://fk.nszjky.cn

set -euo pipefail
来源：http://ea.lnxyls.cn

[R02] 变量赋值与使用
来源：http://wo.nszjky.cn

name="Tom"; echo "$name"
来源：http://it.szxytkj.cn

[R03] 只读变量
来源：http://vv.szxytkj.cn

readonly PI=3.14
来源：http://vg.9csxet.cn

[R04] 位置参数
来源：http://ix.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dq.lnxyls.cn

[R05] 参数默认值
来源：http://uo.szsharing.cn

name="${1:-default}"
来源：http://we.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://wq.jianghongdianzi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ow.shxzskj.cn

[R07] if 判断文件
来源：http://ur.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tz.shxzskj.cn

[R08] 数值比较
来源：http://pz.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ot.521024.cn

[R09] 字符串比较
来源：http://uz.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jx.521024.cn

[R10] 正则匹配
来源：http://qw.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oi.szsharing.cn

[R11] case 多分支
来源：http://ou.shxzskj.cn

case "$1" in
来源：http://ob.colortex.cn

start) echo "启动" ;;
来源：http://sv.yuntaijiaju.cn

stop)  echo "停止" ;;
来源：http://rj.jctech888.com.cn

*)     echo "未知命令" ;;
来源：http://zj.bjjhwx.cn

esac
来源：http://yp.colortex.cn

[R12] for 遍历文件
来源：http://al.9csxet.cn

for f in *.txt; do echo "$f"; done
来源：http://wz.huixiangedu.cn

[R13] for 计数循环
来源：http://lr.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://we.jctech888.com.cn

[R14] C 风格 for
来源：http://on.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ns.panjiajie.cn

[R15] while 逐行读文件
来源：http://nu.hahajie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yg.huixinmuqiang.cn

[R16] until 等待条件
来源：http://gr.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wb.lnxyls.cn

[R17] 数组定义与取值
来源：http://te.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://np.yuexingan06.cn

[R18] 遍历数组
来源：http://pm.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sf.colortex.cn

[R19] 数组长度
来源：http://au.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://du.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://xe.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gl.9csxet.cn

[R21] 字符串长度
来源：http://ng.hnjuh.cn

echo "${#s}"
来源：http://bj.jianghongdianzi.cn

[R22] 截取子串
来源：http://lf.yuexingan06.cn

echo "${s:0:5}"
来源：http://vl.szxytkj.cn

[R23] 字符串替换
来源：http://gn.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://id.szxytkj.cn

[R24] 大小写转换
来源：http://dh.muxihuayi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xr.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://gz.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lc.shxzukj.cn

[R26] 命令替换
来源：http://dn.yuntaijiaju.cn

now=$(date +%F); echo "$now"
来源：http://ll.521024.cn

[R27] 算术展开
来源：http://pb.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://er.nszjky.cn

[R28] 浮点运算
来源：http://xp.lnxyls.cn

echo "scale=2; 10/3" | bc
来源：http://kb.asd995.cn

[R29] 定义函数
来源：http://wn.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ev.wgjwhj.cn

[R30] 函数返回状态码
来源：http://df.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://yx.hnjuh.cn

[R31] 局部变量
来源：http://vt.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://gk.bjjhwx.cn

[R32] 参数个数校验
来源：http://rp.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bu.colortex.cn

[R33] 捕获错误并提示行号
来源：http://uj.huixiangedu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iw.nszjky.cn

[R34] 退出时清理
来源：http://ay.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ty.newstarts.cn

[R35] 后台执行并等待
来源：http://de.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qj.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://bv.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wo.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://rr.nicolike.cn

files=$(ls -1)
来源：http://fh.gzmigu.cn

[R38] 管道串联
来源：http://yj.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://nv.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://hi.huanxung.cn

cmd > out.log 2>&1
来源：http://xp.wgjwhj.cn

[R40] 追加写日志
来源：http://ai.huixiangedu.cn

echo "log" >> out.log
来源：http://kz.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://gh.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://br.yuexingan06.cn

[R42] 输入重定向
来源：http://ue.nicolike.cn

wc -l < a.txt
来源：http://be.shtwfgs.cn

[R43] 按名字查找文件
来源：http://hm.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://ri.chemitech.net.cn

[R44] 按修改时间查找
来源：http://oy.haigaiapp.cn

find . -mtime -7 -type f
来源：http://iv.szsharing.cn

[R45] 批量删除
来源：http://fx.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://mz.newstarts.cn

[R46] 递归替换文件内容
来源：http://dy.hnjuh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bt.asd995.cn

[R47] sed 单行替换
来源：http://eq.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tl.shxzskj.cn

[R48] awk 取指定列
来源：http://ui.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://ed.lnxyls.cn

[R49] awk 带条件
来源：http://qa.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://um.yuexingan06.cn

[R50] awk 求和
来源：http://oi.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sz.shxzskj.cn

[R51] 排序去重取前几
来源：http://lp.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nc.gzmigu.cn

[R52] 统计行数
来源：http://pu.newstarts.cn

wc -l a.txt
来源：http://wj.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://hx.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gh.chemitech.net.cn

[R54] 比较两个文件
来源：http://hz.yuntaijiaju.cn

diff a.txt b.txt
来源：http://cm.shtwfgs.cn

[R55] 压缩与解压
来源：http://ot.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://je.shxzukj.cn

[R56] 远程拷贝
来源：http://if.gzmigu.cn

scp file user@host:/path/
来源：http://ci.colortex.cn

[R57] 远程执行命令
来源：http://cu.newstarts.cn

ssh user@host 'uptime'
来源：http://cm.panjiajie.cn

[R58] 下载文件
来源：http://nw.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ib.szxytkj.cn

[R59] 发 POST JSON
来源：http://tz.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ap.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://dv.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zu.nszjky.cn

[R61] 磁盘占用
来源：http://sm.muxihuayi.cn

df -h;  du -sh *
来源：http://by.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ce.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://iw.newstarts.cn

[R63] 内存与进程
来源：http://ux.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://ey.shxzukj.cn

[R64] 结束进程
来源：http://fo.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://ge.lnxyls.cn

[R65] 查看端口占用
来源：http://wu.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mc.panjiajie.cn

[R66] 定时任务
来源：http://bu.chemitech.net.cn

crontab -e;  crontab -l
来源：http://tc.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://vb.bookmarksfly.cn

openssl rand -hex 16
来源：http://dy.lnxyls.cn

[R68] 计算文件校验值
来源：http://qw.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://we.bookmarksfly.cn

[R69] 生成随机密码
来源：http://ln.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://sp.nszjky.cn

[R70] 时间戳与互转
来源：http://pl.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://sv.9csxet.cn

[R71] 日期格式化
来源：http://hn.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ys.shtwfgs.cn

[R72] 等待端口就绪
来源：http://pp.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lz.nicolike.cn

[R73] 分割大日志
来源：http://gd.hnjuh.cn

split -l 1000 big.log part_
来源：http://pu.huixiangedu.cn

[R74] 批量重命名
来源：http://yv.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wi.521024.cn

[R75] 导出环境变量
来源：http://bw.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://ni.haigaiapp.cn

[R76] 使用临时文件
来源：http://ax.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yb.huixiangedu.cn

[R77] 读取用户输入
来源：http://wq.szsharing.cn

read -rp "请输入: " ans
来源：http://hl.wgjwhj.cn

[R78] 交互式菜单
来源：http://qg.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gm.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ih.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bp.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://xy.lnxyls.cn

time ./run.sh
来源：http://zd.newstarts.cn

================================================================================
来源：http://ps.lnxyls.cn

S. C / C++ 专题
来源：http://qq.haigaiapp.cn

================================================================================
来源：http://hq.szsharing.cn

[S01] C：Hello World
来源：http://cl.shtwfgs.cn

#include <stdio.h>
来源：http://gy.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zf.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://jj.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://vr.muxihuayi.cn

[S03] C：读入整数
来源：http://sf.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://hf.huixinmuqiang.cn

[S04] C：字符串复制
来源：http://ne.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hq.colortex.cn

[S05] C：字符串长度
来源：http://ol.yuntaijiaju.cn

strlen(s)
来源：http://lh.nszjky.cn

[S06] C：字符串比较
来源：http://ea.szsharing.cn

strcmp(a, b) == 0
来源：http://zm.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://xn.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vf.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://jq.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kw.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://gp.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qi.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://xy.hahajie.cn

int *p = &a;  *p = 5;
来源：http://fu.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://zc.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://iw.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hv.asd995.cn

fclose(f);
来源：http://se.asd995.cn

[S12] C：写文件
来源：http://ov.muxihuayi.cn


<!-- 参考信息 -->