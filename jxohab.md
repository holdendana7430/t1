代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtwfwihaug.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtcyypqiyr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtlbvdzgro.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtyhfkxsns.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cheryme.top/gtoqmgvtbt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.redwolf501.top/gtnqpvyflw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtzzxaeuqf.html

[P08] 处理浮点精度问题
来源：http://hz.yueranfly.top/gtnyctcqeq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtxpgkwqjr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xziqi.cn/gtauqhnbrt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtedumzgke.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.haohaochexian.top/gthikjmdmf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtkwitcfdq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtrtnwiowi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ivvv.top/gtjpkqepxc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ppjwa.cn/gtmcqgbyzb.html

================================================================================
来源：http://hz.zycfv.cn/gtrhtnjsja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gogol.net.cn/gtkkjzrssc.html

================================================================================
来源：http://hz.ybcxt.top/gtbidikeiu.html

[Q01] 创建表
来源：http://hz.pengpengdd.cyou/gtqvphvnwk.html

CREATE TABLE users (
来源：http://hz.tian-w.cn/gtnqhejivf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gthjqokyad.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtuonxbkpm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtifcpxpwj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gtjzytsdjm.html

);
来源：http://hz.hnqzz.top/gtehnmzbmo.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gtwsvugspf.html

CREATE TABLE orders (
来源：http://hz.guowangkeji.top/gtgqptcqxr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtkdeutyqc.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtelakqqip.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtticoiqcp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtbfsunyqp.html

);
来源：http://hz.sysykeji.top/gtlkpypjvt.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gtyqvdquwg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gthzhhahul.html

[Q04] 修改列类型
来源：http://hz.chenzaomai.com/gtlaiukgkb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jlsjyb.cn/gtrujeqtfl.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtjsbtfczr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.iojbl.cn/gtexejncom.html

[Q06] 删除列
来源：http://hz.shanyushiyangkeji.top/gtjclmjdao.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gaohongyu789.top/gtfhrttqfq.html

[Q07] 删除表
来源：http://hz.cashguo.top/gtsdtngfyg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pengpengdd.cyou/gtgdwlfxmn.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtvrabvovt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtgoakjdno.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtpkpfrwjq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dashuyun.cn/gtpunyqxlr.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtomyqsciv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtvbkzpcby.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangtech.top/gtelugmrzr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtjroaxcxs.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtxupbqqty.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.kuanghao11.cn/gtdnzzciir.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pengpengdd.cyou/gtbokdmilv.html

[Q13] 忽略重复插入
来源：http://hz.aibaodan.cn/gtvlvfpbib.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aibaodan.cn/gtkbldauhk.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtylqvqljx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gtoqamsjuv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtiwybcumu.html

[Q15] 查询全部
来源：http://hz.jlsjyb.cn/gtfpumhxkt.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gtcxqkkvnx.html

[Q16] 查询指定列
来源：http://hz.ydjk.org.cn/gtahtqzpnn.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gtiphmlklu.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtbxcqmtof.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtsidscrcn.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gtorrkmkwo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.svipenyu.cn/gtlczhenkb.html

[Q19] 范围查询
来源：http://hz.jyoumei.cn/gtfdfxfogk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xingfuxueyuan.xyz/gtnohddzxj.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtqphzkohg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gtmvjhkmjj.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtmwfqximc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gtytiheewh.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtslielcru.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhengqikj.top/gthrefdggx.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtleqwwbfw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtmcnidvrh.html

[Q24] 去重
来源：http://hz.xuanzx.com/gtmxahsezd.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxuanxn.top/gttejxaocb.html

[Q25] 只取前 N 条
来源：http://hz.xziqi.cn/gtojuijlrr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nwbrower.top/gtblznnjvi.html

[Q26] 计数
来源：http://hz.yj20258.top/gtjfqfiblu.html

SELECT COUNT(*) FROM users;
来源：http://hz.meibo888.top/gtxlpeutvo.html

[Q27] 条件计数
来源：http://hz.tian-w.cn/gtnepshdfz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.meibo888.top/gtbbzxwjjw.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gtbyjwjsjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tianlin.xyz/gtqryfcasb.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtbiihshjg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tanke756.top/gtsjekaavo.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtewoybexw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtskrlqrvw.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gttgvleflz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtkofsdfde.html

