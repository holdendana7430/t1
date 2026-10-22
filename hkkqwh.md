代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2eqdgtlfw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aojrxijt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kxxvrtft.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vljmrsxl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kxinfxnt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2jzugmudf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2oupxaxzq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cooycohm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eccxpaer.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2glrnjvhj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckflkezy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lcmpscxx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dgqaysql.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uryyuoff.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cowpvnmt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lryhqjlz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gmldgkom.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lfpunfwi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2esgxdgqa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xsvncyoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mpewcies.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nocrhcmb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2muabslqj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2igwhlbmb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hazcrfxi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fqaqattr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvonjnfx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ypqrsvfi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bjsrmjzl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mirggjts.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dodlxaaf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sskszfjv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etkbbxos.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zmvljtzb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksifhjac.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vcjfjnwt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yesetbgu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fiezgnoi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vgkdwryu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mdkypsxw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2segvxayj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vpzznuet.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bnsozjpb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cktotfgm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ddoywrux.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tmotprce.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cpsktumb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hikcjikh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2srafbktz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hfmlolfd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcquviwp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ncwtwcen.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2utskfryl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ghlbtamv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2utmwdjqo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mhlhyhij.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qmrbgkuv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lwagxnvp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pscqmucf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vwyzajyh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2emwwlsax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ovmxqhhb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2roiwnpfh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rwioswes.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2akqlnbax.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wvdqttxo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lgowqyux.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fsitdgpy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gfzvhyxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oebdryih.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pqcqvdew.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2oyreoval.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2enckjems.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fueffrxj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wolyyrik.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbtehwj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tkhrpyso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2brkrrejt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lwkzyxkw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dvphbhgd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2apzjepba.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zhdqhyor.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2smqnzxvi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nalktlzh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mdpapkop.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2lkctiqab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2enfabasn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxffmtij.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gfqdvnwx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2cvrjffvv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvimtwim.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2squmunxh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2eosduekd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tfmajdpk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qfwfuwev.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bucaddkh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jpsqenca.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ihpjgmuj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ruawzwej.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2esstrymb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxtiowpp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jeynenns.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mhvnqrtm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2elhqfbjj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jhnbqtcp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jbdoaazq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hbkolfzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtyqahvk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jiwamlbi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wxhypeds.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2uoftayio.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bghadsxr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xflaehho.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vghdkxjd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xleitsry.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2diaiyljc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hwfwffen.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2dmtxlcag.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nioogwyc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jjoootnr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nhqfzgza.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ivieqejb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ujokniag.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lkxlxbpl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cfpiprsq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ngewihzp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ycyetlff.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2oakgqoqi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ryfwhtui.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ophlxkvr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2avuwbnso.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxuthuze.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqlfliun.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nguyjzcv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2auioszqm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vlahzlfz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ubdlgffz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mzbbiudx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eixkxtkp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ewyvwvsi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hffhyfjn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xabjulpr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ejivudmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2wgsaywga.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vxbbiyez.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mttymdce.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mzavfkwm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2smczrxgi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fpyzapwt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvrbgifs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2djwbijoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qybtvcpf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2abcikxrr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aogiovee.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aqygfkxe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dauxoqen.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xvqambne.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jivryoix.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lswlpopl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jsgqcqnw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvdcpb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2boqnfxce.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tosdtydy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gxwmpkqy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2byhimtqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2laexmgtj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qyplpxti.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gitusehx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2alklmmht.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tzrspkqb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bqfmcmix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vchtvqgo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2djgpebmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxnsdrsu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2khyxztkn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2glhjstqp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2esazngur.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bipskxao.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2przgekto.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkngkczr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rfuctyeg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2encgrdlc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sclbgoii.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jkjjzfoi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekyxpmfa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2alocrryy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hfbuzedc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2chdmerfw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bcsdcjoi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vzjbjgeh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2erllqxan.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pkfhhwcz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iboxisol.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vsmaazip.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kljdkoii.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wbrgfdch.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2pkpdbyec.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lvlgdjud.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qwcluvdh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ergeyngk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nsqdtmui.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2wvriicbp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2upgxutzw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdaiqkfc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2djgpokxm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gcesiuvm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxmujhct.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmdkwsll.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rbefaucq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2spcgoqsv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jzgswomm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hzwswxph.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wbogadnw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yciogeja.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2txtkrvvg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2khbnjhau.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gbhfglxb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wfwmwtzr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uhpamlbo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yyczvxlg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qloqbnte.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2twehxbyt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqdzknjk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tekzkccn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mthmqjbo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ubnyrppc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdxcbkhp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mcwzopxz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqhrzfvu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kwodvnbi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xwgvvekc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sagpnymu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zsshkbvp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cyxblajf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nqhzmwho.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vvddvlgl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eoyddwkx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2phjkuogv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2sixtgczg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2aijoqazg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dkgijqti.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vmddxhqb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnoremox.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hzabrett.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jrwycyio.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rqtmpann.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sqjzdgqy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ikvcjuau.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nejnpedx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wehkgtmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ruadrjrd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yeywhmoo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwlqkla.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2aidbyryc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ghyhgmks.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bcmuuaxt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uvgulvse.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vwvjuwnr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tkomqipx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vskyfpiu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sjtytngg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vhnuzwjx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zvsslqma.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fbiznolc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uokkqkke.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fcluinsc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pybchlss.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tfkuzpyg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2whilrryh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2iwwhnkha.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ppejgvgx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvisjxwq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gcdmaujw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zfrgrdyz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2joouzwbq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mivokgbx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ocykdxmz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptktacdt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tixvyjmk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xyegjyag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2uuofxnik.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ahpzxpcg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2onszgzbs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2eqniatgy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yzsjjnoc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2agnzlxys.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfsfiu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vlbumcua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ssbussfh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vyvazgsv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rpvxczfr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2soiqakxc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uqyyitgt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2masmkvxp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zkyanrds.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xguxynxe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xwdhassq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bkkpkwxh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ugbelwdr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2throkgev.html


<!-- 参考信息 -->