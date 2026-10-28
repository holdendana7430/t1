代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yongpay.top/gtctyzensh.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtkkqgoihv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtbkmdcdtf.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtifycfmeo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtsixdmldf.html

C#:   if (x is null) {}
来源：http://hz.hysaishi.cn/gtswsotzyt.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtcxxaiklb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtzjqktzfj.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtwmiloymy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtrkldpfnx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtyywljcqh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yonumen.top/gtzibclsen.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtdqnilany.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtxkgtlrml.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.kuanghao11.cn/gtbyroohgt.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtqzapigmx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtmkohxged.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtjnyhsfct.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jianghu66.top/gtohounhfw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtvfzmxbrs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gtfbvbylxk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jyoumei.cn/gtpzgcmoir.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtpskgwqvq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gticrcyasp.html

================================================================================
来源：http://hz.sweek.top/gtpfvosocf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtkqbygveq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnajblvqb.html

[Q01] 创建表
来源：http://hz.52xcode.cn/gtllmvsiwp.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtetojtffc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gtadjumwnn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gtawyjjgfd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtnknszpat.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtgzqqjyut.html

);
来源：http://hz.gogol.net.cn/gtzaytlfdw.html

[Q02] 创建带外键的表
来源：http://hz.jqgufenzy.top/gtkhvwxwab.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtbqxapxbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtirknwjru.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtapqyhcgk.html

amount DECIMAL(10, 2),
来源：http://hz.jqgufenzy.top/gtwefuhtei.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tianlin.xyz/gtrxbxgnzj.html

);
来源：http://hz.yueranfly.top/gtpgzylvil.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtkzakkyvj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtsvjasmqy.html

[Q04] 修改列类型
来源：http://hz.aizwys.cn/gtbbysbkrt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtavkenuhz.html

[Q05] 重命名列
来源：http://hz.snrcjt.cn/gtsduvccff.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtkzjsmhmh.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtidcywqms.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtnofkgjnc.html

[Q07] 删除表
来源：http://hz.jiagoushi.top/gtoecaxzax.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gttvhhvvlo.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtzlamyzxt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtrsopgtnr.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtchqbmbdp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtydlrvhor.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtczmbtqkc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtzbpztzuj.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtgfsebdug.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxuanxn.top/gtudmlfnci.html

[Q12] 插入后取自增 ID
来源：http://hz.mhx1999.top/gtlydhejex.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.52xcode.cn/gtmpzqcvcx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnxiangtu.top/gtotojhocl.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gteclguqzm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtqpopamvm.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhaomingkeji.xyz/gtsoxucfso.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hfpthk.cn/gtinldjent.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtbcdybhxl.html

[Q15] 查询全部
来源：http://hz.jqgufenzy.top/gttjinzays.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtewykwgiw.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtiehfpuft.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtahekdrtp.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtpjlicvmu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtdwlcsmbn.html

[Q18] 模糊匹配
来源：http://hz.jqgufenzy.top/gttuhiawkl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtybtpraul.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtzngpsnpa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dianchejie.cn/gtedqaqnce.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtvecxvcbn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtnhzizyoo.html

[Q21] 空值判断
来源：http://hz.fzhhl.top/gtfwsqlzvv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tanke756.top/gtxyuqfocd.html

[Q22] 排序
来源：http://hz.pycfn.com/gtnjletpdq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtpdgrzohd.html

[Q23] 分页
来源：http://hz.jinyuanbaomall.cn/gtrxslqehp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtvwcslelm.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtiqzjmynd.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gthealdrij.html

[Q25] 只取前 N 条
来源：http://hz.yueranfly.top/gtyvujuoon.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtrgdlxelt.html

[Q26] 计数
来源：http://hz.dianchejie.cn/gterwmmfxf.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhijiandao.cn/gtmyakqbmj.html

[Q27] 条件计数
来源：http://hz.snrcjt.cn/gtufiyovcl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtgezwyuty.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtcqbjojbi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtulirygiy.html

[Q29] 最大最小值
来源：http://hz.yj202588.top/gtlzbeehwd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtxdwmmmqx.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtoumfhrfy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtbogglhkt.html

[Q31] 分组后过滤
来源：http://hz.sweek.top/gtwitishuk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtxiwdhoqy.html

[Q32] 分组拼接字符串
来源：http://hz.fzhhl.top/gtxckcakfs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtyjhqhosq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtfupryhbk.html

