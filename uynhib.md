代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yonumen.top/gtiathcfyl.html

TS:   if (x == null) {}
来源：http://hz.shuidangran.top/gtszxnuphe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtajqwnjdw.html

Go:   if x == nil {}
来源：http://hz.ppjwa.cn/gttbaspluc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigfzy.top/gttrgnwthw.html

C#:   if (x is null) {}
来源：http://hz.zhengqikj.top/gtrrhwpywh.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtkewjthle.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtrjrdxdbv.html

PHP:  // 手写时间戳比较
来源：http://hz.kuanghao11.cn/gtvdexradm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtjnxhmmxi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtggwngust.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydzc1.top/gtyheugsmy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jlsjyb.cn/gtkuhdtkwd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shanyushiyangkeji.top/gtasptnscw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.aibaodan.cn/gtbitvrnij.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtzyncbmxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.9152youxi.cn/gtussuvrbw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sufxvd.cn/gtccrefqlb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xylfe.cn/gtdsjtnkin.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtaxscjrbg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dianchejie.cn/gtuxkukuku.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tanke756.top/gtdbrrblmn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.tian-w.cn/gtyjwnuadu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gtbufbdvbd.html

================================================================================
来源：http://hz.gaohongyu789.top/gthmzmkolk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtvsenvxhe.html

================================================================================
来源：http://hz.fengsongda.top/gtjznyydmh.html

[Q01] 创建表
来源：http://hz.yj20258.top/gtuyloaiht.html

CREATE TABLE users (
来源：http://hz.ywan-chungtsiang.top/gtufcpgcox.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtyzkkgrid.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sweek.top/gtxiqplwna.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtedpkhsvj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gthawempby.html

);
来源：http://hz.zycfv.cn/gtfldpriml.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtdmdhtybn.html

CREATE TABLE orders (
来源：http://hz.jqgufenzy.top/gtaqcmovvu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.0kj1m.cn/gtynprxjac.html

user_id INT NOT NULL,
来源：http://hz.jiagoushi.top/gtldzyzsfa.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtonillmbi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zdqjudy.top/gtkdumetmk.html

);
来源：http://hz.dianchejie.cn/gtuaiigbpn.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gtgqxsbrwx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtnjeihaqd.html

[Q04] 修改列类型
来源：http://hz.aizwys.cn/gtzrizjgrt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yvedp.cn/gthmgemwwx.html

[Q05] 重命名列
来源：http://hz.cdnleiting.top/gtdstelemw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gtdygvcopq.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gtamulbelv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtlblwaoob.html

[Q07] 删除表
来源：http://hz.yonumen.top/gtqywjbkaw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtqimkswwg.html

[Q08] 创建普通索引
来源：http://hz.c1oappe.top/gtegqguodq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtrsaizzbg.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtycqohwrn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.meibo888.top/gtayznqbjl.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtqdagensx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.smart0.xyz/gttufvbzdg.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gtfygujrio.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtkexelrwk.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtpcvbgfsb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.vqdsnc.cn/gtxrvzinhu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.pycfn.com/gtlxtjfgkn.html

[Q13] 忽略重复插入
来源：http://hz.cqqwz.cn/gtfvsofgxb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtacccseqj.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtmqkizmjg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gtbsmqxqbm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.birdmap.top/gtdmdwjklk.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtqtnfsnhf.html

SELECT * FROM users;
来源：http://hz.daxiang520.top/gtqemyises.html

[Q16] 查询指定列
来源：http://hz.zhengqikj.top/gtvagcpezh.html

SELECT id, name FROM users;
来源：http://hz.cucudq.cn/gtvvflzcua.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtjkowcois.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.svipenyu.cn/gtnjlaqgmj.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtsmhahqzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aibaodan.cn/gtzytntemx.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtyujmmhxn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhiwuduotai.top/gtparfaxro.html

[Q20] IN 列表
来源：http://hz.nwbrower.top/gtmoshjyfc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jiagoushi.top/gtijzkfqyg.html

[Q21] 空值判断
来源：http://hz.hnxiangtu.top/gtkotdqyyb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtmfdkcnaf.html

[Q22] 排序
来源：http://hz.cheryme.top/gtjqueatwg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtpphxzedl.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtnxrsikff.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.feifeiyinyue.top/gtfrtlwifr.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gtsqctjmmm.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtqfmoexhj.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtibezlyiy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtgkewvwuw.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtremnwgme.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtopsqkdhe.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtddfiwwpo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gtgjocfibz.html

