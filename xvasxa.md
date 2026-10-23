代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rhnpbwjm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vduvmlwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cnvvdtgg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3wczcqsfz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umqdusgm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xvremgpy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwtldagw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3votzjldu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3guvoiouc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aytzgcgl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hpyoamwb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mfstfrqg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bzdfnrta.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3whmfxnzr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3moimzbri.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tsowiqpy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fukiwzvy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzxrlmmp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3eoaeebet.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bswwzrdu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3laumnkrd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3swzmulgt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahphyydq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pmzgyozd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vnulagua.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xhwwgjdd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bruabffn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uqwquird.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqntwbco.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3katqdvpw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrtbhche.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dfgjbdsw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctnyyqnj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ajcwxvbm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3foatalxo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmtird.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vauxxjoo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ireliijb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xqvkrfxw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gyruhdtu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3huypnjgf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3adofbqqr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ucacloly.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fjzkdcvs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3suokrfdb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hbovhzib.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lsxqpurn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qpuwofap.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qhmmokff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tyzfshtw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3obakgqeg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3wlxnauna.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xrwxdjpt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3apjbgopv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tbcrljcu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3iaryaedo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vqaukhdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tgzmbcvt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mcfqmflb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3opmqoayi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cfbkqckw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3muwnrajj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zyejobut.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fzwonmzd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qknjevwo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ymbdixoz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lurvmzkf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3htaberji.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cbcndeyv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vyzvzmha.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zdabbndj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ekyqpafu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdiquhil.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mshwmczm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kxkmeknn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3urqbygqu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uuusznsl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hddyibig.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cuwqlfxn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xwtsgdjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jeltcten.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3guqcjggp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3unvkufdm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tavbpyms.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hroimmws.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3zzveesuc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tspbyfck.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jnqzsenk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ewuqbbbq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ubblxjyh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cuttcdyt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uacextuj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qorptogp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jdwbavwk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pcfqfutl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qqzkloex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rlwvlexx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fmhjeizu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ejzamprp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3itewwzsx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gywkkgpe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cfdnztjn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ylbimhbt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3topzdbxq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dvzxhjwt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lrdfhvoo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ipuubqgh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3otmreetj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ihdvjfzw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jslmusvd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zoaumhtn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vrdtlwdx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cvjxmwzo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ogodkdmc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dcruwmuj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xfydhxoi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dvzpewlf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gtjwjufy.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bxuonhiw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yjisqifi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3abcosgxz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zhmpugxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jszdjczu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lnycntqk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qjuhkjyo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3piphiict.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3plqczcdf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3osajilpb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fenmqmuv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3iildevta.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3codsfmcj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yyhbxruc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kqhrlfvm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fspuscga.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wpflzmtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3legwjfhk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dirusjne.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hvxdjmjd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xhkebksb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tkqiffut.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fxvpiaez.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vxfayyqg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mrlfzepu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tunpmexa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3erbyxvmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uevbukvt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbmudi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivbpobib.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pcqcusfe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aamohexg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lzczjhnx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igqfjcrk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mqnsewkq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcgvsxcj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kurpflvi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dzzlrdmp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3czdvsood.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3eiildjdn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ybdrpgqa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3umzlojal.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qfjuauzb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tfenyvws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzakijqa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nyttzjka.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dlsnbgis.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3yhjjhboo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qnwxpkff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieqymxub.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ewdabymc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfiljlur.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3iopnsryh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3otuajijg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wbsmcqtb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3velxgnyt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bxwlkykn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bagfpgjr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lonywjfp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gvyablbn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ttzcrxoz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xzgpbdjv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxcoxtlw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3oizbzwon.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cmtdcdbz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dualoddp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xkljszyq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rraylhwi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wuzcpiad.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fdefmgrp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hcjrqcwa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hsgnotpt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdpuqxjm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jrcvjoaj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wqkdfrpv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jgvubkgq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cebtprml.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bmnkxtvc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nyjlabwq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3asfdcqcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwjbmwma.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3flfijyzd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dssttewr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tatgmcfm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xgaxrvcs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3douczjjo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3daipkbvi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ypvghvkb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3svwnxidk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cpdqvdls.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mraplbmg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3shmcgmze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zdxbstyv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zchoyuaw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3khbiivoc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3korvftly.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewhyqocf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jarewbmv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjpctvwe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wjeqvnek.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jdqtyxmd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nccvpgup.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ireflwir.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hnumbafw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pciffrfv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ncflbucc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3xqocvccc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qtvwmgcc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ojxbxgxc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ibowdsks.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nibspabp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3swbveubs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dcywbmmj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhrnbhfq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3akcpgeyz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zoldmvfg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vxakfhwl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cuwoqakg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3szgxmtkz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cvhfkuht.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3clybdcrk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3scdnoshw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3urwgmxvk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3eqtdnqql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xzvhfnxd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wwsnlesl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rzducxoz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bqrtwski.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qewcnorp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bhggmkcv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eaaxzvum.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gekeqony.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mjfhgvmr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qzypalky.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ctnbsgwz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3yxswpkea.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xupeczfv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vkxqcmeh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ebtyphfl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vgklxoee.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ssiaypoz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3smssymxr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wzagwysj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bdummqxb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hdcrvxid.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fcarovtp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wvjkddfm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vhljwjcq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uzdeyvor.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hwuikofe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kinsixjq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ptfvvygg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrvherne.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3csmawmro.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3puezszft.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wimqsmjw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jejjybqg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hjqdrryi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dmgkrcsf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rxmzbiqb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rrohwbzj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vdutujma.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zjfknesp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3feuyjnzt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqbyzerg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pclnkjxb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pwvnvaqt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3viosbnkm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vavwmtgn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hfsihfln.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jvadvxsr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xpipnnlu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3odthcnuo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3avdftwqj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ukygpioj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dshyctix.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kfuhkscb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wuszoxux.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vozssmpt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lhhdmmfk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xjtgvfnp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vlhybgqk.html


<!-- 参考信息 -->