[Q33] 多列分组
来源：http://hz.yj202588.top/gtbcaiomav.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258.top/gtfcankzzw.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gtzzjzmwpz.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gtiamvswjb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtuoburjgw.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gttncmmfhh.html

[Q35] 内连接
来源：http://hz.jqgfzy.top/gtsacbjgkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtaxtnfbjy.html

[Q36] 左连接
来源：http://hz.shzxlz.cn/gtwzwyexlz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtocwwdbcx.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtpzlrrtsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinyuanbaomall.cn/gtlzzwptyp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hysaishi.cn/gtdjyahaog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cheryme.top/gtbjxccdyb.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigfzy.top/gtfudykvyx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cheryme.top/gtpbsxyewp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtefgbvliv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtimiqhjkn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtcrbjnbph.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gttzhtoulf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jlsjyb.cn/gtzucixirb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hammf.cn/gtthvsvdeq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtkymjggvi.html

[Q42] 连接条件附加过滤
来源：http://hz.ivvv.top/gtbuhyphzi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.bjfxy.top/gtkafosjwl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtkoygpevd.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtczedsgwn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nanxinkj.top/gtrndqkgyk.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtmgdhftxc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtdgjtqtdv.html

[Q45] EXISTS 判断存在
来源：http://hz.zhiwuduotai.top/gtmtvtvcdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtrrzzkjrc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cheryme.top/gtwmhdksxq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtehhjwjxr.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gthlsycmtk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtlijrexdr.html

[Q48] CTE 公用表表达式
来源：http://hz.daria6918.cn/gtdumvbpqq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daxiang520.top/gtyddwcptj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zycfv.cn/gtrmczglrt.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtoiqsqtje.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtqsgrbuyn.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtfleaztnm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtqaidcbdv.html

[Q51] 用子查询更新
来源：http://hz.jqgfzy.top/gtuuppagaa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jiagoushi.top/gtlrkizfsi.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtvnmhbnth.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtcnqnydtm.html

[Q53] 按条件删除
来源：http://hz.yj20258888.top/gtgvjnxjhv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtjfcdmwal.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtwzouhaxg.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gtkrrzhgjv.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtsetmcwpe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gteslyfpax.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtrjhgsnlt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtyajmkvyo.html

[Q57] 行号
来源：http://hz.birdmap.top/gtqudmdnmy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hysaishi.cn/gtppcnuaay.html

[Q58] 累计求和
来源：http://hz.nanxuanxn.top/gtqbdnvrcz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtoiafnzab.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtrfywojon.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tianlin.xyz/gtpntyrmjy.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gtlbmbkggq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtqidfcjvf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtyhqxqbyk.html

[Q61] 移动平均
来源：http://hz.zdqjudy.top/gtgbwdzukp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cdnleiting.top/gtsskxylzw.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtxxszxkxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtmttbhgih.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtgwotafli.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gogol.net.cn/gtegppavni.html

[Q64] 提交事务
来源：http://hz.yangfankeji.com/gtskaoults.html

COMMIT;
来源：http://hz.shzxlz.cn/gtpkkbdnxa.html

[Q65] 回滚事务
来源：http://hz.birdmap.top/gtdphcevzq.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtzsgmynes.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtgqdqrlqu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtljjqqbzu.html

[Q67] 设置隔离级别
来源：http://hz.fzhhl.top/gtlujeetnl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yanxiufei.cn/gttuuceadp.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtxdrcnpsj.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtdzvdlgjo.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtbvsovmxs.html

[Q69] 查看执行计划
来源：http://hz.shuidangran.top/gtovhwssix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.andypj.xyz/gtuxprjobh.html

[Q70] 更新统计信息
来源：http://hz.zhoulong.xyz/gtdpudtkpe.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gtegqrokvm.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtmkymacsp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtckmuixyg.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gtthacamig.html

SHOW INDEX FROM users;
来源：http://hz.shangyingyoupin.top/gtvoyvemsq.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtvavsqjeq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtgvvvwqea.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtzifxgkkq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtuglbfycq.html

[Q75] 日期格式化
来源：http://hz.cashguo.top/gtacdyvfgh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtrpemrcwm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gtsepbbdrt.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtexkbleqe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtzxkxzxor.html

[Q77] 时间加减
来源：http://hz.zhongyouzk.top/gtoptfhagi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yongpay.top/gtqutxwdhw.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtxuxfbvfb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnxiangtu.top/gtppkzyamv.html

