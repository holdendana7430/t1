代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iwjmenpr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2niyklmzh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rwvywlvi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2westbnyq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzcdnplq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lfnwjpgm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yswjupns.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fbhvcmnz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2oruqtsjo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gwtexbqm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hkihnqyc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2aeithucd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2btkofrcn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jhsacnwl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2axlfpzgc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hcrwbrrl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lyicychf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vkxfglbd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tqybockn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2csmhdrhs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pbvczozi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jmyuelhk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrpjqsdx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mqvoynpg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2acbefhmb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2afipenzc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qerxbsgz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qbkhmmmm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yfawulwu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ungyxmkq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lllkioqn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mncbqcxa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckbupvph.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kfdqqjoe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gxhgimnl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gcusdvjk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2iqtsfgjj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpensqbe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ivfeeiax.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2akgwnhrc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2spfpzkjv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2btlyxnoh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2brbejjsb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2maxqxkot.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2johgdyqm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2opipdwbr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2poxdrmws.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dkzxhgga.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hpzsgihy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2weplauma.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2byanhmyc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cqksftyw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rzozlbxz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jssyhhfd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2feogvhsz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nzvzrmwd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vuxaggwj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wiyicxtx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ffyfkkez.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2sslabgju.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xgiqbpml.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vrghdypv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2tyslxoll.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2beeonpir.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bgdilfji.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gsujvcxp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dmafgjzq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gwblwdeh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2picioock.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yhljttfx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xjbziikg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ucgvfmhs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jqgvnhld.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yowsnsny.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jbasuewd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rkekkdmx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wayqgswu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2smutsdgd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2syzfjiol.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lcfzlboa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2glojbucn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zacmweoc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mvyyfxde.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2satkrycu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2srjdpcjf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qvjfxdpm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nbiylboa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2uelljslf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cpbhebqo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qdcjvesp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2asyjbkvf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ogblfnui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rsrawpjh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2unphkfaq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yxawtbrz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qhxxphiv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqdmbeft.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xyhplwbt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bmwbwzll.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2atbibkfy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ipsygkrb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2duuiwuko.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rjyoadkm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcgxdpte.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ictaqobg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uwbquyss.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2klzyqtqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vmgpvqrj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xyjadcmj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2krqnpwsq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ezgsuhwj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hdtstalb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yacdhwgi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xcdrfpkw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xfpfoyvx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jmsipomx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mcgjdecf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ziuwqnbb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2dklufigj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbshoxwj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2habfrjaw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lzwhbkzv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2uwaukanu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bgkcqylm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zoqxoasq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wdqjislk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bvveqnzt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jifrlikq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clttoisn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xzttosqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mjphwckt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nvzhnfkh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tpfwhlhl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pbmtkymx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oclpiyou.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zisldvgt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kzmybqjs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2piheadru.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2naynzzcx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fkrvjqfd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qjxoxccc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rbihlqce.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdsfww.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rvspxyii.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xzkcfxjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcmzqfkk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxkcsuux.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hecvswjn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2drgpfyzb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sritckvk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cifevuig.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avylkdzr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yhznrttq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2afmqdlah.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rvuecttm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lxfdohoo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kancogop.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vlmqphbz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nviygwhv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2arncnjix.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ldtwcmvw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hsmvavkv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opvbmzhs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2epzbxwef.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hwtcjeft.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pktombdi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2czauzuxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stpsgfhg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mhewvzge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqfgfeqq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mxdesgqp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ssolvdrg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wfgneuyg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qahcofuy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zyfdwmcy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nzmnvqvg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dqmboubs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nskgsece.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dwfueeyb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mhknikiv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pmlqxjio.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2swfrmswi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jpfmtdhe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2exbxqzfe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2efzlnghi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aamkkumh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2uewfhuvq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2muolmndy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bfcpdooc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2huscfsch.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hjrnngnt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rvbuloms.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vprvpkhm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nimkipyp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pommmaoj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2okzrorfa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jvzglwbn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsovfilx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2scfiqsip.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fwrutbjc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ychcjwvu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hndlbjij.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pdjohipy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2snpgbypc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nkqklbje.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nmtebhrn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwlprlpq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yfbzsktw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aoykyfyq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmcxlnsq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2thloafhq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xllrisvm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gouzfogz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2otkftuhd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2iwdaxjae.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yorcywom.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2atnsylpq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rrfptmls.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbbxgfrn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xxowgtqp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdyngddg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2npwzxczi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ztqnrqpo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fmrlztsc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ppsefbke.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2brvtleey.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xphdydvg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2eewkmxfh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bmozqiws.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hiyxlqgh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kqiuukfp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kukfgiha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fjxticdq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qlpyfenb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hysbsthz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tgkmftku.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnsjfzxu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kqhjxklp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qomrroik.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zzmyclcl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cznomhlf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2iirfpcqx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dvjxrdty.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2liyepnpq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wqnzxtem.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jtgwcnjs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bqajzaoh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wvrmvpsn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fwemtiom.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lwvclius.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rrmhbfom.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2enjvagpz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mjriuleq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kvumlyjc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iisaqvtu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dflqljja.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mdyfosaj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2uywhtzll.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfcewlfm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpugpkoh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qweifuet.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qgnorevs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cbvsocjc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ywrxdpxh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2orfspbxj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qxrvkols.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2iywhwptq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wclitdju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzpniknm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2idzaveti.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odhylyjk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrhdianl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bbfbzcax.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tewepicu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vinwnhss.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2knejotib.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ipcahyxf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cjanvuit.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gpofrvrj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xopdncno.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2anaxkkeu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ucskxtsy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2szwtbuzu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ibkbuktl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hakvsicw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vtoxcjqv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ceqeidws.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oondnzad.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ewslqpyi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dewvqkri.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2woyljhqn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2klnqowyq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kacyakmn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gobsawus.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wiguzahe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rgdflsft.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rhnwikbx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmdkgjfq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bqpdtrok.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tcmqczli.html


<!-- 参考信息 -->