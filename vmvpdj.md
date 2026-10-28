代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.wangdashe.top/gtyvtuluqj.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtkpycqkaq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.bjfxy.top/gtnlvvrrbr.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gthqfbbduj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtnysfmcba.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtcnmfgnqb.html

[P07] 防抖与节流
来源：http://hz.jinyuanbaomall.cn/gthmhgkvow.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtjimhnnsw.html

PHP:  // 手写时间戳比较
来源：http://hz.zhiwuduotai.top/gttqewpzgo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtsilheadv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtjgyuzmgo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtkxtjsafa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.bjfxy.top/gtpuqllxyn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.daria6918.cn/gtbpprrdel.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hywenlv.cn/gtpoitilkv.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtkeoqniwc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gttyfhqvys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtfjklczgs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtstdqpyxb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangdashe.top/gtdgklgnwd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gtzhdndqqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yvedp.cn/gtaaqaartz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.andypj.xyz/gtjhfkzgjw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhaomingkeji.xyz/gtssnfpllx.html

================================================================================
来源：http://hz.52xcode.cn/gtaoeltcql.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgufenzy.top/gtjzfcqxqd.html

================================================================================
来源：http://hz.bjfxy.top/gtuhpmrzrv.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtelgyllgj.html

CREATE TABLE users (
来源：http://hz.sweek.top/gtmgtnuxrr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtzapmrpjf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gthsbdkuou.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydjk.org.cn/gtizjeattx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jianghu66.top/gtthkpcsfc.html

);
来源：http://hz.shanyushiyangtech.top/gtjtkkcmvs.html

[Q02] 创建带外键的表
来源：http://hz.aizwys.cn/gtialwtror.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtdjbptlxt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gthqhxcjwe.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gtbwqdtwoo.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gtrmpibvzu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gtybwuncwx.html

);
来源：http://hz.wangdashe.top/gtyqyalrii.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtdyyirnvl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtkyypimxa.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtpwyahhdx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.quarkkingdee.top/gtxkhzlltb.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtkcmhjfrk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hfpthk.cn/gtlypnbvtw.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtylcsofxj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhaomingkeji.xyz/gtbdppiqlr.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtjtybgwhn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.vqdsnc.cn/gtysaikhlc.html

[Q08] 创建普通索引
来源：http://hz.chenzaomai.com/gtjupyidbl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtajihpfbv.html

[Q09] 创建唯一索引
来源：http://hz.zhaomingkeji.xyz/gthsaizzmd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtofwtvvsv.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtocyasqyn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtuiupjzmg.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtenbcqagn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtnqakgkyt.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtsodytfdo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gtvwphnqbv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtvklunaea.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtqduqmsll.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shangyingyoupin.top/gtbyofdxgu.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhaomingkeji.xyz/gteyxqbrbp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtfidblfyh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtqtuacciq.html

[Q15] 查询全部
来源：http://hz.redwolf501.top/gthpbdewfb.html

SELECT * FROM users;
来源：http://hz.zhaomingkeji.xyz/gtteepowpl.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtvzwsbeun.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtbwcyymcv.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtpqycauky.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ywan-chungtsiang.top/gtrlbwhmgo.html

[Q18] 模糊匹配
来源：http://hz.xuanzx.com/gtkknfchnc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jiagoushi.top/gttogfjamc.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtwvljogyi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtslmrmyaw.html

[Q20] IN 列表
来源：http://hz.bjfxy.top/gtddyhggiw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.quarkkingdee.top/gtjvteuewy.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtwivlfgth.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtblqbhkkv.html

[Q22] 排序
来源：http://hz.52xcode.cn/gtrbceoiqr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtongmuiac.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtlipruuru.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.havefunace.top/gthheghvpw.html

[Q24] 去重
来源：http://hz.yonumen.top/gtzonwzncj.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gttsukngqe.html

[Q25] 只取前 N 条
来源：http://hz.aibaodan.cn/gtrgvpttxa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhoulong.xyz/gtfgndycly.html

[Q26] 计数
来源：http://hz.jlsjyb.cn/gtkkodpocy.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnxiangtu.top/gtiimpkfyj.html

[Q27] 条件计数
来源：http://hz.vqdsnc.cn/gtbsqzjtit.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.meibo888.top/gthadgdoax.html

