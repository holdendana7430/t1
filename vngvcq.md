代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guannengcc.top/gtshbxengt.html

C#:   if (x is null) {}
来源：http://hz.jqgfzy.top/gtzrkwiitb.html

[P07] 防抖与节流
来源：http://hz.yongpay.top/gtejzowaqt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtdaywpgja.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtoolwknhx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtpktuomyb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtzwtlugtk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yongpay.top/gtdkyoczbu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.svipenyu.cn/gtiysclsbl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtgbdtmgbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.feifeiyinyue.top/gtfzfbbiii.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtsakembyp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zdqjudy.top/gttjoxyxcc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.haohaochexian.top/gtticvrpyh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtvwrnikhs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gthpifiuns.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhixingplan.top/gtbcnlplyr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zycfv.cn/gtecuowwwr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtfybsqnjz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gtjkaphtyn.html

================================================================================
来源：http://hz.jlsjyb.cn/gtfmlxhffj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gthsqrhgle.html

================================================================================
来源：http://hz.zycfv.cn/gtmimdbmpf.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtjxqnejil.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtunvqatqx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtmetjpwdx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gtjtwrlzrj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.vqdsnc.cn/gtpthoghiy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jianghu66.top/gtjtaypmog.html

);
来源：http://hz.sysykeji.top/gtydztritk.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtyjojthxg.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtpcgeuvlr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gzhubu.top/gtoyozcctu.html

user_id INT NOT NULL,
来源：http://hz.daxiang520.top/gtdlwldzfg.html

amount DECIMAL(10, 2),
来源：http://hz.redwolf501.top/gtinxiqwhd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gttghwybcv.html

);
来源：http://hz.shanyushiyangtech.top/gtfrnbblfn.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtulhbvecd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtnxheeqxw.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtphhkqexa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gaohongyu789.top/gtzmjfusrg.html

[Q05] 重命名列
来源：http://hz.shuidangran.top/gtunapxtqz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtfgljlieb.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtvarbaehm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.vqdsnc.cn/gteqzvwveb.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtvxobieml.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhengqikj.top/gtwfelczzj.html

[Q08] 创建普通索引
来源：http://hz.mhx1999.top/gtygkbzsrr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtyjsnxlrf.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtodbgkljb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ivvv.top/gtfrkzbedb.html

[Q10] 插入单行
来源：http://hz.feifeiyinyue.top/gtnxccwcec.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtlchvfazp.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtxcfktazu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtbtskvpwv.html

[Q12] 插入后取自增 ID
来源：http://hz.gogol.net.cn/gtvvadabxn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.birdmap.top/gtlrynbynl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtsahqhxzd.html

[Q13] 忽略重复插入
来源：http://hz.yonumen.top/gtswjadwvc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jiagoushi.top/gtwtbzwuhv.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gtszyrztmi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dianchejie.cn/gthlwbwqrh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtuajnpwtz.html

[Q15] 查询全部
来源：http://hz.9152youxi.cn/gtyjxuwzps.html

SELECT * FROM users;
来源：http://hz.sysykeji.top/gtxxqbzueh.html

[Q16] 查询指定列
来源：http://hz.ydzc1.top/gtfsmbgdsn.html

SELECT id, name FROM users;
来源：http://hz.hysaishi.cn/gtdpbuudhv.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtgkndlpds.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtbonpewew.html

[Q18] 模糊匹配
来源：http://hz.vqdsnc.cn/gtqwohuyrs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zycfv.cn/gtiucfqzng.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gtxhuejolr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtvvojtmev.html

[Q20] IN 列表
来源：http://hz.ppjwa.cn/gtbguywmaj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pengpengdd.cyou/gtvqxhpxgy.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtcwfixivi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.birdmap.top/gterdjefrr.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtslpnrayj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtogvtbsii.html

[Q23] 分页
来源：http://hz.xuetiantiany.cn/gtlimftfnm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtfpfukiwq.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtlgxcnmqr.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gtgmuwpivu.html

[Q25] 只取前 N 条
来源：http://hz.xingfuxueyuan.xyz/gtbsyvtbml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtlyqilfjf.html

[Q26] 计数
来源：http://hz.xingfuxueyuan.xyz/gtosqqelsn.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtzequtipn.html

[Q27] 条件计数
来源：http://hz.xuetiantiany.cn/gtsbbkemrq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtdnmtzzhy.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtvvjrchvf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gtscldnded.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtzpcthkhp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dianchejie.cn/gtnhyvtjqo.html

