代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigufen.top/gtlezklowz.html

C#:   if (x is null) {}
来源：http://hz.yuxming.cn/gtutefyoaa.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtlovjwolr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenjidiqi.icu/gtqsjaghpz.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtvhoicnww.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtzxxlllnx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtvissxcri.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gthzwmsaxu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtaaciyxwf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gogol.net.cn/gtbtkwhqou.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtrvyarxwa.html

[P08] 处理浮点精度问题
来源：http://hz.hywenlv.cn/gtiehnhgjj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtmvihfhhf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtsvozgrur.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.vqdsnc.cn/gtgbjsqvnp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtkgsexkwx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gtqyplvskm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gthtupstkg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtmoqcyupl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtxdihobev.html

================================================================================
来源：http://hz.daxiang520.top/gtxqthntmk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.52xcode.cn/gtmiufnqbh.html

================================================================================
来源：http://hz.hywenlv.cn/gtwbbkubid.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtogemsnsn.html

CREATE TABLE users (
来源：http://hz.shanyushiyangtech.top/gtwnaaeqqf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtklyabcly.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cashguo.top/gtuhavjxsx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtfaoaancg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtziwaxctp.html

);
来源：http://hz.yongpay.top/gtrlcjjzfn.html

[Q02] 创建带外键的表
来源：http://hz.zycfv.cn/gtravahcss.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtnodojkoy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtzfsefyst.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gtvnbqqzlk.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtajeqdjtx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gtverxnuyo.html

);
来源：http://hz.snrcjt.cn/gtejgimfgd.html

[Q03] 增加列
来源：http://hz.andypj.xyz/gtbrcxbmhe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aizwys.cn/gtejvqkkjn.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtjnpdvgxt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtokoyoxgw.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gtrwwzrxcy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtrdrfvyjz.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtwdgbqyiy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtublhqmlv.html

[Q07] 删除表
来源：http://hz.shzxlz.cn/gtikdjnhus.html

DROP TABLE IF EXISTS orders;
来源：http://hz.meibo888.top/gtpqqhnunm.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gthtvqxwre.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtbnnyuylv.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtxofoglpy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gthmecpgow.html

[Q10] 插入单行
来源：http://hz.pengpengdd.cyou/gtfpstdoaf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.haohaochexian.top/gtcnyoqlov.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtdghbdyum.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.redwolf501.top/gtbgxdljsi.html

[Q12] 插入后取自增 ID
来源：http://hz.tanke756.top/gtvovenmtr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hysaishi.cn/gthjgylehw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenzaomai.com/gtkubzdyry.html

[Q13] 忽略重复插入
来源：http://hz.xinyue.icu/gtpxpprjxd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxinkj.top/gtembdbrki.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhoulong.xyz/gtkafkixbe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtosijgjoo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shangyingyoupin.top/gtriuzzkfr.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtyfthlfbl.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtltoydphx.html

[Q16] 查询指定列
来源：http://hz.xuetiantiany.cn/gtxqpkxnss.html

SELECT id, name FROM users;
来源：http://hz.jqgufenzy.top/gtpoiyyaus.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtqjfmkilq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sufxvd.cn/gtagfxaupd.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gtjhbjlvig.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtezwvxlhn.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gtonagybkm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gzhubu.top/gtgvzwieyi.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtfixbxltx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258.top/gtnhokifdm.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtwfffcfkm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sweek.top/gtbrgodofc.html

[Q22] 排序
来源：http://hz.shanyushiyangtech.top/gtxohyugyk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuanzx.com/gtyvvwgwfb.html

[Q23] 分页
来源：http://hz.mhx1999.top/gtmfotlooz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtjhkyfhes.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtzrgmucjj.html

SELECT DISTINCT city FROM users;
来源：http://hz.sxryk.cn/gthfufilmg.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtdssfxmqe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.iojbl.cn/gtedqqisig.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtatwbhiwc.html

SELECT COUNT(*) FROM users;
来源：http://hz.hysaishi.cn/gtkhaulcoy.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtzsspxzvj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtjetamivm.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtjjktxlpq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtcmsnmgjg.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gtwalanyai.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtwoefpjdp.html

[Q30] 分组统计
来源：http://hz.sweek.top/gtqyjrkszy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gteslahbjs.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtryerfizh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gtcqrptusv.html

[Q32] 分组拼接字符串
来源：http://hz.pengpengdd.cyou/gtvboviqgc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtcmzutnqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtmhdwvtrt.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtijjoptwv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtwxktgvou.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtgbpvyxpy.html