[Q28] 求和与平均
来源：http://hz.pycfn.com/gtserxcyxn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtxdqldkym.html

[Q29] 最大最小值
来源：http://hz.hnqzz.top/gtvcjxitff.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxinkj.top/gtwntcysmp.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gtrfumnkfq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtlqypbtgo.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gtmdemvwnv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtexjxbvqd.html

[Q32] 分组拼接字符串
来源：http://hz.havefunace.top/gtuyckjhbg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtahlwlkdh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shuidangran.top/gtlpbehtip.html

[Q33] 多列分组
来源：http://hz.ehwqpu.com/gtqowyegen.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dianchejie.cn/gtlfnjsvpg.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtlnufwfet.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtartryawf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtogtxtuaa.html

) t WHERE rn = 1;
来源：http://hz.chenzaomai.com/gtcqersswk.html

[Q35] 内连接
来源：http://hz.jinqigufen.top/gtsnbhgfqc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gttwmucbdv.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtnfykdnju.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtxdizyqft.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtsdodtvix.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sxryk.cn/gteeixpmhl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtyamfjnmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gtvuxdmhdy.html

[Q39] 自连接（查上下级）
来源：http://hz.ywan-chungtsiang.top/gtaumxfqct.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtpphdlkoe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuetiantiany.cn/gtfuqitupb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xinyue.icu/gtgdfasdgg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtoqpewsai.html

[Q41] 多表连接
来源：http://hz.zhengqikj.top/gtugalydov.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtfeywmhty.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aizwys.cn/gtbnrzdkfw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ivvv.top/gtfounrkij.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtmclbjhle.html

SELECT u.name, o.amount FROM users u
来源：http://hz.quarkkingdee.top/gtwvsfmezj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtjmmgbfer.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gthptcgpms.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtiappmjtt.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtefxroabq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.vqdsnc.cn/gtlqfaqfqb.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxinkj.top/gtacqgsoyq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtwsvzyypl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydjk.org.cn/gturlybddg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtzvcazvcf.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtjbuormvk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tian-w.cn/gtydofiiyw.html

[Q48] CTE 公用表表达式
来源：http://hz.pycfn.com/gtiupztkxj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtygmrharc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtspyqtlqr.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtdjjfpcgt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtqfmlcica.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtzbuklebg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jiagoushi.top/gtdiiappex.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtxsahmgrt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtgeikittz.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtgnrcjmoy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtqtvmewqf.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtvfmcslim.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtxfttkpwa.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtdezditub.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtnchlwpar.html

[Q55] 排名（并列占位）
来源：http://hz.shangyingyoupin.top/gtxpezgcqh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gtweharlyy.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtimxahrpf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.0kj1m.cn/gtqlakhpzr.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtornrhnde.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtevvinsyx.html

[Q58] 累计求和
来源：http://hz.vqdsnc.cn/gtogoveedr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtuzntfkck.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtdhpwdgfs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.bjfxy.top/gtbdutrtci.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhixingplan.top/gtedricjhs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtyawecmbh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.316326.xyz/gtjgtjbdny.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtusarpfon.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtthdyrlqf.html

[Q62] 分组占比
来源：http://hz.hnxiangtu.top/gtoxrpjwtf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtdbiroqix.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtrxgljlwj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gtiygsuear.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtoqgjpklu.html

COMMIT;
来源：http://hz.nwbrower.top/gtaednyhbl.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtrpgmdywy.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gtthzwwhji.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtzxzehjkf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtfqqehody.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtxtswjknw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtbevmyzht.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtvjanyjgv.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gtufqirtjx.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtibrjhpir.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gthucftuoz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.redwolf501.top/gtysoiukit.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtondtqnlj.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtaolglrvp.html

[Q71] 查看建表语句
来源：http://hz.yongpay.top/gtpluseste.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtzremjjqg.html

[Q72] 查看索引
来源：http://hz.nanxuanxn.top/gtnjhouymg.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtpkoxodsh.html

[Q73] 查看表状态
来源：http://hz.daria6918.cn/gtddhevkti.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shzxlz.cn/gtcgikmzov.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangtech.top/gtgkwuvezb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtmvguyqfu.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtpfubstsk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.svipenyu.cn/gtudmryltb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtwbrpfxwa.html

