代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daria6918.cn/gtungnhpoz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.dashuyun.cn/gtxtxuunva.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gtczbhaybc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtqchckxqp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtwqtjtkky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gotoacloud.top/gtviegmihl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtqagwnoui.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hnxiangtu.top/gtxlhtgynl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrctlgcqu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtruqllibx.html

================================================================================
来源：http://hz.sufxvd.cn/gtlfkmissz.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gteykginju.html

CREATE TABLE users (
来源：http://hz.aibaodan.cn/gtbfktfhdc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtppowmane.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gtwtbtxjsy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhixingplan.top/gtrafpcwwk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtlxufkuzk.html

);
来源：http://hz.cheryme.top/gtgginmojp.html

[Q02] 创建带外键的表
来源：http://hz.jyoumei.cn/gtynbanarb.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtaegfkgjo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gtjxvtrcbp.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtzszrdfmj.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtudfyihyq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yongpay.top/gtmsjprmzu.html

);
来源：http://hz.jinghuilouyu.cn/gtaidfwckm.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtrozubzsq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gthrilbvno.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtvzzqxqpl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtczdlcjwn.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtxbydalvs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gtetkoucyz.html

[Q06] 删除列
来源：http://hz.jlsjyb.cn/gtxfsyuqqd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhixingplan.top/gtjbobyfuo.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gttyjvgqmv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtkjmwsvkv.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gttemrqpke.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shzxlz.cn/gtcuhuvaeo.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtcwoogezx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtpqkomwjh.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtbatnkvjs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnxiangtu.top/gtfcdmthzy.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtotfenzzp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtmqlskkmz.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtmebrjnmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yueranfly.top/gtxkeeanrn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gtiqmhvvgg.html

[Q13] 忽略重复插入
来源：http://hz.c1oappe.top/gtsftoajjk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tianlin.xyz/gtdexeuvwf.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtfghunaet.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sufxvd.cn/gtrpbxjmbk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtyvuyzwni.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtoooxhfxd.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtskbnwdtn.html

[Q16] 查询指定列
来源：http://hz.sysykeji.top/gtkmkhiojt.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtiirrexjo.html

[Q17] 条件查询
来源：http://hz.hammf.cn/gtborcxwrm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.kuanghao11.cn/gtyfbozezk.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangkeji.top/gtpuhzlqag.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuetiantiany.cn/gtuzpdtmbw.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtpdpkpvxa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtvidhaiyy.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gtirxzmvgh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.meibo888.top/gtxuswcidr.html

[Q21] 空值判断
来源：http://hz.aizwys.cn/gtnnkhmkal.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtcnbsglko.html

[Q22] 排序
来源：http://hz.aizwys.cn/gtnxjypvfx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtdfzqzjxh.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtilmivdio.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gttxhmxomh.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtljjdzeqi.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhaomingkeji.xyz/gtcspufhxx.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtelxqhziy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangshuangyany.cn/gtmftyycge.html

[Q26] 计数
来源：http://hz.chenzaomai.com/gtljpwzwrb.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtwvyaynyj.html

[Q27] 条件计数
来源：http://hz.hammf.cn/gtjrrbhbrs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtpezolxwo.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtxulemldo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgfzy.top/gtojmophpi.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtqitltitm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.meibo888.top/gtpaegkbzn.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gtbtrbevjb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtgochyjqq.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gtatkhucqx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangdashe.top/gtcvfrujeq.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtwtztynvx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtbdngnozn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gtrwfxscfn.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtkivmpcin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gtrflljkww.html

[Q34] 每组取第一条
来源：http://hz.shzxlz.cn/gtdukuaoqs.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtuphrtoij.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tanke756.top/gtdzgpurjn.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gttpadvgfm.html

[Q35] 内连接
来源：http://hz.zdqjudy.top/gtkyakhhlk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtfxemhqvn.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtbpddldej.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtjaffdvqj.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtggeidpva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.vqdsnc.cn/gtstkgvsqt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guowangkeji.top/gtrplynmtq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtycuhoiay.html

