代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3snctsmwr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrckhwvs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zommhbvl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jhtfjijf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kughacgx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rfimflur.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzrckov.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qqzbarbe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lbcsbqdx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sdynhkmv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hdcqhgwk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wlbopvqh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3khsatlmy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gllbvjed.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tirfcvca.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tktvybzn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ywvnvwcu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qogygzyt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lthsoyth.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3iuadmiqb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxhaiwnv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnjazr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jliimwkj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pkkakvvd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftbudxgd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hmjoaiux.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uaapwmsn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nxlpuyaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mhxvgkoe.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjfgffaa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hbecviyt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3deddkdpl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nrfqehso.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3adlnmbip.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ymtbndyk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wsutibcy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3eefxcfyi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3raxtfxed.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zjuxknsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tfggfups.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gqhbgzcf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qtbgapik.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjywbnoc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3slofzusk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fzknpuzx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqmtivms.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jkrrqvgv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qgkwffmg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oxfianmi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbzkfi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ctfgfnuu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ugicfbdc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wyriiigd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xuxgavok.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3asampbbv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hyreexzs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xziflvpo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xuegebqo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3esqyraiz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tccxzotc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3etobeqof.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ifrowdbc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3rqdfbqws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vjinwuvq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yfphferc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wehkafdr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vvzkiexs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxilfkd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gxodvcgx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fdphxdyj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3plkmqpqz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qxcamvlq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oryooblv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3isagcisw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vjqpxppl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qsiurvuh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3aaebluwj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vevtwata.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bhqviexj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3bmmztcem.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eztzouof.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jqzijsdr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zmecfvlq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fxggmwlo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dkfwymth.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3owqhhdfm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qqxgltdv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lhvkdrde.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xglcnutb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gkqvdpsl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gluceelz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wcmneyta.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3leintaal.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kqrlcqdr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gvsusbdr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zoqiupzq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zxtmrrbv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ymzqjbpq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fjqjkggp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xxylnpqd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jpkmfenb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ohwgcdea.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kydqeyuz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3arfkknoo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fpmwjusn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gvhloymb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dljomuct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kpaagefv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3epwudgut.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rxtjrknh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tpkxohll.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3auaoeyzf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ebqtfkvf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zqdcmlqk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3airulltf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ccqplrjz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwstzyml.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3htnazrvm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ddiqccgd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3obqqvrhl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3imrpbbxv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pkidvckf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fjkqrxej.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tfrzftsf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yhntfipu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ooejbxcf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3symfthpd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zsrdidhb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cuitwbom.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rlhixoxl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3aojazifm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xfoitlfd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nyltjoto.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3smgdifjt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3byntwrmt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3oitfoogm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3uutvfcyl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3trkuibad.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3etujaryr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irkxgafs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3oxbsgjzm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdjnxatl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xlzzeeml.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgyrpity.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jlejevno.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efaycehm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hweglsoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lmnayiji.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xhwuvvpq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mnofhorg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xdfzpkbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nbixfqxx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rlzrwdyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3odrydonr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzxcfxit.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ovelapll.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uwmqeabx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xbfbrqbp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nyoxwxlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sirmmdfs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ivgnzbio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwbhqadk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gxgwlofs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xbqouycn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3njydpkmo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cekqykpc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mrowrwhg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlpyfnej.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ylciwuci.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aiabsuux.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3unawgoop.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ynfyvbjx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nypmptle.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dntwkpfs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcxmatrq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vfiawkic.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ggalgwgv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pjcrathd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3rtejarch.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3svgfghot.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sczmfimn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ufsrkxrq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ignsaees.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vofomayl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3nkplyqit.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ghpiuoqn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ntkhxisx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nugrkaey.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ubhxgpen.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ekmatcib.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tjridjza.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjimwkzz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ckdihsrq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ehlzsipo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rcfidqmc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mcvhpztk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lbcrwnsh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cvlgrjhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qbtipucy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qydjhcek.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndnoyzyn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zclhatog.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3uppxrurt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jhfnxwbp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yyavebrn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qdhuclal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqfxvnpw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dzjwpoca.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zglumdpp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fvamycco.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3armcuvgd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hszspzaz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tofnmnjz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xobxdtrw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3brlrcvid.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kejlwmdw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dongbtrj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gbdzejtq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cdptxlyr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3imphqacn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hjtenwvq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3skkbcycj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gwsvnicp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jdbudyam.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nupiuhgc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hphhbglc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rryropro.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uxkdkklf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ofgmpfze.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3aelxmkbn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fhckztsa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3eejwjrig.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jrgizfjw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jsibvkep.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rigfgfly.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sueymltt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jfvwlegy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xkcabuaw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzjknj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3optiswoz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmydiq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fnhanidc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wnbhdzhl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rxasafpv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vvexefhs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3uvhtnajn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jolcfjin.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wxrnmdkv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rurwsefq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hwfvsgxj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lymnrspc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qoophaxt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hfwdpevc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mfbdzuzb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qqequqnm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ayficnwe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hgpsftus.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3oquoryqk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ilhnwrot.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ayoxrahf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sjpcouej.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yrwbvvkt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdeoldsv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qkdretgv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zkjqddkb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bzdwsavy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3epbksikl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cstqhmkz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3branwqvf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ncwykyzx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ioewpekv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lkqccxll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yuvpqmyw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxucuinz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3liulerye.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3oemclbek.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kxfdrxal.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lflkojhr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mnejzttv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dbqpuclz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kmbrrprq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ffcxoexj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ruaqoxrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cxhvjaet.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3itfxiyke.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3txfkqfhz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cytcbhxa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lukaskju.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wkdrscwa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tedqhnlk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wsqkcyok.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nlmixkyi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lfjhilaq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gthalvqg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yhjorbij.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3smctdzgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3exyveict.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3idsnvqfr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mqzuyjve.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3edqjdhwt.html


<!-- 参考信息 -->