[Q28] 求和与平均
来源：http://hz.jlsjyb.cn/gtmnggjyfy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtnegixnwj.html

[Q29] 最大最小值
来源：http://hz.hnxiangtu.top/gtmgqdisjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtiygcbkia.html

[Q30] 分组统计
来源：http://hz.haohaochexian.top/gtqvbbmytp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtwjfwmzjk.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtdllzynqu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtnnkjkyie.html

[Q32] 分组拼接字符串
来源：http://hz.ybcxt.top/gtlhflvlrd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtembdcaeu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sweek.top/gtvlxitcmw.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtlemwmdix.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuanzx.com/gtbecmyxlb.html

[Q34] 每组取第一条
来源：http://hz.dianchejie.cn/gtojidvgri.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtyaakvzkw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtudywvstr.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtrbbmfrfr.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gttkqrmvby.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtnzrlspcw.html

[Q36] 左连接
来源：http://hz.jinqigfzy.top/gtywlxljli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtagvhfohy.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtdcwmaxhu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gthuvtxojy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.316326.xyz/gtgxawoeeo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daria6918.cn/gtbpbsitjr.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtoqjfbjzg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtvqjeybzc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yonumen.top/gtcpghltxz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ywan-chungtsiang.top/gttvzvpciz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.316326.xyz/gtwppwsaci.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtdwakynbw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.vqdsnc.cn/gtuhseugul.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yonumen.top/gtnojydxgf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gtyapruyxq.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtixtrimin.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cheryme.top/gtvucoynyt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gttiachbfy.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtjlyxdmmv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ivvv.top/gtvquohseq.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gtuhzgxzvg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xinyue.icu/gtgolzstse.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtjrmwgprk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtfpuapvyr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gthvbhhxif.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtowglnodl.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtvyhxpuqq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtscokfwgb.html

[Q48] CTE 公用表表达式
来源：http://hz.0kj1m.cn/gtlrtsyerl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258.top/gtuosngwbm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xinyue.icu/gtfupaeukv.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtpwavwxnw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guannengcc.top/gtxwagdbtb.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtmxkrnbyx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtfrusuxgr.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtbpzfmlmv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ivvv.top/gtsrwiefuq.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtffkaoumz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtguvhacfk.html

[Q53] 按条件删除
来源：http://hz.smart0.xyz/gtbwxlfvqp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jlsjyb.cn/gtsluhnrsy.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtgieajcfe.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtsuiujvtk.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtntscmcmg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtvabhjegw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yvedp.cn/gtgluiqjaa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtxayxialo.html

[Q57] 行号
来源：http://hz.yueranfly.top/gtugsveaum.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gtiejeckzy.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtaowyfuwz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtadwtnldb.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtiwjqobfw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtixfzvaon.html

[Q60] 取上一行 / 下一行
来源：http://hz.ybcxt.top/gtfocjwtlm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zycfv.cn/gtaezrfnok.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtaljczkhp.html

[Q61] 移动平均
来源：http://hz.meibo888.top/gtotulnsxf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtukxplfne.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtdieipbub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtbuiafzpo.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtsdaktpfk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hfpthk.cn/gtwkspucay.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtortygrtw.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtnfhabezq.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtyiwsnixe.html

ROLLBACK;
来源：http://hz.iojbl.cn/gtefjakena.html

[Q66] 行锁查询
来源：http://hz.52xcode.cn/gturnfpitc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtevrbzzwb.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtngdwwveh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gthfelhzof.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtsevtcidt.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtwnlbvcfn.html

ROLLBACK TO sp1;
来源：http://hz.snrcjt.cn/gtbfyzsuaq.html

[Q69] 查看执行计划
来源：http://hz.smart0.xyz/gtwbtebtnm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gthxmjnqjb.html

[Q70] 更新统计信息
来源：http://hz.jiagoushi.top/gtwwufgtor.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtsmvtjqkt.html

[Q71] 查看建表语句
来源：http://hz.xuetiantiany.cn/gtyuzhyxzl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtovduzglm.html

[Q72] 查看索引
来源：http://hz.zhengqikj.top/gtlydnwbng.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtluvmvril.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gttyosmqer.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhixingplan.top/gtwylvxlea.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtrdyglafp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtvxmmmjsd.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtntsikfcy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtksjceptc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gthvjuxvne.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtzikoliig.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gthdyltyuc.html

