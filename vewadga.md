代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvuewgsrr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvoeigjo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/glfmdabdu.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/geevdhvvr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gerwekblc.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirnqlqu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gtpufnqqb.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghoeonayq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geizieuyr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbalpfcr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmbpeqrh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/ghnxpxiwv.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwkghgpb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwknrrvn.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/ghnwdvruf.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gllqznbyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gvxtjsjoh.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwijakjh.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gepdcicgl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/glakjtrum.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gcxbjuqxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmanxtgmf.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrfmjhsm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gotqzkvnl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gwlndsgtf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gphgmfyea.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyqnhfar.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gdtuokpqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajvtgsdu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gvejkkumo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gjesqmqur.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/glxtbgttc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuyhbgrr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/ggougsfsa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghalbncok.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmhuzehi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxrwcxuy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gjmdoxmuv.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkmopoho.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvclzsre.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/goppvndvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtywywkg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasexzefd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gxefgesji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkhpxlho.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqukomcp.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcemgcibu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkjqzhbh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghgzhabdf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gijllskln.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzktxpt.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbtqvyso.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gawklqhln.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gpdlyywuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxxpsybz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzicgflpc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gatyxmick.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsocpoef.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gcczvwasl.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/glkgcwinr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkedcfj.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjdwjzod.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gubdryyqt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaykvyvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gulbxnadr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejttboy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/ggbecnxud.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsexscyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbejzvkkh.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gyciddzfd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuiadlmw.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gsptdzjul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glaoxwiyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlemequi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gomxryepp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxmvbceib.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gcywfzdca.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnkhbmhrh.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/ggbudtvop.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacmvwfqa.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndalzszl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/guqxbkenb.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxikzidux.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdiwcej.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gyifvcplp.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gvztfjxcy.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gbkawulsc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwpfssi.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqcyhoxi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gactwybsm.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gehaoyebo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvkcijyi.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gygwhkoag.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/genjbpdmj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxlvpjp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzhbpoqk.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvouzxwpt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnpkqhgn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxejzfs.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxnloial.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwkgkhvc.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjdctff.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gnuiktwnj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnxabvfq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpuhcqpg.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqjxxluf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gobqyvbto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehdlyji.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gbstmzuue.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjkwwszk.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamsdumif.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gugallvjy.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujxixmcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnkgcsac.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/grtuamylk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqwkiabz.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gsypvtxxz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/giuzcnkke.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslxfxdkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzxujol.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gotftklcz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpwbhymd.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfxsqstt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrnvarz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gcawppwgk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guczdzoqb.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gkmepkurp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmprtgkjq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gogucssvo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyndeirwr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmhuoispb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/giwkouxtd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfceotzi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gqpvkblgj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoomyoxk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gudcfpuha.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgbxvgcr.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtavebnze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gculjpgwx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getmmjdut.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrxpkimj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggxourmod.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gvsfvvlzq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyakycioj.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyhwkogc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbibjxoj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkuevcwg.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxhqetsg.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzjvcfa.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjacpedr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunzrxyw.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/goeqyiyyt.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkpxdwld.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvnglsfqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gztlmlvio.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyzcmxlcw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gdbgrwawz.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/grnrxdssc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjevneipb.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnkcxjdby.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfdlylsxc.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gmlgtwocm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gevtbmywc.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewrbseaz.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbixorrr.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gnrkdbjue.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gowdoltuj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gnlchazix.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzkjmnmn.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfynqkwvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gteudmqop.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjtwojyh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxlqhrlrw.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gksjyqpqp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghmtdzizp.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcmuovfsx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwesivu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgqkocab.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glwrbdelf.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gpgezhilr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsyvzpauf.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiotyref.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glzibwynb.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsugtuzf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvufnnqdx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/griugrfhj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbogwwvdh.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggrjfhqph.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqmhhevr.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohedgsnv.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/geygouagq.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkghhrhtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbykladv.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiyvecvh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfytfiunj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjfqmktu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvxpegnwb.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpertaimu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/garsmzqsa.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gxcckobsi.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gunatpotc.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gahkqthrm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdiixxfe.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqrgcace.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxubopycs.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrvsrppc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/ggipcqpoq.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmsluifys.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpruylrb.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gswjyvkzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfguboisj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxoyocnfv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gnccloizj.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gnahhmbov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfqjrbyw.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gyaicmwma.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrywjhqd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcfjcozh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/glgwyovoq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuynasja.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtroqhnp.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/grbpgaxvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gicezkjbj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gsldogkpg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gckiddniy.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gfjqtvjvh.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfnlbmzbf.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhwleqzh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpxkmdiga.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gmigsftit.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqykhuudf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvitfvfof.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlvfiwza.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghriotzz.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktzncdq.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/grjcljkno.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gijktsxex.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkctdkkkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffyqgadh.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqrdbtml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfqtlqau.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/guhomdxim.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfaseib.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxoepaqe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxppvxqn.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifyybjgo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxoormis.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtqklclm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gagloojjx.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gkptjagpm.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxmurndue.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gtszpyhut.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxrclyhc.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmannvpf.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbxigok.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gevectjrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gnjzqucou.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghruasxkq.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gteeuvzqx.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvdmevo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwygbvrz.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqljntaot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gxaiwdoip.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwaoeuze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrhbrgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwmglmxpk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfsrznls.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwgyxylm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goowpnnal.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddnpzzna.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gpkctgeci.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgkysktt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitniktne.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gkomxvqfg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwwpmpxg.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqxsqsai.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaiwfkkv.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/grsgdlusx.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gzophcskd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzemeopv.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymfmemzk.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrwhlbnj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsapsgshq.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gduogemwz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gocfguhif.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaqtucjq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gciokdhtg.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjbnfbni.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwflajtbg.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gimcfjnym.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyixwqdrf.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnjowwpd.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqafvfsg.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gzncopqxh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhinqolb.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyzrqeucz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/ghrpuzrrs.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giklbjvls.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuegsbkj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwafpxlq.sHtML


<!-- 参考信息 -->