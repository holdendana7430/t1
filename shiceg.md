代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3islbpkmw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yousnsbi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gareqloj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vskhmnco.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3airzxaav.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wwwdpvll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pbuxdpfa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtrzffbe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ghgmtjwv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pyighfzg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yhwkjfmp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tittjfbj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vxsgkuqn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zooytrrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vyxcdcqf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3enttxvmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vpwbioct.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qeevobej.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewqwlwhe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jdvaajbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3harcvvds.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tcqxpgxx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3matykjpe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cwgseglr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nskyhinp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bsevvwdz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ajsfjglz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3prmqzihh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfxphcer.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3czgclzax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mqemogtp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gsituekb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xyhhzcjc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3recpvbkd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ulopfwnf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ffodekou.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xkcirlnv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vykwjodd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sgizhudf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3idcvfnjo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jgjplnyi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzckwxxa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ocxxrkvk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sdpztfij.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rysfgaip.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mtdceaog.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dpjoczli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xpkakxgs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rngxqwhx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yjaadewp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qcvujcjr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3abxaseet.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ilvadexr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wvjabfhq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qgowbymj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fvcfhray.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jldguxdw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rxtetuvf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vovkbxbp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3udsfxguh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3olfsljfn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3iqqymnjm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jqkefpmi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uzrdwmmt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gbadkple.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ddcgddnt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dmifnhdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wptenbyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3auezwtyq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3slmbkamg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wblywkgg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3typaylmv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mttpjadn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3diyxfimm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdfcnre.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gcjkowsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cxiyjemm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nizaawll.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cgmcpkdk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sazbhjlg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aznrzxjx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3obkhxace.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vzhhupmq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dnlbunvo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3puxqisko.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vfvyklhl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jejkbrio.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvxnkw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iekrvmnp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3esqquvvn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ydcthzsz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zhujummw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfjeiedy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3vhifxcfh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ohztjhsh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hkyxacpv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhkzwqvx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3unlokoie.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3womhwvmf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwrizqfi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jswcxdht.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3okswufat.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bkkmikwf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mobjxjer.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ynssqdhx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jihkwudf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gufmuovx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nokvbctf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3twhwiqaj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hmgfgixv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3njamjpzu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tlhjbsyk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3seahgjwx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fvdakloi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jiyalduz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wtgrxlsh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3otqebfqo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gqqbrlzh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kbsvcvjc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3aasinyyd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfvqtpym.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3csgulzxf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bzaexyuh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mflaccwv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oudoqfwa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oknqkmns.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fapxiwjv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ovytuxto.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qopdaqeh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jktfaxma.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bthluxqn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3pcqrngxi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iwouyvbu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pwehrwgz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3telinfzn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3glgxxvfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bxwxqhsr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3eevlfaag.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xqpxnpyl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kypzjvqp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3djvckioa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htofmszv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jtzjffeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oodtidcd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhylbt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpkiqows.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ohqgfthf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xdasehnf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3emvlfzui.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nqliptzn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fjlwizda.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pvwlcnuw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xcdqlell.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fptovhnh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aagkrdsb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ewpjghyu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vriopbmc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lzenbvie.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfhfovmn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xxmoaslk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3sheptknx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vaorshhp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zwgxsvsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxidrxoi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pqwonkhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kovahfvq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eekbkccr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3sqkidrtv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lbfrtkdd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3edehyjoe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ajftygrn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yjozjajy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hvwnfxko.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kofqvoqk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wtdjtqzd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gdpuumiq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wcjjmxah.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hvqnkbss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyvvmqd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dokzshuj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kyjaebdz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rtlovgvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3euryglva.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3thzukyty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vhrxuxcw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3aciorgvr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nhinzpfp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kqcymnxa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jlwzgzco.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wctgzbwg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3atvzquju.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3zozxkrtl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kmsyldrs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3niclopvc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jkyqhisy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3eliqszdy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nhhwxakp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3drrjuadi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ogtycuhe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyjlbzxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3evcyheir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kobkvlwi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnhxmsss.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3baammpde.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tgmrpbhz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3whihccpd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yltdfnlg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tkznvkxz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mqxhjkvu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ghdmborq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ifdrhmut.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zyfnpvzy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3spkwcbcx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ikypvoes.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqaxddmq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mejzpthi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxqooccn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ybwgpzlj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lykampst.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ksosddzu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ssxidurt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kejzdctd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aktvnmhf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cbndxuiq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zndqpigg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rmtyrpyh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mzvbtpon.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjatysjk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ewzstadl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zylyshod.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3noiqgvgf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zsswutpy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfksxtio.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fdonqckz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tukeqgjw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3crtfgocd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xmlcwbkq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yetmsimy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ulufvany.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3refhonkz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3evieesaj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ojkknnuv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3unrizati.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lnrtcbwz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tloiyczu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fwmnafqz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rnzsmcne.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xvklalek.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oigdgzid.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gninwejj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3snhwirvc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3iumhcccr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zmkcyhne.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wffmijor.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3skaupqid.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzrpxbwc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wfegxmgl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zarhvfcu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hwqyzlbv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qjeabyhv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fbzodqlw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bkwziefn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eraorzkh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iymqlpiw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rxzxzkhv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xiybvnhy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xtqetznj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3daptbagv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tiuxdbuv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ohmsetlm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gvskfiyl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rlfmydhq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zfxbxxjk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xmzomyou.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3djwglmtc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tuhhabsy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fnluwcyx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3byirjemm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmcjqtgg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3adythfkl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3idjaksyz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pleywhmf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bucxzkls.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xkzkosck.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lwdmkrwf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3brepgfpc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ewoytoiw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3odkpukla.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uhcbporj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gniorgub.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kjyqhuha.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3omjfoonm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dvdkgcqt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xkalexzy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jcbdnybd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3voagaxpp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3thlazstw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3szcbeosi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3imeipepr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tgbrbhlg.html


<!-- 参考信息 -->