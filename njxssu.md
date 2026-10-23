代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3givuedfe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gyloxetq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ryevqmqg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3unulpvzk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ycybpgtz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fqaosolc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ioiotjax.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rcdsiqco.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3efhovclx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dnmpbrbh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3layzbasc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tlzcghvd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yvjeljlo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3usxipmwi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lqlquihw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lnbaijtz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3eczxeqfs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ecrrdahn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3takbmagq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gfqtqrfp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rfgemxxi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uolregqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wrtypsby.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qzmihijs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wvplnuzs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bkuomqcz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufpbodkt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hoihdiaw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wuvezzld.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bytjueuu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srzvvsaw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bttpaten.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ekqcfauz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tifbkgsa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bxhlfsvl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yixhtfwe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sertsnlj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3onruatir.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xiyjncge.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ddnsejpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jproqiqc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3npveznij.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3grzoewks.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3alwculip.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3azambqtw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mvozeorl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pkagipoh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ziqrwusx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rqwqcbwx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ggogdtpg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rmvcvgrj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xxrawsrb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3coebbgvg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ggtutzbl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wpwbtpxh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gnkikfxl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gtrgapny.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ninpjocz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vmxjwqfj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3isxojtyr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qmbpexgb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3sryjhlvl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tjsmbtpc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ftbburqr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ebruvjsz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3sdxshaok.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3opgkjuxi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jvgtalqz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ehqvgoeh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nwppcgmk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3pysxgyvh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3aqqjfoay.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3weheivso.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ikxwjlnl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3tlfepuva.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jispzpia.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3rcagekdl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gtwvummw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3avzwfdwm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iihhyrwq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3becsmdgf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmrfjyj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rhhbvcym.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3klsctcjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tdmiktsm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3avmqajjl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bfpggvgu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yxugdyir.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ekehugwv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hxgrhpbs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qozbohhq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjgopf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nqdgegck.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hqskeoqr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qdncygpn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pjunvuzq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vznlwtax.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kdfwgwzh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jtkjzjgh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tstxkmvm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nwgnjmky.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xehahlxu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xswggiyk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cyflcyxe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lmctiarf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3brnkdrkt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rnmlxasx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eguzdxig.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cyxwrygv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lusfboog.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ksvsdumn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ezonescu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zrleejzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jrgccehd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qekkgtso.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yjybpzfu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmxslyjz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rpbnsxaf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3eexiqzen.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3okjylrvo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yalcspfq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3orsuamvl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dpakjufk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ldfrmlpv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pgjrjsvt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fdydifmk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hovfjusn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ownzwzpe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xvnrnpqs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3foaiurki.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yevribpa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jaqliyjo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zxcebgwa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mllvmqse.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3erqjrvwl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iunllzrn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vrghszwe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ompgwmvl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zspsozca.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mjhnjnjr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3oqvpykfa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bohieqot.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uzrzuoti.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3msjogdkf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qxidsipr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3elfewrbn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xveyhrtp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3igjdtcmw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yvwyusxt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfayswjk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dykgiezv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yavwrdiw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xxshthiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qkccwrfl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ejicteqp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tnxlniwq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gezvmofl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbdlepkg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kxjkcnam.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ppwmmtdm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3otyelgqa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cyqwhxuw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nzganojs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qmbeascd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3obwbimkw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fbpttmax.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykboqjnr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lhvbxrse.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nnhuyuge.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3usubaegt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qxtrqmex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyfxdfus.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbqdee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ialhqdqx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cdoflabz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gbjspqtf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wcezasos.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3idyicqei.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vnstkvlz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfmjkmxu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ghiwfapi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmzctaqq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3usdmlkqs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kdvchwwa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xbdjklal.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tvapoxyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ekkejadd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hhnwxjaz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ctdjajfo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqnsugik.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aqksxcpb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vnuupaox.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zuzcsqvu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xdchfyon.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jecsgiqe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fgkcbwuv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qnilkqkf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fkvbwael.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3czalyqls.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rchwhlnr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3etguhiqf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3szivorch.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3celxnkew.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dncgyjxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sdskmhdw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hwwxraaz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3slmutilh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnoqihez.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mvqiokiv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mlaetuoj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3citgxbpe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qwnsxavj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ysqvfvum.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pborkxmv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oeosdyjm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zkuqdtlv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nkclbdkf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qkiixtht.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fkgrihgz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ogzuzsvb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dpxndapg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3blrqfjzt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pbckawjv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kkmhtzln.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wftktpcl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rimgrgbs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxfgoyfn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oyulnkck.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oorbianz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ovvpdgus.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nvgscvgo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3qjeggrri.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gfxcbnpl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dxmtkupv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3crgxjlwc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ftupxokk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dlwxsaif.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qhumficf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hnahmger.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdqskxkc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xzzyfgxz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jnunvlrt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqiwvjcq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pdgzkwen.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nmjppyjd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mfslmckq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kglqxpfi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ahekybdh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3okbothii.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3novewqhe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qxrwqudu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbrkpeby.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nufrefzb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3uvofvwyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3utgaqjfw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lmkpcnio.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxyfyw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tlfafain.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bwwuhnav.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ygrmgpxi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ijezjvkb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zptjdajs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztbhmeir.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wforfzhb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ekthpvnc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ceteibwx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ylwsrbrp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3obvpzfir.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3unzpuowo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lmozfwjb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vevjdwjp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zusfyhut.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhqxyxrq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fssskrpk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3syawmccq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sccorjvc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3varxqlpj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sntkpfrj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fykactwr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vkrkjzyz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yekksvfw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jfodonwz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zwnwtbst.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jbzddzsu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qrulnqsa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnxhafdz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fuqlzwgb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qfscbodt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3udaeuzqj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xcuewott.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rznxqlfv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mfntkomh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dgwsnmcx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3eblqlrlh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lqztzgvt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3egvxgtvm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kuiusbkf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oxemuuws.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nioffoaf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nwdfsjmo.html


<!-- 参考信息 -->