SELECT * FROM (
来源：http://hz.nanxuanxn.top/gtqrjtjard.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.iojbl.cn/gtherhdzfn.html

) t WHERE rn = 1;
来源：http://hz.zhongyouzk.top/gtatmznpvg.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtlrukieal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtsbfsjdur.html

[Q36] 左连接
来源：http://hz.zhaomingkeji.xyz/gtfjdslumb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtknbvvtor.html

[Q37] 右连接
来源：http://hz.jqgufenzy.top/gtmdxeeujg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtkczedwyq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gtfgqdaglh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.aibaodan.cn/gtupnzebal.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gtszofxlrl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtyqalrrhp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtilvorbvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtdrwfrvop.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtxztxcofr.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtfzbytrib.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtervqmpbv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtyzukqazz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtdxcdrtah.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtrxbixizr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dashuyun.cn/gtkxufnltm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtmrtznwzl.html

[Q43] 标量子查询
来源：http://hz.tian-w.cn/gtvcgsnacp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtbvjfmmny.html

[Q44] IN 子查询
来源：http://hz.yanxiufei.cn/gtkpgcqvir.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtwvckutlo.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgfzy.top/gtbqbenpwi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shuidangran.top/gtpmkdavqc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtxhlbnprf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtnesxsjhy.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtqlalkyhy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtnaazrlhh.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtxzkmnqfj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gtmyitxaac.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gttgwnuath.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtgfzvlxpp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtnpcmsesg.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtmcxcubdp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtyjwymjoh.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtmtppdpmr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtxjofxoog.html

[Q52] 删除指定行
来源：http://hz.yonumen.top/gtwrabupgs.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gotoacloud.top/gtgmadvacs.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtpyrbezuc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtngxoafih.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gttcclhgcs.html

TRUNCATE TABLE logs;
来源：http://hz.dianchejie.cn/gtfwotasro.html

[Q55] 排名（并列占位）
来源：http://hz.xziqi.cn/gtnjaczqwu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtwuvcxtbp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtgoqtjvrh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydzc1.top/gtitqmupyq.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtscgfurxm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangdashe.top/gtpuieahde.html

[Q58] 累计求和
来源：http://hz.fengsongda.top/gtmjywudbn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gtisfifygw.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtswhjglzi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gtskddqqkh.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gtptfjwpae.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtkgqzswbg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtwwyzyrfx.html

[Q61] 移动平均
来源：http://hz.mhx1999.top/gtyimknzif.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gtvmjbckda.html

[Q62] 分组占比
来源：http://hz.xuetiantiany.cn/gtprzcwvqy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtiylnfpaq.html

[Q63] 开启事务
来源：http://hz.hnxiangtu.top/gtnembkddo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtbiqyhzvk.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtxnssutzc.html

COMMIT;
来源：http://hz.gzhubu.top/gtwxdwriqa.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtsecliaqg.html

ROLLBACK;
来源：http://hz.guowangkeji.top/gtqxphvpwu.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtsonnoiqg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.redwolf501.top/gtpxchxxcu.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gtaoecgrex.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gthkpnmtvg.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtxzmbhcxq.html

SAVEPOINT sp1;
来源：http://hz.jinyuanbaomall.cn/gtelqzenwk.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtabwcilic.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtmvwoaypo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj202588.top/gtqclfklgi.html

[Q70] 更新统计信息
来源：http://hz.dashuyun.cn/gtbbnxqmfq.html

ANALYZE TABLE users;
来源：http://hz.gzhubu.top/gtjqvkkhrn.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtybdfhofu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtbhxqoxxg.html

[Q72] 查看索引
来源：http://hz.jinqigfzy.top/gtjzkpttaf.html

SHOW INDEX FROM users;
来源：http://hz.xuetiantiany.cn/gtmqywbgze.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtdmmpekkk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhaomingkeji.xyz/gtpzjaahfj.html

[Q74] 强制使用索引
来源：http://hz.nanxuanxn.top/gtdjqplvcw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gtxprmdsem.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtqxteflhf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gttyexepoo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtzchlrghf.html

[Q76] 按天统计
来源：http://hz.yvedp.cn/gtudzryjgi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuanzhike.top/gtihygznsk.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtxmusnucf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xuanzx.com/gtopmunpfr.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtjsgcedkv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtbefymhtu.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtxhghvbqk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtmqyvfzgu.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtvgaalbux.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtumyrbjie.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtrrpjbdpn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zycfv.cn/gtwgmiglqe.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtowdiwyse.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtqwelxovy.html