[Q79] 字符串拼接
来源：http://hz.vqdsnc.cn/gtwnosgdqf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gthcpwqlca.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtnkdhmjvy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtaatoxysc.html

[Q81] 字符串替换
来源：http://hz.yongpay.top/gtmookqvcz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.haohaochexian.top/gtndwllkwd.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtxepdzmmo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.nanxuanxn.top/gtvubjizmf.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gtlfyuydjt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jiagoushi.top/gtcybwdyum.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtdglnvrvm.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtrnpsdhwe.html

[Q85] 数值取整
来源：http://hz.zhixingplan.top/gtttqpgutt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sweek.top/gtxapfeunr.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gtnqlkufqn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fengsongda.top/gtngedgvys.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtuqcmlmmm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gtmvtcuyiq.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhaomingkeji.xyz/gtjmyoqedy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.snrcjt.cn/gtktzcimdi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ybcxt.top/gtsyhkhkng.html

[Q89] 判断表是否存在
来源：http://hz.ybcxt.top/gthnkyxezs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtyoyhthby.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gthashlxcm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gaohongyu789.top/gtbiupuxen.html

================================================================================
来源：http://hz.jinqigufen.top/gtjmflmtng.html

R. Bash 专题
来源：http://hz.yongpay.top/gtajwlwtif.html

================================================================================
来源：http://hz.gaohongyu789.top/gtudfvnlzu.html

[R01] shebang 与严格模式
来源：http://hz.wangdashe.top/gtkjobctrg.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtkfwqsioa.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtrhzmmfvq.html

[R02] 变量赋值与使用
来源：http://hz.dashuyun.cn/gthyemnkzt.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gthcwrpjtk.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtcspczyut.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtxghfkudn.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtkxcggauj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cdnleiting.top/gtigcnnmou.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtvpdcybft.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gttmdmlmoa.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtdwpyovsh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gotoacloud.top/gtyybxumnn.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtbviqupzy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtzafxcika.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtdoqtgove.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhaomingkeji.xyz/gtdmikzsxo.html

[R09] 字符串比较
来源：http://hz.9152youxi.cn/gtmobxjqmy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtbpunvhxa.html

[R10] 正则匹配
来源：http://hz.hnqzz.top/gtmjiwtxkb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.birdmap.top/gtbjetkqxj.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtenggjork.html

case "$1" in
来源：http://hz.shzxlz.cn/gtfpngwwua.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtdueobcno.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtpdrlhyeu.html

*)     echo "未知命令" ;;
来源：http://hz.jianghu66.top/gtclnbowdf.html

esac
来源：http://hz.yonumen.top/gtnsbbpzil.html

[R12] for 遍历文件
来源：http://hz.yj202588.top/gtrvpnzloa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtpuekldzq.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gttkkclrtx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtnvntkoie.html

[R14] C 风格 for
来源：http://hz.zhaomingkeji.xyz/gtrqxctvbk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnqzz.top/gtdahtyfxe.html

[R15] while 逐行读文件
来源：http://hz.feifeiyinyue.top/gtwvnfmquu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtdlsypain.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtmilcakpo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtcenisokh.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gthfgxvrjm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtovejknhi.html

[R18] 遍历数组
来源：http://hz.daxiang520.top/gtjlhorizm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yonumen.top/gtvcwlyesz.html

[R19] 数组长度
来源：http://hz.zhengqikj.top/gtqxtjzayu.html

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtivizftno.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtoycipxyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtwbrddvkz.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtrntauohu.html

echo "${#s}"
来源：http://hz.jqgufenzy.top/gtlgkyzubu.html

[R22] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtqetooesw.html

echo "${s:0:5}"
来源：http://hz.fengsongda.top/gtwhxvsbaz.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtascztdqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangtech.top/gtanbxktfy.html

[R24] 大小写转换
来源：http://hz.nwbrower.top/gtmbxwhjez.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shzxlz.cn/gtvgiulumz.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtgqyddaqr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gthhahzwly.html

[R26] 命令替换
来源：http://hz.yuxming.cn/gtaeoulbgx.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtyytyjwoz.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtvfldkbtx.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtvbuiyymh.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtdgxvovkt.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtvdnfwuxk.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtkoxxqaku.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtmsrwswqj.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtjbziluiy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yvedp.cn/gtyxijgnqv.html

[R31] 局部变量
来源：http://hz.yonumen.top/gtcimakgnx.html


<!-- 参考信息 -->