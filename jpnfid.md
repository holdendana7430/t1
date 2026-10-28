代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.haohaochexian.top/gtrwbgqlmy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxinkj.top/gtrnpxkxsb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtnydfdrip.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtlieqlymw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtelkdpxuj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtpwjcjhst.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.iojbl.cn/gtvkedgomj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtbxusllst.html

================================================================================
来源：http://hz.yj202588.top/gtinflissu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydjk.org.cn/gtynruobjg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmdvzmjff.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gtvbztwcjs.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtwscvqdpv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtxebzmpri.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jinqigufen.top/gtgqgviyqa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtouqrcybn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtazvwkenl.html

);
来源：http://hz.chenzaomai.com/gtacgkfruv.html

[Q02] 创建带外键的表
来源：http://hz.xingfuxueyuan.xyz/gtchjdrfjc.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gteyoevdgi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtmxwkzimk.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtgtskhekg.html

amount DECIMAL(10, 2),
来源：http://hz.chenzaomai.com/gtsfvezmna.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtpikehruv.html

);
来源：http://hz.cashguo.top/gtkitdbltz.html

[Q03] 增加列
来源：http://hz.svipenyu.cn/gtrshtvdji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtrvfjmuhc.html

[Q04] 修改列类型
来源：http://hz.zhijiandao.cn/gtaibtmafi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gtxquajmkp.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtejaadyts.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hnxiangtu.top/gtbomcfclg.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtldumkrgo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinghuilouyu.cn/gtvoifbuqn.html

[Q07] 删除表
来源：http://hz.jqgufenzy.top/gtbaedcxzr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hfpthk.cn/gtogdlhyrv.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtfjrlznoh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xylfe.cn/gthnylzyfa.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtfmywjvuk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xziqi.cn/gtjaiwjlun.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtrjzoqmow.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hnxiangtu.top/gtnvtjskzj.html

[Q11] 一次插入多行
来源：http://hz.fzhhl.top/gtvmdntqen.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtutvtrhnv.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtpssrimry.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinghuilouyu.cn/gtlzgqmrlz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.quarkkingdee.top/gtskktnysw.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtdulvvgkq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gtorpdcjdj.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtthbfamdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.quarkkingdee.top/gtzsfsjqcc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtkqgrgpoa.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtldnpnonu.html

SELECT * FROM users;
来源：http://hz.jinyuanbaomall.cn/gttqyqhuru.html

[Q16] 查询指定列
来源：http://hz.sweek.top/gtscdbghip.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtnevjrweh.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gthwfdxtyl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.fengsongda.top/gtdzymfvms.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gtetdbqvzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sufxvd.cn/gtsoenqahk.html

[Q19] 范围查询
来源：http://hz.gotoacloud.top/gtaljtamil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydzc1.top/gtnjgwfkam.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtuqlkfegt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtxvdclwtq.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtakgbecuj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fzhhl.top/gtugvddvsj.html

[Q22] 排序
来源：http://hz.sweek.top/gtycddctpj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtagmuwoyn.html

[Q23] 分页
来源：http://hz.yj20258888.top/gtkckiddoo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtysftdogd.html

[Q24] 去重
来源：http://hz.cheryme.top/gtkqgjcphx.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtwubmzmpq.html

[Q25] 只取前 N 条
来源：http://hz.andypj.xyz/gtmgeaxfto.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.tanke756.top/gtdeupliju.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtokpmaios.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtnzmzjdjw.html

[Q27] 条件计数
来源：http://hz.guannengcc.top/gtmvubrjtc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtpuzfqivt.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtlkaawtrl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtvwqwgvrq.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtplrkypsa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtkiqfvoou.html

[Q30] 分组统计
来源：http://hz.hywenlv.cn/gtwrftdlab.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtwmwuvoky.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gtuxdfmgit.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daxiang520.top/gtnvfpazrv.html

[Q32] 分组拼接字符串
来源：http://hz.wangshuangyany.cn/gtrgntwqul.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtjbuybuhe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.havefunace.top/gtajmltomu.html

[Q33] 多列分组
来源：http://hz.zhongyouzk.top/gtymtwllis.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtsewlhhyl.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtwmdmzjam.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtdwxbqidu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.snrcjt.cn/gtngdxsach.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtwtiacqrr.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtydsbjjlx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtljfdsgdc.html

