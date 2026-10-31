代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ll.9csxet.cn

[Q24] 去重
来源：http://gk.colortex.cn

SELECT DISTINCT city FROM users;
来源：http://dy.szsharing.cn

[Q25] 只取前 N 条
来源：http://ej.haigaiapp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zz.jctech888.com.cn

[Q26] 计数
来源：http://nk.jctech888.com.cn

SELECT COUNT(*) FROM users;
来源：http://cf.huixiangedu.cn

[Q27] 条件计数
来源：http://tr.bjjhwx.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gr.chemitech.net.cn

[Q28] 求和与平均
来源：http://vy.bjjhwx.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gy.huanxung.cn

[Q29] 最大最小值
来源：http://rw.521024.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zb.shxzukj.cn

[Q30] 分组统计
来源：http://sg.asd995.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ag.hahajie.cn

[Q31] 分组后过滤
来源：http://vz.muxihuayi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ia.gzmigu.cn

[Q32] 分组拼接字符串
来源：http://in.hnjuh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wv.nszjky.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://js.bookmarksfly.cn

[Q33] 多列分组
来源：http://or.shtwfgs.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yx.colortex.cn

[Q34] 每组取第一条
来源：http://sz.shxzskj.cn

SELECT * FROM (
来源：http://gz.asd995.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xd.nicolike.cn

) t WHERE rn = 1;
来源：http://bs.lnxyls.cn

[Q35] 内连接
来源：http://jw.huixinmuqiang.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ke.bookmarksfly.cn

[Q36] 左连接
来源：http://ey.shxzukj.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gl.szsharing.cn

[Q37] 右连接
来源：http://ba.lnxyls.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jx.newstarts.cn

[Q38] 全外连接（PostgreSQL）
来源：http://db.asd995.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mh.shxzskj.cn

[Q39] 自连接（查上下级）
来源：http://ll.chemitech.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ae.szsharing.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gs.huanxung.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jn.gzmigu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://py.yuntaijiaju.cn

[Q41] 多表连接
来源：http://rf.nszjky.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tp.jianghongdianzi.cn

JOIN users u ON u.id = o.user_id
来源：http://bn.huixinmuqiang.cn

JOIN products p ON p.id = o.product_id;
来源：http://xl.yuexingan06.cn

[Q42] 连接条件附加过滤
来源：http://ix.lnxyls.cn

SELECT u.name, o.amount FROM users u
来源：http://xw.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lz.nicolike.cn

[Q43] 标量子查询
来源：http://if.shxzskj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sx.bookmarksfly.cn

[Q44] IN 子查询
来源：http://ak.gzmigu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vy.huixinmuqiang.cn

[Q45] EXISTS 判断存在
来源：http://pe.chemitech.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ro.panjiajie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ev.yuntaijiaju.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fi.wgjwhj.cn

[Q47] 与平均值比较
来源：http://xf.huixinmuqiang.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kn.lnxyls.cn

[Q48] CTE 公用表表达式
来源：http://kr.gzmigu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yi.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://nu.nszjky.cn

[Q49] 更新单行
来源：http://zo.yuexingan06.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uw.haigaiapp.cn

[Q50] 批量更新
来源：http://si.wgjwhj.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eg.shxzukj.cn

[Q51] 用子查询更新
来源：http://qs.bookmarksfly.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dy.shtwfgs.cn

[Q52] 删除指定行
来源：http://wo.szxytkj.cn

DELETE FROM users WHERE id = 10;
来源：http://fl.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://en.shtwfgs.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ik.huanxung.cn

[Q54] 清空表
来源：http://ho.nicolike.cn

TRUNCATE TABLE logs;
来源：http://us.yuexingan06.cn

[Q55] 排名（并列占位）
来源：http://zy.asd995.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gp.chemitech.net.cn

[Q56] 密集排名（并列不占位）
来源：http://wt.bookmarksfly.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lb.szxytkj.cn

[Q57] 行号
来源：http://ta.chemitech.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ks.huanxung.cn

[Q58] 累计求和
来源：http://pb.jianghongdianzi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nj.521024.cn

[Q59] 分组内累计
来源：http://ei.bookmarksfly.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yx.colortex.cn

[Q60] 取上一行 / 下一行
来源：http://xc.huanxung.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lp.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kd.huixiangedu.cn

[Q61] 移动平均
来源：http://bw.asd995.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kl.nszjky.cn

[Q62] 分组占比
来源：http://nw.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ut.colortex.cn

[Q63] 开启事务
来源：http://zh.szxytkj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://eg.bjjhwx.cn

[Q64] 提交事务
来源：http://wy.newstarts.cn

COMMIT;
来源：http://hw.jianghongdianzi.cn

[Q65] 回滚事务
来源：http://qk.nszjky.cn

ROLLBACK;
来源：http://mo.szxytkj.cn

[Q66] 行锁查询
来源：http://rq.bookmarksfly.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kq.newstarts.cn

[Q67] 设置隔离级别
来源：http://kd.bookmarksfly.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ko.hahajie.cn