[Q39] 自连接（查上下级）
来源：http://hz.smart0.xyz/gtqncyheel.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.iojbl.cn/gtmdyivtdo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gtnbjbaxbn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtnakkirxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtscyvefek.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gttgzkxcod.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtswdaeowo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gtcnvqfaha.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.c1oappe.top/gtbittlylg.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtdrjebrut.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtftffmmew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnxiangtu.top/gtxtbmylrd.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtyismzdsx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtbtumoomk.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtfflgkpjh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtgwkastdg.html

[Q45] EXISTS 判断存在
来源：http://hz.xuetiantiany.cn/gtgzispfzy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtrbrkpkkk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxinkj.top/gtbaepkjjk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtwghocsir.html

[Q47] 与平均值比较
来源：http://hz.hnxiangtu.top/gtofbdtjpv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xinyue.icu/gtuafgpeex.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigfzy.top/gtnfidgqsd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtwdszfiaw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtbqfrrtkx.html

[Q49] 更新单行
来源：http://hz.hnqzz.top/gtzapauvgf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtmmrehqec.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtwzjkylpa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fengsongda.top/gtqtgxipql.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtdhtafjpk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xziqi.cn/gttmcgprab.html

[Q52] 删除指定行
来源：http://hz.svipenyu.cn/gtquacsbre.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gttxoqpufn.html

[Q53] 按条件删除
来源：http://hz.jqgfzy.top/gtxoxpveyj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hysaishi.cn/gtvholjemr.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtuwbiacbm.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtuhoghuvk.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtxterpmsh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtvvbzkfdg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xinyue.icu/gtfjrrfacn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtcdcyjafy.html

[Q57] 行号
来源：http://hz.aizwys.cn/gtwxxzcudu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtoormtvlo.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtvhigyqby.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtbnqevnnv.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtqpicautf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtrkwtomxx.html

[Q60] 取上一行 / 下一行
来源：http://hz.guannengcc.top/gthkajpoxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj202588.top/gtgjhzglul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.feifeiyinyue.top/gttirshrez.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtfbyujheu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtxyolnius.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtpisryosx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtltbskiwo.html

[Q63] 开启事务
来源：http://hz.pycfn.com/gtglzkqufj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtfqpftvqc.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtlvollpcu.html

COMMIT;
来源：http://hz.ywan-chungtsiang.top/gtjtqspyom.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gtnvaczivi.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtcibocatn.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtkzpmmwmy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtzziejscy.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtinvczwts.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydzc1.top/gtxfznhuxv.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gtnlagrjyo.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtbwlsfibh.html

ROLLBACK TO sp1;
来源：http://hz.vqdsnc.cn/gtoaowjydz.html

[Q69] 查看执行计划
来源：http://hz.mhx1999.top/gtotaovqqm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhaomingkeji.xyz/gtlbdkvepi.html

[Q70] 更新统计信息
来源：http://hz.havefunace.top/gtnpyroxfk.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtiekolxwn.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtsiauviyq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtwoixgvrb.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gtxkdneaml.html

SHOW INDEX FROM users;
来源：http://hz.zhijiandao.cn/gtikaiyyhz.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtcytagssy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtqhswttww.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtoynskjjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtewafffmo.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gthhskjioa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtgfexxazh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtcjsnjdae.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtdltukuqw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtuvkczruj.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtztuarefh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.havefunace.top/gtwulxolye.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtlkvttwyd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtuptayfns.html

[Q79] 字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtuplmokdt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtgumgmbwy.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtnqlvvafj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yuanzhike.top/gttjphrcmy.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gtbgwgauym.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtlghbwrfo.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gtqxswmbvh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hongshengwenyu.top/gttxdomemu.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtlefulsun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtooarsqgw.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtdytpqaic.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtfxaqzcjx.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtpngveqzh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.fzhhl.top/gtvkjloizv.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtwsflxyuz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtveqqykpn.html

[Q87] JSON 字段做条件
来源：http://hz.nanxinkj.top/gtalqboypz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gtihdfqxqn.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgfzy.top/gtxcoksagw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtxbemzftj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtildwoyru.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtrajrejto.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gttozdxrif.html

[Q90] 生成序号列
来源：http://hz.fengsongda.top/gtmkazkmna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gttovpvzii.html

