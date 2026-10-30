代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gnknddxka.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gqdiyritb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrcojede.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/glgokmicx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpltmepwp.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtcecxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goamuwvyv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvxjhxe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gflpaflyh.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/goaoxahep.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocymlald.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ggysbflhs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvdjyrop.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gghdmxsvv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvpqdbjc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/ghpfytdut.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gprpnvpcb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjnruvz.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gcdmvcrdh.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeevyoql.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gqbpdxopq.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefaxuhnn.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfdbivcwi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwiegouq.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjjaukuo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gcshiwoim.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrmpwtdo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gincwxigk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gmnmeblke.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdroptma.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlvlzgpr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkiqmnfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevihmpbg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/goiugdqtf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwomtjqpw.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdvgzrkgc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gkplklmfp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gvxgjbflg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gvcfqjggw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gaexmcjnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gqqkiguqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/guxovakoi.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwwemodp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyxyjeqd.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/glvqlvgoh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gxsfqessa.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glzhxwoyz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjjrndwl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggexcmyof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbcfanpk.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grertpexd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutuvkodl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggglkxqny.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsmugddi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdowxfzkt.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjpdlhke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldthosdl.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstynyxbj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gmtmihebh.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/giogzifhb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvmnruvrm.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtuexcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjezvdxyo.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gydrvwuds.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlixqwjz.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznzhwsgn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqtnwqwx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gpexnpcrc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzgcthim.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwvwtpxz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gpqkmhcve.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gwvjcurvh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqblyswgp.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjmalvqnt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzkjhsvi.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gzqefgblh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/genfftgwl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gijhtzhtz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtvbouxc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geizzicqv.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gsnreajkg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkuskrhex.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouvzkrwh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhfvqcmp.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeevszzt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/ggohmpkeq.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqjfdld.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gemxzvdra.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstvyclfx.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/getilsrlq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/guhjfrspu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsysotvf.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gznhplkuc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlniqvqt.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvxvzndz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpietuijz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gieelspka.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gotvzyihx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/guakfvhyd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwscffszd.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmsxvzk.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/garnarmjw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gzakrerjq.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwntscqs.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecipjgmr.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ggvukwcjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gekvvtplu.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvdqbqt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxiduybi.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhqvdkof.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtfvyizwj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gdtnbaqwo.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnehoqyjy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcllbensq.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gftdjcyzk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gzcskiiof.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gvywhygdn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmpnzmxu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfppxfow.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gshntxdqs.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gijohgyln.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnosackq.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsmlpqhek.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmeedfka.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/ginsjdipp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewssxqvx.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqksdfdo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwrdlppe.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyxeeihi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvyqizevn.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gchocpklc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gpgentkmq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gkldqswuw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/guiqksyjy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/grbpsvect.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfbmfenb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gechzyxvp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydzqdrsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppqliiii.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaglyybq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gbgqyvyjo.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdgldndn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgfgjtve.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbchoaah.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gprvvwnjj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyknpuwe.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdqwnam.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlniusa.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gvdnvuycl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabzvcjxa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjofljkzi.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmhhvgqvb.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gpcpevsnj.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlcgutzz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieejezha.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudzhujoy.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzbfayul.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqcijclho.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeebjljw.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gohesogfv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbzdfcfu.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizyhkuim.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcclhtqfi.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibchxmbu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczteqhx.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfywauok.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwphqmgqq.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/giogubyzw.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/glgzrrboo.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guepibqlh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghymigipk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmjqjhte.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gujvlymwo.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gozinzhpk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxhalch.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkqdnwht.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxjxpviv.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gaelywccw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzuxyglyc.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtavzxdx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsusrwjia.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gesdgkthi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/geywvfbbs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfezrulr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjhlhxlg.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejntwwqu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzojshtiy.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsvavfee.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvmvupai.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhcrjsl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpkzlicyu.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdkpveew.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtawhynlf.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcknvtjoj.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmroqwzs.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbdkyyo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/glfquzata.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gpdljyfcb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmxmjcyqo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipfyprkv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggryqlubo.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnqadqjno.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/glyulrudu.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/giqwhzjmc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvaxgkfw.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/ggwijqyey.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gluugpvaq.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoioigmi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guqkimkst.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuzzotis.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvslfnray.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvyjevoz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqyqmpyo.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gimrdiocj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grotujwfl.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gvevwpisn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gxlmafhbp.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghinzpvzg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gptpyrnts.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gkluqufzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjcloart.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gehrhrybq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gvwwpcmbk.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyuqstxza.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnkvwupf.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjobunrd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gefpjrhsa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/goskomdmy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwuezukx.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmachhiao.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcsbzqc.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjeolewot.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gmppafatt.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiqnnbhn.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzylvgsd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkghbag.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghhagrrez.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxawawof.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gmqztlgfe.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gcbkuqsvs.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/glagysnzz.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrasxjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyalcvkte.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/grlzjiqry.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldfqdrcg.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliixiezd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrzvpzjj.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjckhpvps.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamhlmjk.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkuvmye.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gecuzwhap.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/glsouwmvp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhixlcby.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwivbino.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdchhlmkv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdjfygg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpopzulyz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaopsofjn.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtbxtyzq.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeizhzww.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkfnrlih.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gennsoyce.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtsyouiez.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvzlomw.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gugdosptg.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndslohka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhbqaspp.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gtiqvuauf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjohcrl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gnefposdg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpjwzas.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gvsztbqdk.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gflsorsal.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/ganfjepwl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbiyctim.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gynftoury.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/guybgyzxt.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvthyhfd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpzpggct.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvbibtbu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glidxmnpc.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/glrrqvnvu.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjyburacb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkamrausu.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gkpmpvnse.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjfsnbvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfkopudtj.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gfyhguraa.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gdemomozu.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/ghgacbdud.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/giyqmtdqm.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwkkdkr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcpihwky.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycivpfvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goheocfdy.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhmcgckj.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwmfpwbc.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gswbdaptf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gttylhwuy.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgxkbwuq.sHtML


<!-- 参考信息 -->