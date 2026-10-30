代发 wailian999

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gxlybseyj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gtykqatub.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gpduzihhg.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gsqmyxzat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gxbbflgrt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gaukxvotr.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gebrifbar.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gaxlcbgxo.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/ggrdrrdar.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ganpcndcr.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gmnexukzk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gwjtdkzzb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gakaxenjg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gujgigpbo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gkcragjgg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gnoelvlkl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gsliywwie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gikczlioz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqjawbf.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gdpintovh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gaybyqxan.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/glvqnrfhp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gutxbcmss.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtustctti.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gkparokpq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gfhprrkyp.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gopnlutnh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gqhurwubf.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gpnrnyrcr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gtzxwojqi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gwtveushb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gqsvtxkih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gwkhphfqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gcppwlaot.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gxjrwipou.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gkloqrwff.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gbcabcqjo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/grxaiuvak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gbsfamkkt.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gksllzofv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grkvrpexg.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ggptznbzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gicmajvbw.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gcucavmpx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzanptrmr.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/giiabnyhs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gwimiuvis.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gxttmqhjl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gplogchwj.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/ggqxwpyew.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gevvmpyzt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gejfyxfob.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gyutnvxso.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/grhmxsvbb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkivcljvt.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gsvxrkdme.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gezbbyhfv.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gfdbzxkvm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gakawiieq.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/glnpuuexw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfosvdr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/grhwtzwgg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gimqcrxat.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmztgxdlz.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gjhwwqhla.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtayuxcmr.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ggjesgkdt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gyfihedsu.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gugvberlm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gtxpcdzjh.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gnebnqizk.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gcasktvbq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gocwkubbe.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gzuwtukov.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtavprdiw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gwwfuhgco.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gthjwywio.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gzawifgxe.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gsynajytk.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/glpaepqfh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/ghmnhzzvn.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gpsfejgyb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gievypmqt.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gnlvxerhp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gbqtazhyy.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gcnxnamac.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gauqycndi.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gltejbjwx.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjezwerkl.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gtkoqwijr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/grxuzqsml.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gniugltvc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/glffqmgtx.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/glcynhjac.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/galmkqoem.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/grqjtrlpv.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gbwiahjpc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gkgprosqs.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gamwgjpsk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gmjfuzgqp.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gtapkomit.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/grrbjgeih.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gimitipks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gvjdjgkpn.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gcgngziwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmouvjrgk.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gvihcytoe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjoboyzba.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gzdewammb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjmsxywbi.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gwtidehdq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/guimeckat.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gqerahunx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggzyamyvv.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gbnyqymop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gydfefkak.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gfyokvggq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gcqowpiih.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gycoegpye.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/grajwcxge.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfiyajsiz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gjixkkrbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gppurzfso.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gfwlcibrc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gmemljkjy.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gjpgoxmgz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gwrfvwjej.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjbdgcpru.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gxfyiopbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghumaunay.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gsxrmwxej.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gxokebaaj.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/govmvjnzv.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gdxicmuxe.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gtlddmfdu.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gbkwzcmzc.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/guhkxqdtp.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gzpxmxclb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gwecawboe.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gcmyilsxo.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzqvpmt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/grsrictom.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gnvxqpuen.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gyoszbfnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gaacvjvpn.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gdvvkntvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gfepsjjsb.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gtzeulbir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/grntvzixb.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gmfitepyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdqdjgcox.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gnvubrwos.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gpibonyet.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/ghljvywzk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gezsaxjlj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gtcukkums.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gxcnjwumo.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfupjryjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/greywtrvy.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gprvlplwa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gyofifzjn.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gtgigqfwq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/grlyoruaw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gsoyuebdt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/giknwzehk.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjskpgxbk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gioldjrde.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gtzotokyc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gmkicutsx.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gclmvbdoy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gegdiuunu.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gfzwhvfwl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gplweyaau.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gbifrijkt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gjnypvvby.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gijemruuf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gccsjqmyg.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gfcrtnrns.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gucknwpau.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxzklaguf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gjywpcnub.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gucjsbhmp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/giwyqjqzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gsmsejuim.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/ghdvxyokd.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gsmgtdjil.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gsdonzlrt.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/ggzgoqbzw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gamqxpltn.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gtflhdydm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gkrvqcceo.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/glxilcbem.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gkahchden.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gwblvrstc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/grhvwmbqq.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gpehkfuej.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gbfmawsjv.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gtpjmhcgp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gnljekbfh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gyqzdrdzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gonzyhjhj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gnzppuvyg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gciexyygk.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gkvcrueat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gdammkuun.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/glqtmfcml.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gaeklsxso.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gdbbqqixd.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gcxstzuhe.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gqvimesnx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/ganxrkztu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gffcevrsa.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gxxhachor.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpyvrborx.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/goodvpvcc.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gftatlreq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gizjmawbk.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/ghpfhaqtw.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gyoaznvzv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gdxpjsyiy.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/giuqnftgd.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/ggbyrvhnj.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gvfgqsvzq.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/galisukna.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gpwyxqixh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gquuokqmd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gsoxxruag.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gnxiebehs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/grgrbdmue.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gftkwvrjs.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gtnmwiyfp.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gkeajoght.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gjxqhoclp.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/guvnxfyjr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gptxvkgmb.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gaaklvfjx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gyxwlwqmn.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gbztyopqc.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gnebxmydx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gszlhxisc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gfpbrfpsv.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gjmlucrjx.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gsfxhorbs.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/ghkxiuqqu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gwqupoozl.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqkoqqsif.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gsaxnofpj.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gsvthssvz.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gzkrphlpv.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gueuhjdtu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/grhdowqzp.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gbopdtqtr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gnoxdnlsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gkpsafusx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gjomegcdl.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gkodankzq.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gapyolnnt.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gvaslhgba.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gigtwfmfd.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/glrjjvhwd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gcislccqq.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gtbyzfgeg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gydoudwyt.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gmqoxknnl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gnaffcitc.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/guldhzcjl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gafjdvagz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/guqgjcstv.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gsofakhkd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gywhqoqbg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gjpschfch.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gevtevusc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gfhncepud.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/glqgiaukv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gbjbhxlys.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gncrhmahz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gtxqbucem.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gwzatcret.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gamuccjzs.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/ghgyfjezc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gtgkgsjkk.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/ggehbzlfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gluwsbejn.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/glzqsoedy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gzldwhzbe.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gcdywtshy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtpjmynij.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gztbpgtbh.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gvceplfzo.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gtjevcinw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzzazdrhg.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gippmmmrf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gqskwhhjn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gsayxrazf.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/glnuvoxug.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdofidagw.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gqbkjybln.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grfwqzyca.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gguhzdcuu.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbsvcpv.sHtML


<!-- 参考信息 -->