[Q68] 保存点
来源：http://uk.gzmigu.cn

SAVEPOINT sp1;
来源：http://gg.lnxyls.cn

ROLLBACK TO sp1;
来源：http://fi.asd995.cn

[Q69] 查看执行计划
来源：http://hd.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hx.bookmarksfly.cn

[Q70] 更新统计信息
来源：http://qi.hahajie.cn

ANALYZE TABLE users;
来源：http://id.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://in.nszjky.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://io.lnxyls.cn

[Q72] 查看索引
来源：http://fq.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://pz.haigaiapp.cn

[Q73] 查看表状态
来源：http://iy.shxzukj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bu.szsharing.cn

[Q74] 强制使用索引
来源：http://bt.chemitech.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gf.lnxyls.cn

[Q75] 日期格式化
来源：http://ld.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tm.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hj.9csxet.cn

[Q76] 按天统计
来源：http://hb.huanxung.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pp.521024.cn

[Q77] 时间加减
来源：http://pp.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jf.yuexingan06.cn

[Q78] 当前时间
来源：http://pv.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jj.chemitech.net.cn

[Q79] 字符串拼接
来源：http://tk.huixinmuqiang.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://go.jianghongdianzi.cn

[Q80] 字符串截取
来源：http://eo.huixinmuqiang.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sd.lnxyls.cn

[Q81] 字符串替换
来源：http://yf.newstarts.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ij.gzmigu.cn

[Q82] 字符长度与字节长度
来源：http://gs.bookmarksfly.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gg.521024.cn

[Q83] 大小写转换
来源：http://yc.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yw.huanxung.cn

[Q84] 去除首尾空格
来源：http://kq.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://pu.lnxyls.cn

[Q85] 数值取整
来源：http://fi.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mg.bookmarksfly.cn

[Q86] 读取 JSON 字段
来源：http://sq.newstarts.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ar.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://th.panjiajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ho.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://lm.jianghongdianzi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oi.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rd.nicolike.cn

[Q89] 判断表是否存在
来源：http://xt.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jz.gzmigu.cn

[Q90] 生成序号列
来源：http://ov.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mn.chemitech.net.cn

================================================================================
来源：http://jk.huixinmuqiang.cn

R. Bash 专题
来源：http://xm.huixiangedu.cn

================================================================================
来源：http://sv.lnxyls.cn

[R01] shebang 与严格模式
来源：http://vn.nszjky.cn

#!/usr/bin/env bash
来源：http://an.szsharing.cn

set -euo pipefail
来源：http://sw.huanxung.cn

[R02] 变量赋值与使用
来源：http://pq.jianghongdianzi.cn

name="Tom"; echo "$name"
来源：http://ng.chemitech.net.cn

[R03] 只读变量
来源：http://mb.nszjky.cn

readonly PI=3.14
来源：http://ly.hahajie.cn

[R04] 位置参数
来源：http://vr.muxihuayi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ol.bookmarksfly.cn

[R05] 参数默认值
来源：http://dl.shtwfgs.cn

name="${1:-default}"
来源：http://hh.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://so.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hp.nszjky.cn

[R07] if 判断文件
来源：http://dj.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dl.panjiajie.cn

[R08] 数值比较
来源：http://cm.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tk.huixiangedu.cn

[R09] 字符串比较
来源：http://ki.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zk.shtwfgs.cn

[R10] 正则匹配
来源：http://vc.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vx.asd995.cn

[R11] case 多分支
来源：http://hh.asd995.cn

case "$1" in
来源：http://go.shxzukj.cn

start) echo "启动" ;;
来源：http://mc.chemitech.net.cn

stop)  echo "停止" ;;
来源：http://gs.chemitech.net.cn

*)     echo "未知命令" ;;
来源：http://bg.huanxung.cn

esac
来源：http://ox.nicolike.cn

[R12] for 遍历文件
来源：http://wy.shxzskj.cn

for f in *.txt; do echo "$f"; done
来源：http://yw.bjjhwx.cn

[R13] for 计数循环
来源：http://zp.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://vd.bookmarksfly.cn

[R14] C 风格 for
来源：http://hq.shtwfgs.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zb.hahajie.cn

[R15] while 逐行读文件
来源：http://vl.nszjky.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://td.jianghongdianzi.cn

[R16] until 等待条件
来源：http://cv.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bk.shxzukj.cn

[R17] 数组定义与取值
来源：http://qc.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fl.colortex.cn

[R18] 遍历数组
来源：http://tq.szxytkj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pe.nszjky.cn

[R19] 数组长度
来源：http://mp.colortex.cn

echo "${#arr[@]}"
来源：http://pe.chemitech.net.cn

[R20] 关联数组（字典）
来源：http://fj.hahajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xt.nicolike.cn

[R21] 字符串长度
来源：http://zw.jianghongdianzi.cn

echo "${#s}"
来源：http://vp.huixiangedu.cn

[R22] 截取子串
来源：http://hb.hahajie.cn