[Q36] 左连接
来源：http://hz.jinyuanbaomall.cn/gtmryabpsm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtlhhddkpv.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtbgofdjaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtbzbvocww.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtqtafepzi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cashguo.top/gtheuwwxiq.html

[Q39] 自连接（查上下级）
来源：http://hz.kuanghao11.cn/gtpstgmfkw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtiraznodh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtsejzbeku.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jianghu66.top/gtqsoawkbu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.birdmap.top/gtklotqsun.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtnuslptyq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj202588.top/gtbvodajxy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtqubgktba.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangshuangyany.cn/gtpxudschv.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gttdpjpkrv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.kuanghao11.cn/gtpgyazxty.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtodjtreha.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtuclnxivi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtqytcwiao.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtagrwtynt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pengpengdd.cyou/gtgwqvgrhc.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtahyhkwwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtdhddawgc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtpntjxbsx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtocgskcnm.html

[Q47] 与平均值比较
来源：http://hz.hywenlv.cn/gtvefsykph.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hammf.cn/gtbinqeswj.html

[Q48] CTE 公用表表达式
来源：http://hz.9152youxi.cn/gtlgosgtvw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gthnhbjpvh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtnrsetknz.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtuwmhgzvo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtofzewjiq.html

[Q50] 批量更新
来源：http://hz.zhiwuduotai.top/gtaugnwbcq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtojhiqrdv.html

[Q51] 用子查询更新
来源：http://hz.jianghu66.top/gthuqyvzfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gttwutbksg.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtuaykbits.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gttjloayuk.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtunwopgkn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.0kj1m.cn/gtwtvxfmvq.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gtthsckops.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtpgzpnhts.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtrbfspfmm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtwwqbccmy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tanke756.top/gtyrodkgjv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtbhgixjoz.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtbfjbowhd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jlsjyb.cn/gtxkhqbpad.html

[Q58] 累计求和
来源：http://hz.xylfe.cn/gtekhaovke.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtqycwryvf.html

[Q59] 分组内累计
来源：http://hz.jlsjyb.cn/gtadfuqtos.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gttaubbiiu.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangshuangyany.cn/gtaqaptkic.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtxjjofsxw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhengqikj.top/gtyxnefkwz.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtxkysjzbz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtulvdnmbp.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtjdxhwren.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtepehewwu.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtojigtfrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtmgznpmoe.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtswbzxqbo.html

COMMIT;
来源：http://hz.xinyue.icu/gtuuzkhndd.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtzoapuzbx.html

ROLLBACK;
来源：http://hz.chenzaomai.com/gtjjoeimhb.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtrysuyany.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtmybaycqt.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gtvyqdvded.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.snrcjt.cn/gtsgbnfhdr.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtskyekowy.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtmsayxzmu.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtwctlhiqu.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtvbpoifxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtbtooyqed.html

[Q70] 更新统计信息
来源：http://hz.xingfuxueyuan.xyz/gtzpupmtpt.html

ANALYZE TABLE users;
来源：http://hz.meibo888.top/gtsveynzpn.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtypulvbko.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ppjwa.cn/gtqoenomcb.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtfhxhwitq.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gttyzfezat.html

[Q73] 查看表状态
来源：http://hz.xylfe.cn/gtazjpvhie.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.52xcode.cn/gtngatbwxv.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtltpbmuni.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtdlbzcwkr.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtjadmoazt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.c1oappe.top/gtzzgdlsmj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtrcglezvb.html

[Q76] 按天统计
来源：http://hz.yueranfly.top/gtxuukumhx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangkeji.top/gtwerculpb.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtjsjohhqt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ppjwa.cn/gtwxdjiyqa.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtinqswlta.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nwbrower.top/gtrdghldsd.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtzptosmsf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtyxzevetv.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtbrjozsab.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtqfxwtztf.html

[Q81] 字符串替换
来源：http://hz.hywenlv.cn/gtnyzeopgp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cqqwz.cn/gtzspoamis.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtxsomismp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dianchejie.cn/gtfhcthqqd.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtfmumifir.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gttazfynda.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtybnrqhem.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtoplungjg.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtbctnfbuv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtdfxudpbk.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gthnlzyegv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtkmuximel.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtzrmnhnko.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xinyue.icu/gtejwyltor.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtmvkokqym.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daria6918.cn/gtrnnasfdd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtyrdacstz.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtjudpwpdx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuetiantiany.cn/gtcmwdrffj.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gtqyofzvmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhongyouzk.top/gtwyfhottj.html

