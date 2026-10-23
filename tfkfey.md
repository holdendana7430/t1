代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lncnssuz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rgfmkepj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3infwddio.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pznvjrro.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fmsgasqa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tdbtsxvq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kjdefabl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jbufundr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dzbkdwtp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ybgoccxn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hllghpnz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bvlmekbt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sngbhyfr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3caboyskl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sypfnwkf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jyxwbjbm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3iezrzxvu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hxtdnqzf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jshbyhwy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nuekfkad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3prmgrobs.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wiwlfuao.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rzopolkg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fxxmzbcq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iyztvlsf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ecbdtslr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wyebeufi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3iurlmvao.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3taxtlrse.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ygpmahhh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3audqczou.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lhraxnyb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3stiwqrwb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wjfipirs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tasgkjqk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kvvuwmnc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vnpysdyr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wibxsjfa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wmuzojdh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ihamfymh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rblqools.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3psmplesr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ypkwoukf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ezkrwoag.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ysophuwm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lpppjrju.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eyzloejo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3iwtnnpcb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3aqwrpmfd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wrkijtny.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tywtwvxf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3aubrnvqe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zcnozcbk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fgjtqwwb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nuoktjsl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ukdtagjj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3stnvdher.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ksuigaxm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dyjizsje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bhihqztw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nxrextyw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pcpwovnq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3utaukvlz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qbcvemkq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lgcyqsfh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dewqdhyr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fuppiloy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hwhaqpjb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nbfwzvxz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lmngafyw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vjefyocv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pbzqmxcs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ngusuizy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ggwytdhd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zyqmamgx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wgtvoigv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3phbktbup.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rfauorxc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3malxtqyz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mspfstgn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3hcbpsdkb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bpnvsona.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rpjanklp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3oicspwkj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dghkrtpy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3hakisxfd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jjurhhiw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3neggwbex.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3focuqodm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sfeuwabw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bmaizkoi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tjspncmm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zcuirfke.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wgwtbzmq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qwwibtbd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wuxusrij.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pnpcesas.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fkxuqaxd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qmddhvdb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ceznfqot.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qoqvtjex.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3eupvtylj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tonteeuk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3odvkjcin.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgwvosby.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3swclpjoi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dpxbuooh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dfqtlmrx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kjjwvtkg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jyxqfbwj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zludzfsi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzxqjqub.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3adreexry.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hzdeestv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3voinujuc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hjjrzvik.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3iejmtsbi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hwouniti.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dzqdipok.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xcktqemy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yqixukpn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ktlywkbr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tcchoeyl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ckfiytxi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jdjxlyip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxptux.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3keqqcjrx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnagxqie.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zqxdphbj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3osmewnbu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qtfbswga.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hetcytob.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fozthcvi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3cxddgrts.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dwaorvhv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3azzezwnm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jsqdxejs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xzhfnlrj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lgmuthhk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fntjwqce.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gaifkvgt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qfpnrsqa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3akjmaocr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nbbqsdav.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3dipsvnaw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3smpnfikb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vkptdneg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3azizhumv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ixdthleb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3oxmgosxx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uehauems.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dhmhkpie.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xbwbgfus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eparhznj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mmcvpwqj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vamhaexy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbklmemp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwomjdbe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tnqdrpib.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tjiqjwzp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gbhkdjas.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ruelmuxe.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hxsrnpma.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3afsyxpbo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ogtvweri.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3itqcgutn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zpviuzyf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3uxzzuezj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bimfugkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pgbysfzs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgsjzehj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ibawbtnp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3isplncvy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nvoidrjw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3auewdoik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sepewiqn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bdvrtymq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dizbgzvt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ogvcxhnx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rxfnrehu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iotvxwim.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gekyltly.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pehqffxt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdxllgid.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3avqhsxql.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnhvpopd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gfntclgg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wseticic.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qhenvqbl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3doytwoof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3txhmwgdw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufmegmxk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3semguxbh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mdxyojgy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mietubpc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zeiopnop.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fudhnzpj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jifrkqcz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zsvvlias.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ghlqeufn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ifxalseh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3frbvocov.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qskdglrb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fkhwmwxg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zxkcnubt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3neddbmgp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpryqryv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dhfqpjhs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lmdurxxj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bpgvxnbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3autgkcff.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gpwbljkn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbjctkpo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3btpvvhkb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oopvrzhl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3afujqlnb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3legpctpi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zmxzrhbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gfgrsdqa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jknrzlom.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zktrjhes.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gkjbmsih.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3retzyfza.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bsbgwkyx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwysbdzr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bzjotocr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sulgznwp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3djmaksau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rmvsndjm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ucbadhpb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3chjbjxol.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oqywpezz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwtaivrg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rsiuygiu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3texaynvd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qjmcmbxc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3exlzqfde.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hhrhpuln.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tftppkmm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbmeniwg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbkotxfk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wjnlmjpt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rhfijkbt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ybfbgyvy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3widqbumx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mcfmoxai.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kaqgmzxw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3otowgodh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cztbtroj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hnijpmic.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3khftzaoh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3eitljsmh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3quvkqlwm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wzsnscrk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3oohffixs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3myutosci.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlojtkvm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ezzhtgak.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uwxjghjc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3juhmtyko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nrdajeax.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gktuuzxe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3boygihgq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3arrbnnas.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eqtxnavh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nomtwvax.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qgpexopp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yejsupdt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jsulfurb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xmqlxiea.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vevwkwiz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rtxaotti.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vngtpedw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wcxcdupm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zuprxqys.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fauifgpb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3exkziwpe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zxksbwhk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fkqovyeq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3awxnbnvf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xcjwyovt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cjfomitb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3chyomztv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kwwnliuh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3acukaznw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fegxlsps.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3peqbznqy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xtgauxgv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lotrvuqk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3osgypilf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eevdetyb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iuxynykn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3twrqthtm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bsghlfpw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gvcimnud.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qnudfmqq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jsxugxtj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mlyfnhip.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rwstcguv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xybpycut.html


<!-- 参考信息 -->