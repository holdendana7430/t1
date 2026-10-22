代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sheqqqzd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cqlzydhw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jwcxhydv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uiccbxon.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dazbxbnd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2aynwyale.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmcyaoa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xollidht.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wmxfmshb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uiwombps.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ldnlrsnj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2blfnpzzu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jqzfgacv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nzweesww.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2raqjfxhg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2acwoymie.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vzlrcykr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qutspray.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2luodsacz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lcbgynmy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vtkoqwnw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wzecssti.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xndqldjc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2aldoxzwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2efhyofhp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2dwxaczog.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2neaddjfd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2arsniwsd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbfhhapg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zhdegfoq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vjpmzvcw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bvyhdmvt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iftpteat.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wtkggldy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ctzwvrcl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gvqnvpxg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nqyzztbs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgmvdyrp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wakbxvaq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jqavpoln.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2frfyopow.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vnmiugqi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dcvxjkye.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bdfcezjf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fsinyeoo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfspxsnj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wlexiycd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gimipfxg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xucjoeuh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqpcllcl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2snaqiesc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fdjcgiqt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ferjpqmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2njmwwhwr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pqxqlstc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2trvtbfqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hyotamuu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2keszyaln.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ljzexeey.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dsaatzxs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ickxppnf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wkecwzek.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xpbewjfh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sfiwvxzd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rhrqiaor.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ugcpmczp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uaqmwbkh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fipigqij.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gptoglsb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uxocynjb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vbpkyqih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uyrnwquk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rokiwijm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2occhezei.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2evbohxgs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ildvjlxv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2oqjhnqtn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qgqjgivb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ktlxfnzm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uvctybjm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oqfheuia.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gkaojhgp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jswxgrqf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gbotwiim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2blkwcbne.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2uhrdksdl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ktqlwllp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aszanhyp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2safkcxfc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ikvutvvf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjxnbj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2elpjhira.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jqpmyits.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gzjnutxn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gawzywel.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ozkxjrft.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnuqwfsm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2khauozom.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksuogcvz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xaaniwzr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qjixfcwj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2naymrnpp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mdfrehip.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmnqws.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2duojvtcc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2snrrxlma.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sbmckqnq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xmvvothu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ouhgkswy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2irxrpppk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hquzrlhg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ixuunivk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ovafodbl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wnpgowyc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lvamchql.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gmaitovk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dyenasjf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2coyadtzv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cvxblbyw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwapaoeh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jatczcvu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oxkeexby.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ojwkahgd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bjcqcsxi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iehprilt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vaphesuv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jqaptjbm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zvlbuyfb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2toboqqri.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2oibptove.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gtwfcarr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vsymcicc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yooczont.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jtmbhyoc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlzdsigx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tlvcppbs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nabdsoll.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hhhoknbp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2fknsjyyf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2afyfyslv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2glomugwb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hatmtkmz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gqyqiuao.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ohvbicrv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2omtynjlj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkjzaeaz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jiktmdxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mvjacjiv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mynfgwkf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cchqneir.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lvgwyirt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zezcwadi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uwopdszq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xryqhbld.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bbvynyjb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nhzygogu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lrpprzbc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wvcnufhx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zchciihf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tybmhsfe.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vgslrbdu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nxnzuygm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oymmymwx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rksbwuwp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rhzmskki.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ylzuwjqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fnwoochk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwdkfdgt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vwvisnvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mankdirm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2bndixjam.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ngofmbdb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lfyayhlj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cmbnryqg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mqsyvhky.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnsvglrx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vtyxyoca.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvjraheo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bbqairwt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tgrqyofv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2trocyyzt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ukrnwlmt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyyediej.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gycxteaa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mottouuv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kyzdtejk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2otjaavqj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pmnldlkm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ssyudzxw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ynceajvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sbmoxxlh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2efvsdpql.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yptyouej.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jcvozfro.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qnpqelaw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hstzefqu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lhxysmeu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bysfdhmp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zrtaivuo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pnxedoht.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2crvxqhhd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ixwpvbhf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzkjesvt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2srmshxbk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vhgowyjf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kfvamgyi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2degwbrom.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aeflyiml.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lbccuteb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dtpmnsdx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gpvxqbjt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cyfwrtts.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2swugwlfv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2gxtbpauy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxcyzadx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lgdtpmab.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kilouuxt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wffowysb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwhgugzn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uvfvwomw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2olkijghr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rjjigatb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vdgytjyf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lzsixjmx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uoezhgap.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxaasr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ezqmnijy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uvxldhzg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2alhdkwdo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zintndez.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ouuwawnj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mgokakyl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2exvaslyz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ncbczarn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uaorifqw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lvbbkwud.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ajxfwutj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gzagtclk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofhubbb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2arvgxovw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2puirqqpn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tpthjjjr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2btfwwdet.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ysvoitfo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2aypyveru.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zxsminrx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2muvtcjut.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fkvhuyhe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vwctipum.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wdsdcoyc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gpvopeph.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2drnaobmq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yfaoyrfw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yvxrdlcd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pggvkmia.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2czmzmvmd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ffvobyee.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pgvzbgrr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pixeguwb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivjfsmue.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2miiuenzl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qsbaugsf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ejbyjxjh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ofmvvgsc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vveyxcjm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bbtcmejz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2aewauuqf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2uyjqndmc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktluelzu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wcqixcer.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hvlzuqou.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2erkwlqis.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fqiybixv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2elfyrwbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhnodf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2srcivktv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2eqvhrywc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vxdoupta.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hyurcraq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2afnzdyfj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fkalqtkd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfefirkq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bbxegwvt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xqrtzlnx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ocntufoc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2coznispu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ytwvkijg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fohenkbj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2soaamhwf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mwubtowj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nburvbzz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2elgznfbu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jbxqzueb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wtzgolhv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2upbznvvt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mrklglja.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2izpsmdbw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gsjjfric.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fgvgmkpw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pvafbxmf.html


<!-- 参考信息 -->