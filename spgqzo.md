代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xbpjyrne.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2sndjrlku.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2upnapblk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nkpzrmjd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hqelhwii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2jyoyazjn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jjqkooxt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ekjvhdtv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qcibjthe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2njijzhsl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jurjigur.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jrwptgxo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfiixfin.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nsabikvn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auiqybxi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lvhgltzq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phknnhrt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jzwsonve.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lnmocwuq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sfguqsdo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dwayrnws.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ajeocgvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pynabqwt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2uycoazzf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pgrgqowy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2otozdfui.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nufjrqec.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jplltiuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kyubcwbl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ovfbwhxm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpahtedt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wzmhlzyf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qsewuwis.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yjqrhqdo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2apzdspqo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2heyywywp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqcttqdn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xifccctm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxtajikm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ispeshls.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nkazwasr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rcgkbsyl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wwpaqiog.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vthauszk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvpqnmm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fzjholht.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mvklncmh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fhhyexla.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2goorqcwt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2islpjbje.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2edrvjarb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2trqwuphj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wzvcbsca.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hcxyofea.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dqmnvnoz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wxawxauj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qsdfvujo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pstbibzp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mtvzesei.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jypwoixd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cpcfdhua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dmnbcids.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zjkakrmf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2apjquspn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnxido.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2klpzhoix.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cbzsevyu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hywcgzic.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ewgcmykn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gkncdlna.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zyalbiqo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ooepwatv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jsintixw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yelfocal.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmxcpdxl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2phtemvfy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ycffvaqf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2objulwxg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dkoddjun.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2temvdhrq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2binyrfse.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2scalmfew.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vcgnmoyg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2duhdprng.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nyzcicty.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cqptzfqr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ymvykacf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rcgwjndz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jgnqlsew.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xxfehwtx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgufhv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2doulfqyb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aimnyafu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xhhnsayz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2esfpveaq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kapjefao.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qrkujivd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cgpofofm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tkdwgikf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fexbxzgr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dhbklmot.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ljohlweg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pgmwhiik.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rswbhiqp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axugjsqg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2odbmbhix.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2axeyrtdw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tdemfjvs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdpshzgk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lhivsynw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zykcmfqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wwfeyfgh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xloltjpk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmsudsfh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fnnvtpmc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2myhtjkcs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2aqzeouar.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cnnyblsx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ogqzerut.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2edkuuchy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gnatiali.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hytseibv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pyrulowh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2edaqiudy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vbuzeidu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vhdyjdsi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ehonlrmg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jwsdotmz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mwlviheq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sskozuce.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zehstjph.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xnefidli.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ezvmidtm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yjxlhual.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zjdmqrdc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xjpsursi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iamxqatb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2owyvgqux.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nesmwaxu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kqhoqjvz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vmmulish.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ppslwwys.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bunlpuum.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qlcpseuz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fnppbvpn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uhzpavae.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ghgtiwwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rowmexac.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yevtguwq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2enujpwmo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sfesgzxl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wwbnvikd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rdwxdddq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xgzxhsnp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2osrypkhy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trgfeyqo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xbqpnhdf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hktryaby.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zzkxxaef.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dbfhpbbl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kwlylypy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqifndco.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ymahbsac.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvcrtw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhiipw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wdsyyvdg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ilhiikyn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dkpayejn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eoxseqxi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kljbcezx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2geafawtf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2unoqzxxg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yhdrmdph.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2symrymrf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jedrlkkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxxxgpuj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wqukuoro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qznqdtdo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ulhalyto.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2plywfcsx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uovcybro.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qlypjich.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2atdtzhqx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sckeocoe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wuzreppo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gotstgol.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2gfhluytt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hmykxzkf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vyyssxrr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rktjddxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dliincoz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtezdimk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mdpglxzv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2idybxykl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rgiduohf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgpknzbb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jsrrhzue.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rhmdksac.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cqbhmjer.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ngnwvwya.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vnkriebn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dbqyerwq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2srhnntnu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2voyfqjcn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ujyusdpz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uytkdwem.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2czcargfj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxnjrgkz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dhmbfmuy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2gtzebrch.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wtazmhog.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2arsltgli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vrispnbd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hfvaqwbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hdolzbga.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mzegfmbh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yhqhwwey.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nanjxtqc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2irfjemoi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tyvivzih.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcgyovdt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fumqmqee.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2emqhbzem.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2alkbycpu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qgjdkrok.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tljydwbi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjgxuxld.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ftkauejy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mxyurdpj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rlnzomkd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggwzfosk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cptnwaua.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2aosxodkn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vlbunglu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vnmvumrj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zrplpczt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aepeuirs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2oooxmxlw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vyvwuvfa.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbmblbqp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cgenwhdo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jsoqrggy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ffwhkjlh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lsmcmuua.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjrchna.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rdkhmsii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uegqghpx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fskybpsk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2guonqpav.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kmtycbct.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2chdcokxk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rarizijc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iyvzkgse.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ntistdza.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dowdsjoo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2atmhkduw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qaswgczh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gfgmjrrl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qvdryspf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hihloaew.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wznfanuu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zojfujzl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vthzqoya.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kbebvkni.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xaokkqcm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gugrhxgn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mnzkxfhb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uauxwogj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rbbkyzkw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vyglhtwx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ycprosng.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tzadwfsl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ugnftzkv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lgakjlnb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cnfjcoxe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2moydlhnf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwcczikk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ywopaekk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2evdlwnnn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ccyhayfl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gzyyjgbp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lpurokvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tykodixt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qrsudrzg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dwzqznpw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kdtibjsn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkdnkqdw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kjtpvtgt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uilmwvxc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zprtundb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ilqotwzo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rlwlibcc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xnvpreyn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tliczedt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wxdtaylk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qcmnflss.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ydnffjyu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vvsuenna.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qeewqfop.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vkawhzsu.html


<!-- 参考信息 -->