[Q76] 按天统计
来源：http://hz.redwolf501.top/gtfoxkwlfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guowangkeji.top/gtlshdswmq.html

[Q77] 时间加减
来源：http://hz.xylfe.cn/gteagwjbxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtvszvcmcu.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtfytphfiq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.smart0.xyz/gtgtnwrlqv.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtzojfhufw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pengpengdd.cyou/gthszhickm.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gtdzvetcvh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtjzipvyzo.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtauwxagfv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aibaodan.cn/gthkthrjuz.html

[Q82] 字符长度与字节长度
来源：http://hz.yj202588.top/gtbmiysmrm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtjmgswxhh.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtjtquefeq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtmxtjtyze.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtzviwmuew.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinqigufen.top/gtnbxywetl.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtctfczqvg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtjblwlynz.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtnrnllugl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pengpengdd.cyou/gtwpozjurf.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtnkwstksi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhengqikj.top/gtwthbvhtd.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtmwpdvkwq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtnneoonwq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuanzx.com/gtepyuigby.html

[Q89] 判断表是否存在
来源：http://hz.nanxinkj.top/gteigzdafp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtcvwaeloc.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtdpbtwhzn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtnndifzfw.html

================================================================================
来源：http://hz.daria6918.cn/gtnihajkko.html

R. Bash 专题
来源：http://hz.yonumen.top/gtjgtiolud.html

================================================================================
来源：http://hz.aizwys.cn/gtukbpwkxn.html

[R01] shebang 与严格模式
来源：http://hz.tanke756.top/gtymmnxfbz.html

#!/usr/bin/env bash
来源：http://hz.quarkkingdee.top/gtxfewvvdv.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtpwqcoqgw.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtyzwfkqef.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gtlxtzeayd.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtqedmvmus.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtyenlpnom.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtluwnofgb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtzlxrnjby.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtehxxxhak.html

name="${1:-default}"
来源：http://hz.xinyue.icu/gtvbpxyuqg.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtfeqanfuw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtobiaasoy.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtsndicqkm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtjmcmdzgh.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtdsrireez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtqndttykx.html

[R09] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtkgefrzaw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigfzy.top/gtfxjzksxg.html

[R10] 正则匹配
来源：http://hz.kuanghao11.cn/gtizmliqsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuanzx.com/gtnwtcmqlh.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtwqbdexvo.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtqosuaxga.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtskhkmigj.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtajoinvwu.html

*)     echo "未知命令" ;;
来源：http://hz.xingfuxueyuan.xyz/gtouezkqwn.html

esac
来源：http://hz.ywan-chungtsiang.top/gtecohtgps.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtemhykuxw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtatbjicsr.html

[R13] for 计数循环
来源：http://hz.wangshuangyany.cn/gtbowrzwop.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtrdqftjut.html

[R14] C 风格 for
来源：http://hz.nwbrower.top/gtbryidgbh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.52xcode.cn/gterncahzb.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtqwgiyxlh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtruxjqsdv.html

[R16] until 等待条件
来源：http://hz.yuanzhike.top/gtrajawgfw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtbvpeyvzc.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtgfwnjyug.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtwbuzierk.html

[R18] 遍历数组
来源：http://hz.yongpay.top/gtbekjuhco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtpdujzejn.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtyiitizvy.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtrjsuksvg.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtjppjsheo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.316326.xyz/gtqfybflnb.html

[R21] 字符串长度
来源：http://hz.tanke756.top/gtraurovmn.html

echo "${#s}"
来源：http://hz.shzxlz.cn/gtizppjamr.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtalioysbk.html

echo "${s:0:5}"
来源：http://hz.fengsongda.top/gtpgdshdwb.html

[R23] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtsstjkwoy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tian-w.cn/gtpwawkeec.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtdqspkcml.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtqbukyldm.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtaonmolhh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtpnjwpbhb.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gtsezuqyxb.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtrkoddume.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtjlipovvh.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gteqfkhiga.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtxxiqvxxc.html

echo "scale=2; 10/3" | bc
来源：http://hz.smart0.xyz/gtpyjihpzj.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtgasvpyuf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cucudq.cn/gtemkwsjho.html

[R30] 函数返回状态码
来源：http://hz.jinghuilouyu.cn/gtksfriqap.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gttndzxfag.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtkgubhugt.html


<!-- 参考信息 -->