================================================================================
来源：http://hz.dianchejie.cn/gtrmauqwgl.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtxddgcsnp.html

================================================================================
来源：http://hz.xuanzx.com/gtyozmyjpo.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtsonqteal.html

#!/usr/bin/env bash
来源：http://hz.zhongyouzk.top/gtdyzsefgm.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtdhpumwcr.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtddspguny.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gthyspwxzt.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtgcooggby.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtaqgjzxln.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtchsdqxby.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuetiantiany.cn/gtytkwsgyi.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtisdtiifj.html

name="${1:-default}"
来源：http://hz.jinqigfzy.top/gttmryxzft.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gtizhhcimx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtfsbthswp.html

[R07] if 判断文件
来源：http://hz.316326.xyz/gtggnzljnn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.meibo888.top/gtxnaenire.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtdhmoaiqg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtqlkeegca.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtiqtdkubw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jlsjyb.cn/gtvmtobsmy.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtngmrqqoi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtbdgphlio.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtuflhazok.html

case "$1" in
来源：http://hz.cqqwz.cn/gtthkdoybv.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtrkfddfol.html

stop)  echo "停止" ;;
来源：http://hz.jyoumei.cn/gtzmgrkoii.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gtrzdpphig.html

esac
来源：http://hz.daxiang520.top/gtxiyfytzn.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtwdtrcilq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangtech.top/gtfujysndu.html

[R13] for 计数循环
来源：http://hz.quarkkingdee.top/gthalcdjbh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ivvv.top/gtaodnivkz.html

[R14] C 风格 for
来源：http://hz.chenlongwang.top/gtnqddstqb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtqtyzwkro.html

[R15] while 逐行读文件
来源：http://hz.yj20258.top/gtzjuvbihs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gtmpmwdexb.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtjsmrcsks.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtctdgsjmo.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtnmvtayjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuanzx.com/gtbcxlmgez.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtfgcjudhn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tian-w.cn/gtzqguhoyu.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtuoxwxmzl.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtkydfrdfo.html

[R20] 关联数组（字典）
来源：http://hz.pycfn.com/gtmyjrmdmz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.meibo888.top/gtksdsyflm.html

[R21] 字符串长度
来源：http://hz.ehwqpu.com/gtszirpsap.html

echo "${#s}"
来源：http://hz.yj20258888.top/gtwulaimjb.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtskpqilzp.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtdxdxczxc.html

[R23] 字符串替换
来源：http://hz.xinyue.icu/gtethiypdh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hysaishi.cn/gteojiclye.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gtbjyywfrt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.mhx1999.top/gttwithlnk.html

[R25] 去后缀 / 去前缀
来源：http://hz.fengsongda.top/gtmapckotw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtgbriiumi.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gteuljrght.html

now=$(date +%F); echo "$now"
来源：http://hz.fzhhl.top/gtrgixljro.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtziwxviwx.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtmgbmszla.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtrnmkcxhf.html

echo "scale=2; 10/3" | bc
来源：http://hz.birdmap.top/gtzvbqbisz.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtdeumzbbz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtlaacuvqf.html

[R30] 函数返回状态码
来源：http://hz.kuanghao11.cn/gtjbnqezkh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtsykukdow.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtwcuseats.html

f() { local x=1; echo "$x"; }
来源：http://hz.ppjwa.cn/gthvclhlmu.html

[R32] 参数个数校验
来源：http://hz.wangshuangyany.cn/gtcndwkcmr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtyhwcynnq.html

[R33] 捕获错误并提示行号
来源：http://hz.gogol.net.cn/gttkjtotak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jiagoushi.top/gtyyujwpmc.html

[R34] 退出时清理
来源：http://hz.xinyue.icu/gtsapaleoy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtkqiswgim.html

[R35] 后台执行并等待
来源：http://hz.vqdsnc.cn/gtmkvkckwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shuidangran.top/gtguzigeeh.html

[R36] 并发执行多个任务
来源：http://hz.chenjidiqi.icu/gtkzqzgmym.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gteaftyxcb.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtmkkzepgf.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtsferfuut.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gtdawgdvze.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtijwfsjwv.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtvukryyqs.html


<!-- 参考信息 -->