echo "${s:0:5}"
来源：http://jf.huixiangedu.cn

[R23] 字符串替换
来源：http://ly.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qn.haigaiapp.cn

[R24] 大小写转换
来源：http://jm.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gg.huixiangedu.cn

[R25] 去后缀 / 去前缀
来源：http://lb.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kd.szsharing.cn

[R26] 命令替换
来源：http://tv.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://xh.haigaiapp.cn

[R27] 算术展开
来源：http://mw.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://rg.huixiangedu.cn

[R28] 浮点运算
来源：http://jr.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://xq.nicolike.cn

[R29] 定义函数
来源：http://em.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hy.szsharing.cn

[R30] 函数返回状态码
来源：http://ko.nszjky.cn

f() { return 0; }; f || echo "失败了"
来源：http://ln.szsharing.cn

[R31] 局部变量
来源：http://ix.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://pn.huanxung.cn

[R32] 参数个数校验
来源：http://dt.newstarts.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vv.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://ue.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yk.9csxet.cn

[R34] 退出时清理
来源：http://by.szxytkj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qn.muxihuayi.cn

[R35] 后台执行并等待
来源：http://fj.shtwfgs.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jq.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://so.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://by.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ad.9csxet.cn

files=$(ls -1)
来源：http://dg.huanxung.cn

[R38] 管道串联
来源：http://oy.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://az.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://jx.huixiangedu.cn

cmd > out.log 2>&1
来源：http://le.gzmigu.cn

[R40] 追加写日志
来源：http://ql.nicolike.cn

echo "log" >> out.log
来源：http://kx.wgjwhj.cn

[R41] 丢弃输出
来源：http://fk.hahajie.cn

cmd >/dev/null 2>&1
来源：http://yu.bookmarksfly.cn

[R42] 输入重定向
来源：http://zd.yuexingan06.cn

wc -l < a.txt
来源：http://kp.hahajie.cn

[R43] 按名字查找文件
来源：http://gg.hahajie.cn

find . -name "*.log" -type f
来源：http://kn.wgjwhj.cn

[R44] 按修改时间查找
来源：http://ig.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://sg.yuntaijiaju.cn

[R45] 批量删除
来源：http://nb.521024.cn

find . -name "*.tmp" -delete
来源：http://nn.9csxet.cn

[R46] 递归替换文件内容
来源：http://tf.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xf.chemitech.net.cn

[R47] sed 单行替换
来源：http://hw.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wr.gzmigu.cn

[R48] awk 取指定列
来源：http://tm.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://tn.colortex.cn

[R49] awk 带条件
来源：http://vz.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gu.9csxet.cn

[R50] awk 求和
来源：http://ge.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zh.shxzukj.cn

[R51] 排序去重取前几
来源：http://uz.nszjky.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wz.521024.cn

[R52] 统计行数
来源：http://ve.bookmarksfly.cn

wc -l a.txt
来源：http://rd.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://mh.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://am.huixiangedu.cn

[R54] 比较两个文件
来源：http://yc.haigaiapp.cn

diff a.txt b.txt
来源：http://uw.bookmarksfly.cn

[R55] 压缩与解压
来源：http://lr.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jk.shxzukj.cn

[R56] 远程拷贝
来源：http://ve.gzmigu.cn

scp file user@host:/path/
来源：http://ue.jctech888.com.cn

[R57] 远程执行命令
来源：http://kl.szxytkj.cn

ssh user@host 'uptime'
来源：http://xp.bookmarksfly.cn

[R58] 下载文件
来源：http://xq.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rc.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://ai.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gl.lnxyls.cn

[R60] 只看 HTTP 状态码
来源：http://ri.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ef.hahajie.cn

[R61] 磁盘占用
来源：http://mg.szxytkj.cn

df -h;  du -sh *
来源：http://is.hahajie.cn

[R62] 找最占空间的文件
来源：http://dd.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ea.szxytkj.cn

[R63] 内存与进程
来源：http://tb.haigaiapp.cn

free -h;  ps aux | grep nginx
来源：http://jw.muxihuayi.cn

[R64] 结束进程
来源：http://zo.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://cy.jctech888.com.cn

[R65] 查看端口占用
来源：http://ei.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lg.asd995.cn

[R66] 定时任务
来源：http://wa.shxzskj.cn

crontab -e;  crontab -l
来源：http://xj.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://wv.szxytkj.cn

openssl rand -hex 16
来源：http://ra.huixiangedu.cn

[R68] 计算文件校验值
来源：http://cg.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://my.wgjwhj.cn

[R69] 生成随机密码
来源：http://gi.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://vh.nszjky.cn

[R70] 时间戳与互转
来源：http://gh.nszjky.cn

date +%s;  date -d @1700000000
来源：http://pq.shxzukj.cn

[R71] 日期格式化
来源：http://sx.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wk.hnjuh.cn

[R72] 等待端口就绪
来源：http://ng.newstarts.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ty.jianghongdianzi.cn

[R73] 分割大日志
来源：http://tr.shxzukj.cn


<!-- 参考信息 -->