================================================================================
来源：http://hz.jqgfzy.top/gttqwwsore.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtutwdrnjf.html

================================================================================
来源：http://hz.bjfxy.top/gthwigiwvy.html

[R01] shebang 与严格模式
来源：http://hz.guowangkeji.top/gtljoakqbb.html

#!/usr/bin/env bash
来源：http://hz.jinqigufen.top/gtknqzcadb.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtstvvvqoq.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtyftgsrue.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtuzjrjymw.html

[R03] 只读变量
来源：http://hz.chenlongwang.top/gtxrllmwhs.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtcyjikvbg.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gteksbmxwn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hfpthk.cn/gtppyzwbke.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtxaciegen.html

name="${1:-default}"
来源：http://hz.shanyushiyangtech.top/gtvuelgemw.html

[R06] 判断命令是否存在
来源：http://hz.nwbrower.top/gthkwjxsbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtxpegcrci.html

[R07] if 判断文件
来源：http://hz.svipenyu.cn/gtlvteljcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuanzhike.top/gtwncacepp.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtxduhckvm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenjidiqi.icu/gtrkuwumiw.html

[R09] 字符串比较
来源：http://hz.shuidangran.top/gtmtmfcycn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cheryme.top/gtgnqyxvsr.html

[R10] 正则匹配
来源：http://hz.hysaishi.cn/gtwpoteetk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtiyhhrgdy.html

[R11] case 多分支
来源：http://hz.cdnleiting.top/gtctztffmi.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtztmcolpj.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gthlfbzqhg.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtxajkhekl.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtmtthpqoi.html

esac
来源：http://hz.svipenyu.cn/gtrkohbjmp.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtqilxzhck.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jianghu66.top/gtcvxzxgft.html

[R13] for 计数循环
来源：http://hz.ywan-chungtsiang.top/gtgajxsnwg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtwosnybig.html

[R14] C 风格 for
来源：http://hz.shanyushiyangtech.top/gtqrdcgnsb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtfhkdrhdr.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtpwtnnhoy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gteiwwrbnb.html

[R16] until 等待条件
来源：http://hz.gogol.net.cn/gttsvfozcd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtsbgafvcm.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtxxvqxyqf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yonumen.top/gtbpahtmkr.html

[R18] 遍历数组
来源：http://hz.yj20258888.top/gthlqnwhwb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtjigwfhit.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtfjqrbbsb.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gtxjohtlet.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtqycpycll.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtkrgetnmi.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtokltbhue.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtjsvauvzo.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gthlzlwnsd.html

echo "${s:0:5}"
来源：http://hz.vqdsnc.cn/gtwiwviscs.html

[R23] 字符串替换
来源：http://hz.sufxvd.cn/gtrlqttzth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtxnsnrrjn.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtsboqxbpg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yuxming.cn/gtjudnmlmy.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtywdihmti.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtzkagkimk.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtxdebbvwb.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtvrvwbrip.html

[R27] 算术展开
来源：http://hz.zdqjudy.top/gtanjhxolv.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtjcbzclxk.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtmnlhfuel.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtjhhnscud.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtihmeyxyi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtxwxdvqsk.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangtech.top/gtaqjcvrlc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtjiyfdrlo.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gteotxmzxm.html

f() { local x=1; echo "$x"; }
来源：http://hz.bjfxy.top/gtyrznliiw.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtxbustkit.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gthtnkxusq.html

[R33] 捕获错误并提示行号
来源：http://hz.fengsongda.top/gtugqqxpyi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtmwljilui.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtcttwgzun.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtlqrtfuvt.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtnpyvwpou.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yvedp.cn/gtlyrqesjk.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gtcbsqxepq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yuxming.cn/gtpbvcpgwp.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtfuvnmqxs.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtdubnhrjn.html

[R38] 管道串联
来源：http://hz.shanyushiyangkeji.top/gtjdkbzbrx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shuidangran.top/gtgrfddzld.html

[R39] 重定向标准输出与错误
来源：http://hz.jinghuilouyu.cn/gtjgyqrnzg.html


<!-- 参考信息 -->