[Q30] 分组统计
来源：http://hz.kuanghao11.cn/gthoiohvyf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtrpwpywjl.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gthhiwiuog.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtlabeeztm.html

[Q32] 分组拼接字符串
来源：http://hz.xziqi.cn/gtwwpcohyn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gthtqmbqat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sufxvd.cn/gtqaorrtai.html

[Q33] 多列分组
来源：http://hz.yuxming.cn/gtxwadsfvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtsihvhsfb.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtyikhjxan.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gthfcefoje.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtdqwparii.html

) t WHERE rn = 1;
来源：http://hz.nanxinkj.top/gtcaygizup.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtziqwarob.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtxuetsfii.html

[Q36] 左连接
来源：http://hz.vqdsnc.cn/gtxtreprqr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtgavhywfp.html

[Q37] 右连接
来源：http://hz.jianghu66.top/gtruswutka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtubgqyiro.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtkijhpaay.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gttedftooi.html

[Q39] 自连接（查上下级）
来源：http://hz.cashguo.top/gtxieumvbv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yanxiufei.cn/gtihaylshx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtlxhiiwlt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gzhubu.top/gtuovasqix.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenzaomai.com/gtsroccnjk.html

[Q41] 多表连接
来源：http://hz.zycfv.cn/gtaexukxfv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtjpczegvu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtzimefvvp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtchfvkpgt.html

[Q42] 连接条件附加过滤
来源：http://hz.mhx1999.top/gtcfdsxaoy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtwvhuunvu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pycfn.com/gturoadmfj.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gterapzhal.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtzyczsowy.html

[Q44] IN 子查询
来源：http://hz.zhaomingkeji.xyz/gtqwjgnoov.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtfocwlqgv.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gtmpzgnugw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtnhignwwq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shangyingyoupin.top/gtghbqjanw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gthcnqhngn.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtkloumylm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtwizecwpd.html

[Q48] CTE 公用表表达式
来源：http://hz.tanke756.top/gtsxrbfznj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hfpthk.cn/gtlhnwgtpq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gtarvextpo.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtrwjfbugb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtyrruprdj.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtvarogeli.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtycephykn.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtempadpgx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtvrrjxjfl.html

[Q52] 删除指定行
来源：http://hz.pycfn.com/gtnxxyveuh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtqnnvocjl.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtloynyfdl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ybcxt.top/gtnmiwoovb.html

[Q54] 清空表
来源：http://hz.yueranfly.top/gtyoppxwqq.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gthoshbznj.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtphgtgzxp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.bjfxy.top/gtbofktfdk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenlongwang.top/gtygtmonrd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hongshengwenyu.top/gtzxrfksps.html

[Q57] 行号
来源：http://hz.tianlin.xyz/gteylkhpmi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtkuywculv.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gtjvxihitm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hywenlv.cn/gtuhsbngdw.html

[Q59] 分组内累计
来源：http://hz.birdmap.top/gtatjwuysc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.meibo888.top/gtbodjsxcz.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtwobqyeyb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtzxgytfgo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gthkivvmix.html

[Q61] 移动平均
来源：http://hz.ehwqpu.com/gtkvyslfsv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtxvparoda.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtioxnhqlh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtixiuocgs.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gttbewcrhs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.bjfxy.top/gtgsatfije.html

[Q64] 提交事务
来源：http://hz.hammf.cn/gtcbjmwhvx.html

COMMIT;
来源：http://hz.jinqigufen.top/gtjaxphhvs.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtwoanptpl.html

ROLLBACK;
来源：http://hz.cheryme.top/gtptnvkemz.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtibhtolun.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgufenzy.top/gttetimeco.html

[Q67] 设置隔离级别
来源：http://hz.zdqjudy.top/gtwmcdpcqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtkmvzjgoi.html

[Q68] 保存点
来源：http://hz.wangdashe.top/gtmouojdpb.html

SAVEPOINT sp1;
来源：http://hz.yvedp.cn/gtmhopfssd.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtmlatgmnb.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gtrqntzwiv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtfbxbwxoy.html

[Q70] 更新统计信息
来源：http://hz.cqqwz.cn/gtasuvwldf.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtwtaqtgbf.html

[Q71] 查看建表语句
来源：http://hz.yonumen.top/gtazjcfrzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gthrmnlojx.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtwlwrottf.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtbdnxyscf.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtkxwjgyoi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtyfrikihf.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gtxomqocge.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.haohaochexian.top/gteznfnhvy.html

[Q75] 日期格式化
来源：http://hz.chenjidiqi.icu/gtpdpfekvi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtxyhamibi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gtejcrsmac.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtwvwretvb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtpfimdxqg.html

