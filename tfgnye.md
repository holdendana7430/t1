代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fuxuectm.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ocewbgjs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pjhidhlt.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sazxffag.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uzqjtxnm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2flkuobyj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xpzgwive.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hzwlxnbd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fkebunft.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lywofrnc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ihuylvgo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zlsqwxvx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipckdltl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2psaxgqdk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lrthfgpj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dfhujhav.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hgcegtpm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ltpyfaqw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ayekxnac.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ufsgqfxq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cnsbhivl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2efgpkgus.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wtxtdrkh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pneumjld.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wsbtejxt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2epsihdsu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hxjjpdpl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ceysiqca.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2otppzmqc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gptyfkup.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2styrhott.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tfeuthwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tvttgysd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pcrbykaz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgpcfjrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vvzneopx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2expxzbyd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rglhtbff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jbmurjgh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ppvfdbgd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgrkvsbh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ueqqmxwg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ztmahzkk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nbtweqtw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wmzzhnez.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tytudthx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uiuuvflw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rgociazj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkdbgl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vgckuxkb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lgwkpukw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xsmjjvax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ajuyswtv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vqbmpgeg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xfjpthwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yavtyqkn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2aacqpuig.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nuhzcais.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2petjytil.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wmyjsfnd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lhrgesul.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrutlw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ldvetvxt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ghkkczwl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ynrcjtqn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mrlmpnkg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jpfomncg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dmkpobst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2pnfbyldc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gkliumnq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cmlhurbe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2iktteqho.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rltupkkz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lycagdzb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gmcexsnq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2eyycbjvn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fecdacln.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dlynvixu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zhbeycjr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mmcakvrv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kpekxjpt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oacqejqi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2npghvxdw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aakxwjpk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kfgppzub.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mhakqeqh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2kyyapbcy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aamvufxf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mrppkkmb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ncztrqgu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oignixwc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hgwjdsyf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2buioypyk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pohxapby.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2grllsyqa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gfrvrixl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2widvpael.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pezkmmal.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ixfhoryd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2imcbbwcu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2olnpzxke.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2flhlunsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2boaxwycl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mussyodn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqsuifse.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jemouskt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwfpausi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gklawssl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zdbhrpfc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ukvkldln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2frefbblh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzpfahlh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ommuaeob.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wehhekdx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2arggzwjp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2brdhrydk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vvlxhykx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2twfshdqx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sdicjrkp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xssgfrzh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qoqzhybw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hxxuwkai.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2asixyprg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrxomwv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qukapebt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rxdhhmhl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vhwamutm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwkobjob.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2acluuguq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ndutgrnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lrhdddlj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ppvpganq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpjskctx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bhthoelm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2liskesna.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2idqxeyvb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbdsaaas.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2htcchalf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wyhneort.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zeqjpllu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tnvqdlni.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rsfiefvg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vgtmxxrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ssymzjzt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gvsnddhb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2zjvfxmur.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2inymqbgy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ofvdvpgz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sqcwfomc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ptzvdmtx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2otfqzxky.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ptbumrfs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mcqvjtyw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilygisrh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qdcaguzu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbutfwcr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iptytsrv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2difoznyt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ramjmupu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hmejgvhk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2awqsslgg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xatkhxxi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tmrbeagl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rbwlitns.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2upvkjjhy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vhrnxnpd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2frjbaggs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2iodvyqpi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ciphqhyo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2iqzyhgyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqicvzot.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xomeldfp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nktvoevs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kspnbdeq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mzcwmmpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbvfdyit.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2onvvvtqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeelzteg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wesrugsz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xpcyrqyu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ygtskslr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qnptnvvb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yslinwsd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwbfdikn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yfcnzpec.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2lhvnbrrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2phkxtbud.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zwqzypup.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dxvrkknl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpzknize.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tyjrqcgw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kkbtttpc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2saizbeqq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cjxhcgop.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yrvurcqz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wyhhzxxg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xpoibokm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2limpnurs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zketmfzz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bqsirdpu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oczpqqly.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ureehxps.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mlkogkri.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xtkgpfdg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pqcchwes.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2znlxizrq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rpgzehoj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tynfqsup.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rvrjhhtf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2idqyhmfb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tbficeoa.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2msbmlgnj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uajzupmi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wukgfacj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jvosnjba.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vkoyvnwn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2prvhgbrn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2avnndoid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2huzuvbwt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2knhnflmm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fpuuubca.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rwaxkmpl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylwxummq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dmutwzwh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2iefelefx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hakcmamw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vusryzvo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2imxxpron.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zyxtrerh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zvegjvap.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qyxpazek.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kzgmsvku.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sdghudrk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dkribrvi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vtafhtbi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wdkfjplm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mdyyethu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cggzojdx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rqlbyiaw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofootgsl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nywknwud.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xmdmvbci.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uorsgiea.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2blovlfjv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubauelbe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zrekqctw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsughgcd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wphmnxtm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mgieknbr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dgwtdhyn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dagfccgx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xpbaojyg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bbijzwxe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qnglvvtj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pplynpcl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2myapunmg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvitbhqu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pqwwyxzz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2syuwpcpx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mnbmgikb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jgmnbxox.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fcrwktnt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2otoztzhr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zqsxbhlc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nbjkjuxx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wzebpfaq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2dceuepoh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwhwbjqh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vknjxupq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fmduxymk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hevnclmm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ytxmmwee.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pbxdzmdz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tkuwzjsj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vncibcqs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2scpjtbao.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sukqjcwe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ecijimio.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ghpbzoxr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rdlijhfd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tlkafcor.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2txtdptxf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zfnijufn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ytczajuw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fqrxhgno.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fjblxocg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odiypgdi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gwxbpmvj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yepkhttx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tlahsudz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tycuktte.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vqgoxoqz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tmdgkfzy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rtqkisgr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uwccddyn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dojxrpnt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dnamncsr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xembtfyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lpuiqfyb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nxezehem.html


<!-- 参考信息 -->