[Q83] 大小写转换
来源：http://hz.guowangkeji.top/gtqupnvbrl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvjtsunuf.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gtncaiozdx.html

SELECT TRIM(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtizockoss.html

[Q85] 数值取整
来源：http://hz.smart0.xyz/gtjicvdttr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtocoskndx.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtpgmakuru.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtwlmzxrtw.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtsyhnhijt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtxmvowtwp.html

[Q88] 行转列（条件聚合）
来源：http://hz.gotoacloud.top/gtjkfthjim.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gtlrxsutcs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtnndmopct.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtzjnhvqjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtksninntm.html

[Q90] 生成序号列
来源：http://hz.hfpthk.cn/gtykemiqdi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtwadjdyjd.html

================================================================================
来源：http://hz.kuanghao11.cn/gthwotgfrv.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtgofueldo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtppkndemw.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtwpauibpr.html

#!/usr/bin/env bash
来源：http://hz.jqgufenzy.top/gtdphecwyo.html

set -euo pipefail
来源：http://hz.ywan-chungtsiang.top/gticzxpvea.html

[R02] 变量赋值与使用
来源：http://hz.gotoacloud.top/gtunhngrzo.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtfurwilld.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gthdkurdiw.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gttppeqqao.html

[R04] 位置参数
来源：http://hz.gogol.net.cn/gtshtwiokz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenlongwang.top/gtsuzjobou.html

[R05] 参数默认值
来源：http://hz.jiagoushi.top/gtnugyzekg.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gttbhqvoka.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtvrrjumft.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.9152youxi.cn/gtupqfmhkx.html

[R07] if 判断文件
来源：http://hz.jinqigufen.top/gtpisemynx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtqogsiagn.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtdfceebag.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gttfrlqrdc.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtyadmwicp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtercnhzka.html

[R10] 正则匹配
来源：http://hz.zhengqikj.top/gtcpnrqiug.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtogvnrsdg.html

[R11] case 多分支
来源：http://hz.svipenyu.cn/gtpxbbezjh.html

case "$1" in
来源：http://hz.gaohongyu789.top/gtxtiwibou.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtnikpyqyf.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtxkpyxnuq.html

*)     echo "未知命令" ;;
来源：http://hz.yuanzhike.top/gtbeeptfdl.html

esac
来源：http://hz.jinyuanbaomall.cn/gtxmkrprfu.html

[R12] for 遍历文件
来源：http://hz.zhiwuduotai.top/gturjwkdbi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtwdqtvnzw.html

[R13] for 计数循环
来源：http://hz.c1oappe.top/gtgwnesnas.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xziqi.cn/gtaspwjdmh.html

[R14] C 风格 for
来源：http://hz.wangshuangyany.cn/gtuhxexaed.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtdvbcqsqw.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtwcebmdqb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtyeejpuqc.html

[R16] until 等待条件
来源：http://hz.9152youxi.cn/gtmrgdtukx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtmylamfrd.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtsmfxutbq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gttkuuobwh.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtphcunfnr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtlqilyovq.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtnmaydvsx.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtuofpsgxt.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtzdpgylml.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtpxeaizaw.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtzwgefgqv.html

echo "${#s}"
来源：http://hz.smart0.xyz/gtbclzthzk.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtvagfpcan.html

echo "${s:0:5}"
来源：http://hz.xinyue.icu/gtyynmcoae.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtqkleuozl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gtvdzjmhaj.html

[R24] 大小写转换
来源：http://hz.chenlongwang.top/gtudswkeow.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhoulong.xyz/gtmvkpwpur.html

[R25] 去后缀 / 去前缀
来源：http://hz.hammf.cn/gtdgyuxpgm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gotoacloud.top/gtgamkwscd.html

[R26] 命令替换
来源：http://hz.0kj1m.cn/gtzmclyhof.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtencfhxdd.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtbqythbur.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtbcuudsee.html

[R28] 浮点运算
来源：http://hz.jinqigufen.top/gtsbivqkio.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258.top/gtafvsrmhq.html

[R29] 定义函数
来源：http://hz.hnxiangtu.top/gtzxihekgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtacemdstg.html

[R30] 函数返回状态码
来源：http://hz.yangfankeji.com/gtrzphkfxo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtqlammcki.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtkjmesnrn.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtosghckbx.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtdziayqlm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gthigrqtrs.html

[R33] 捕获错误并提示行号
来源：http://hz.gzhubu.top/gtprmbudye.html


<!-- 参考信息 -->