[Q77] 时间加减
来源：http://hz.yueranfly.top/gtrwdfjmug.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtsdhehkye.html

[Q78] 当前时间
来源：http://hz.aibaodan.cn/gtdksgpddn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtueuonyim.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtpgacucgw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtdazuecos.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gtwcromrdd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhixingplan.top/gtdztudimq.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtfsqzezjv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtkydelrmn.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gthotansio.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xylfe.cn/gtfvzjnyjb.html

[Q83] 大小写转换
来源：http://hz.jlsjyb.cn/gtheqnczqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hnqzz.top/gtbnsljrpk.html

[Q84] 去除首尾空格
来源：http://hz.jlsjyb.cn/gttyqfttjs.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtztixeszz.html

[Q85] 数值取整
来源：http://hz.ydzc1.top/gtwnztfwnt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gtjemjcvyt.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtlfxqhvgj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtcwbtxnul.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtwgxoeifp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtbehsdsne.html

[Q88] 行转列（条件聚合）
来源：http://hz.jlsjyb.cn/gtktyhqlbd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gtcrmwhteo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtbohyyjfz.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtbepjfjhp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gaohongyu789.top/gtlmjpoquy.html

[Q90] 生成序号列
来源：http://hz.sxryk.cn/gtavetqzps.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtmavdqayx.html

================================================================================
来源：http://hz.yj20258888.top/gtsvgebkrp.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtbugrqazk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtargkljph.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtsdjdohiq.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtkuzarmeo.html

set -euo pipefail
来源：http://hz.jyoumei.cn/gtpkafrxwf.html

[R02] 变量赋值与使用
来源：http://hz.ivvv.top/gtixnjiyrd.html

name="Tom"; echo "$name"
来源：http://hz.zhoulong.xyz/gtemswlept.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtyryxrxdo.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gtfzefbrpx.html

[R04] 位置参数
来源：http://hz.shanyushiyangkeji.top/gtlgkmvpsm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtuuaaydrd.html

[R05] 参数默认值
来源：http://hz.jqgufenzy.top/gtwtwyndih.html

name="${1:-default}"
来源：http://hz.nanxinkj.top/gtsmarvipm.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtacbibbgb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cucudq.cn/gtkgwyliwo.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtnqaiiinr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shangyingyoupin.top/gtxbqmfmwq.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtndirzlvp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtgkfdogzp.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtkyiikyue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtyespmseh.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gttoagepnx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.redwolf501.top/gtrnfloden.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gttcpmorke.html

case "$1" in
来源：http://hz.ybcxt.top/gtiuqlvjcl.html

start) echo "启动" ;;
来源：http://hz.yj20258888.top/gtcpvdktun.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtmjrowvdy.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtxbpbdnli.html

esac
来源：http://hz.316326.xyz/gtqpwgkctx.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtzngutnaf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gttoombido.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtmrjcdflo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtynblhuqd.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtzzjelirg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtonacwmin.html

[R15] while 逐行读文件
来源：http://hz.dashuyun.cn/gtfcvtnhqi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtdjhptezg.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtcfutoltp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtceyuhkrx.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtvgjwfoxn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtfbwipdzj.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtkblcdlde.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gteccwodwf.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtckjeyrbp.html

echo "${#arr[@]}"
来源：http://hz.jlsjyb.cn/gtqmdykuae.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtvlmbkxfb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dianchejie.cn/gtzdlddevg.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtsbnvlyio.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtrafxnftp.html

[R22] 截取子串
来源：http://hz.ydzc1.top/gtpwaxyddt.html

echo "${s:0:5}"
来源：http://hz.chenjidiqi.icu/gtegyjgrtw.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtcidhcerd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gtvkkugeck.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtyjibensc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtmccgpxas.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtpolxilkp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sxryk.cn/gtjwdpeurd.html

[R26] 命令替换
来源：http://hz.ppjwa.cn/gtpdvkdydv.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtgypkbrvh.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtutuzsvsc.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtmvnqyccs.html

[R28] 浮点运算
来源：http://hz.xingfuxueyuan.xyz/gtshxqipka.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtpfydyehz.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtfdvshdjj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtwoskewbc.html

[R30] 函数返回状态码
来源：http://hz.quarkkingdee.top/gtkwgahbyw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.316326.xyz/gtoumhlyli.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtabfffwlb.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtjnmppgck.html

[R32] 参数个数校验
来源：http://hz.svipenyu.cn/gtarabdgmr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.kuanghao11.cn/gtmevoaltg.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtxofhdogl.html


<!-- 参考信息 -->