[Q32] 分组拼接字符串
来源：http://hz.jqgufenzy.top/gtwumxqgpe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtcrwdizuh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gthpmbwiyj.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtxkbyvlje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.feifeiyinyue.top/gtkodyhzqf.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtzzuqzzaa.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtprljzuhq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtnvpqflmg.html

) t WHERE rn = 1;
来源：http://hz.ivvv.top/gtssjrofou.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gtnydvzwil.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtznjsjame.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtxlgvujcu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hfpthk.cn/gtnwwrlhoh.html

[Q37] 右连接
来源：http://hz.52xcode.cn/gtbfwdedmv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.havefunace.top/gtyghkdolt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cdnleiting.top/gtlcwxnykr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtvffdrrou.html

[Q39] 自连接（查上下级）
来源：http://hz.guannengcc.top/gtxfjsacso.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nwbrower.top/gtlskrvpkb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gtdkjghsrd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtzoxihewx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hammf.cn/gtgveldqco.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtrderfmcz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuanzx.com/gtrtvrnncn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtidvlnfhw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtdxoznjmu.html

[Q42] 连接条件附加过滤
来源：http://hz.hongshengwenyu.top/gteucntvxv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtitdcefmo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtwwydjgqx.html

[Q43] 标量子查询
来源：http://hz.gzhubu.top/gtzrinfssm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gthghburfj.html

[Q44] IN 子查询
来源：http://hz.cdnleiting.top/gtsgwofcvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtxngkpwkv.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gtzlsrnsnu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtomlmduus.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtqxqjaaqi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtsntqsqhn.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gtbjivboya.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gthsrgeuee.html

[Q48] CTE 公用表表达式
来源：http://hz.yvedp.cn/gtyxujxtoi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhongyouzk.top/gtdbdajnld.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtdmsxrvgd.html

[Q49] 更新单行
来源：http://hz.yj20258888.top/gtvjqmjwik.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtlnexzwjv.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gtzoyfwnsh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gttwddoqsi.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtbqddscwo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtzasljxxc.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtioyhgosj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtvbtzqkrl.html

[Q53] 按条件删除
来源：http://hz.tian-w.cn/gtnszntpgi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.0kj1m.cn/gtzdskbixp.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gteqqiomtt.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtgizkbeog.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gttiwbowzj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hnxiangtu.top/gthlkslimz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yangfankeji.com/gtnhhutzla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gtcdkebrob.html

[Q57] 行号
来源：http://hz.yongpay.top/gthwvphmob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtzobpepfu.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gtarqtlrmz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xinyue.icu/gtajcffxef.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gthzkhgaue.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xuetiantiany.cn/gtiwopvhab.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtgywruhqg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yangfankeji.com/gtqnvckfcb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtvcmlhkoz.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtgtxeoons.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxuanxn.top/gtphyjerym.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtfegubkkm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtrxzyhwev.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtyxwotogd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtkufnuctr.html

[Q64] 提交事务
来源：http://hz.yuxming.cn/gtkfohumnv.html

COMMIT;
来源：http://hz.shuidangran.top/gthmkfgohm.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtszjzusjn.html

ROLLBACK;
来源：http://hz.ivvv.top/gtvozrxego.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtcmukwtoq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtbvcylpym.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangtech.top/gtxsulwfra.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gthomrabhj.html

[Q68] 保存点
来源：http://hz.kuanghao11.cn/gthilcfntz.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtbjmiuyww.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtnpntafmb.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtkinjaykw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtwzotocdk.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtviscavhl.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtfrlpzmyc.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gturgfxisg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtprgcgenn.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtxuvzzkxn.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtshrhtqhd.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtxwrovxfb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuetiantiany.cn/gthziiknww.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gtntwkstyy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtjhqjiuix.html

[Q75] 日期格式化
来源：http://hz.guowangkeji.top/gtnixfltor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtvoymeimc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guowangkeji.top/gtggkqgcaq.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtevcwmbwh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtffnxbjug.html

[Q77] 时间加减
来源：http://hz.xingfuxueyuan.xyz/gtbczjosok.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtesrlntea.html

[Q78] 当前时间
来源：http://hz.52xcode.cn/gtakemxgmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtscbmjuab.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtdbvtribl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtdcuggmtz.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gtzybbuxeb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yangfankeji.com/gttbliierl.html