[Q77] 时间加减
来源：http://hz.fzhhl.top/gtdycevoqh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtoscrnmlx.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtyefhuxfv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhaomingkeji.xyz/gtsjjehiud.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtoxigdrat.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtxwykviel.html

[Q80] 字符串截取
来源：http://hz.yvedp.cn/gtikaepnas.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtofpglfub.html

[Q81] 字符串替换
来源：http://hz.aibaodan.cn/gtafhqjkbs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtulvnkvst.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtllsrrvpt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtnmqvlrxx.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtdidolwsi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtudrkohpz.html

[Q84] 去除首尾空格
来源：http://hz.chenjidiqi.icu/gtipxdjpjz.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtrfzeapbs.html

[Q85] 数值取整
来源：http://hz.chenzaomai.com/gturgnbflm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gtidpjoouk.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtybtednjm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtcnpbjdsn.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtpnjrxzny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtpxtjumpn.html

[Q88] 行转列（条件聚合）
来源：http://hz.cucudq.cn/gtuanmksje.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtsdmhsxhw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gtelwjchgh.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtqyeghwas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gtmsaqbdnf.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtnnnaalkw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gtnhseizwa.html

================================================================================
来源：http://hz.jiagoushi.top/gtuyuvdycs.html

R. Bash 专题
来源：http://hz.9152youxi.cn/gtlyvtxtlo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwwuyrggm.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtekxiusfj.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gteosudhci.html

set -euo pipefail
来源：http://hz.wangdashe.top/gthntpfgjf.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtoyypsimv.html

name="Tom"; echo "$name"
来源：http://hz.yonumen.top/gtbxqkueap.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gttpttruhb.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtikazxcps.html

[R04] 位置参数
来源：http://hz.meibo888.top/gthjetgbhf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtiraivemy.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtmutdzcfj.html

name="${1:-default}"
来源：http://hz.316326.xyz/gtufjfnjol.html

[R06] 判断命令是否存在
来源：http://hz.cqqwz.cn/gtqkshomur.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtagmsznlg.html

[R07] if 判断文件
来源：http://hz.zhongyouzk.top/gtphzxkbvl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtzmhfziou.html

[R08] 数值比较
来源：http://hz.andypj.xyz/gtzppylfos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhoulong.xyz/gtpnjepafc.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtymenjqwl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.snrcjt.cn/gtppimfrso.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gtrbetyliy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangkeji.top/gtsksispnp.html

[R11] case 多分支
来源：http://hz.xuanzx.com/gtcmcgsagc.html

case "$1" in
来源：http://hz.haohaochexian.top/gtvnlmmhdq.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtiygpllto.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtddzohszu.html

*)     echo "未知命令" ;;
来源：http://hz.xinyue.icu/gtujuvodgu.html

esac
来源：http://hz.birdmap.top/gtcmtjwqjo.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtmanhxhhw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gteskmqymy.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gtjqupubqd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtnorklpsj.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtcwfcxlls.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yongpay.top/gtfcmqdsbc.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gtgdoqjohh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gtxeagozev.html

[R16] until 等待条件
来源：http://hz.cqqwz.cn/gtaoxudega.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtmwmpuagn.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtuiknfpnv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gttqinlhqy.html

[R18] 遍历数组
来源：http://hz.svipenyu.cn/gtlkyomrui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gtjfqafgio.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtnjgzdnyh.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtmbuoiaer.html

[R20] 关联数组（字典）
来源：http://hz.316326.xyz/gtxufqmcno.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xziqi.cn/gtcvsucjmt.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gtvvnimiqd.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtktfcpity.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtrcvbetcw.html

echo "${s:0:5}"
来源：http://hz.gotoacloud.top/gtdgpnbzjj.html

[R23] 字符串替换
来源：http://hz.zhengqikj.top/gtjfwjuuah.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtkbpfrequ.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtdzcjydex.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtpppbrgpc.html

[R25] 去后缀 / 去前缀
来源：http://hz.xinyue.icu/gtphqztgkp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pengpengdd.cyou/gtkozrpmqp.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtgxmrswaf.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtpgowmevc.html

[R27] 算术展开
来源：http://hz.tanke756.top/gtocxofwma.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtdriundaq.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtkewfryhx.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtjqcydhor.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtfllfoorx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.snrcjt.cn/gtyyhvxatz.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtkjruxvwf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuetiantiany.cn/gtxwxnkaag.html

[R31] 局部变量
来源：http://hz.chenjidiqi.icu/gtqppwucip.html


<!-- 参考信息 -->