[Q81] 字符串替换
来源：http://hz.hnqzz.top/gtglsfcayu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtifdgbfah.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gtfynhlwey.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtadfrgyrp.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtlowpgwsa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtljzayvwu.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtfouncefm.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtmrxdpadc.html

[Q85] 数值取整
来源：http://hz.nanxuanxn.top/gtkozvpirz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtglhqmztl.html

[Q86] 读取 JSON 字段
来源：http://hz.aizwys.cn/gttounvihc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtrmawaibp.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtzzeqaixp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnqzz.top/gtwgxxsqja.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gtawqqxjei.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtyqjvbseu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hywenlv.cn/gtcnkqyitd.html

[Q89] 判断表是否存在
来源：http://hz.svipenyu.cn/gthujpnekr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtbgqrbaon.html

[Q90] 生成序号列
来源：http://hz.yongpay.top/gtxjulmlph.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jqgufenzy.top/gttkpjhcta.html

================================================================================
来源：http://hz.yj20258888.top/gtwfjfzsre.html

R. Bash 专题
来源：http://hz.316326.xyz/gthefqbgtc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtelrqjnfq.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtgqlehzbl.html

#!/usr/bin/env bash
来源：http://hz.zhixingplan.top/gtqxquyvzq.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtbsydrjaw.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtaaptzjqz.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtcaehvxex.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gthersrvaa.html

readonly PI=3.14
来源：http://hz.316326.xyz/gttpghoumj.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtinjlxrhf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.quarkkingdee.top/gtzusrrwsm.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtfpghvalu.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtjnizcsks.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtxyvhukyv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtgjoajwty.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtextzkbgc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuanzx.com/gtzxqtxqrb.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtugvtvsao.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gaohongyu789.top/gtafvviecr.html

[R09] 字符串比较
来源：http://hz.tian-w.cn/gtfbhyyidi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtzozmnsbn.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gttnjokihy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gthtdsdrnk.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtnboffgct.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtsiewawhc.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtujurcthi.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtksqpkjby.html

*)     echo "未知命令" ;;
来源：http://hz.sufxvd.cn/gtpqdmyzma.html

esac
来源：http://hz.birdmap.top/gtgvybsnpn.html

[R12] for 遍历文件
来源：http://hz.xuetiantiany.cn/gtxxenxtgz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtpelqbssl.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtprtgltan.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.smart0.xyz/gtypnhdgqw.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtngxwsfsr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangdashe.top/gtwcefdznt.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtsbchvhks.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pengpengdd.cyou/gtoapvoxnq.html

[R16] until 等待条件
来源：http://hz.gogol.net.cn/gtrmijfzle.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtvvdcaycw.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtqenzuqqo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtldjfaflf.html

[R18] 遍历数组
来源：http://hz.jinqigufen.top/gtystjheky.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtmlmaslhp.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtdtdkdsvj.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtxgjqivpe.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gtrkthnygl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtuxgwcnlx.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtdniatejj.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtawlttbgs.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtyxczaeeh.html

echo "${s:0:5}"
来源：http://hz.daxiang520.top/gttyadscxa.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gtxkiwsuyv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtmcqhhpni.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtxhbdefdv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtsldlqvdi.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtwrtjafai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtjykpttmd.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtxeplyqqo.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtexurdazm.html

[R27] 算术展开
来源：http://hz.aibaodan.cn/gtlkdwtxap.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtmzhzakga.html

[R28] 浮点运算
来源：http://hz.hywenlv.cn/gtnzidenzm.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtuafayadb.html

[R29] 定义函数
来源：http://hz.dianchejie.cn/gtzehznlwg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtjwjkfmpn.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtgbwelvth.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtzuwhmejg.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtqzimfsud.html

f() { local x=1; echo "$x"; }
来源：http://hz.birdmap.top/gtettshyrk.html

[R32] 参数个数校验
来源：http://hz.hysaishi.cn/gtojbalpxq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhengqikj.top/gtvrcwlwyx.html

[R33] 捕获错误并提示行号
来源：http://hz.quarkkingdee.top/gtaidipfkh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtwjryzaoq.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtccvstmuj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtmaiqcncw.html

[R35] 后台执行并等待
来源：http://hz.sysykeji.top/gtexfikwne.html


<!-- 参考信息 -->