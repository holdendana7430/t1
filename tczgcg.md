代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sysykeji.top/gtfggmgfdt.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gteyudgdqy.html

[P07] 防抖与节流
来源：http://hz.jqgfzy.top/gtebgrgqcj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cucudq.cn/gtnmnacokz.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtttlokitt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtnykdhmgw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtrcjgfuxo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangkeji.top/gtqstttwtw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtunvpqrva.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cheryme.top/gtkvvizgkj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtrvowvper.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtqdcnwfxq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtlritzbpq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuanzx.com/gtyrettxyr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtesepfxew.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtxumjrsiw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yanxiufei.cn/gtluvwxswj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtzjdlsimg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gttqileqya.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tian-w.cn/gtvbsncbzu.html

================================================================================
来源：http://hz.daria6918.cn/gtmldffyhu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gtegbuhtuz.html

================================================================================
来源：http://hz.zhengqikj.top/gtztzgumvh.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtkigknegg.html

CREATE TABLE users (
来源：http://hz.yuanzhike.top/gttggehlpz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtmkvthnbj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pengpengdd.cyou/gtxxfohbbd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ivvv.top/gtzvwwmekq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.316326.xyz/gtaylnbuin.html

);
来源：http://hz.sysykeji.top/gtalqrsntv.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtixutbbpt.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gttaijjbqq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtjdawcmbf.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtqgoyvuat.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtevthlqyx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ppjwa.cn/gtwljoeumw.html

);
来源：http://hz.xziqi.cn/gttumrvxik.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtyldnmtgj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtuzfccdgx.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtugvftywi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.nanxuanxn.top/gtpdreqzrw.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gttfhoqgtt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gogol.net.cn/gtdgmricvq.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtsrsbjpyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxuanxn.top/gtytbggpfm.html

[Q07] 删除表
来源：http://hz.yuxming.cn/gtieetesoj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dashuyun.cn/gtbifmpgoq.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtiyobzuhy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.daria6918.cn/gtmahclelu.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtvgiavmxk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nwbrower.top/gtjgfmtxrf.html

[Q10] 插入单行
来源：http://hz.zhaomingkeji.xyz/gtcdgnwrdg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.nanxuanxn.top/gtttiyvztk.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtozwhqqty.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.haohaochexian.top/gtwrxxvmqg.html

[Q12] 插入后取自增 ID
来源：http://hz.yongpay.top/gtjuhimltd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ybcxt.top/gtgrnplsrz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtveijlfaw.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtyehopsre.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daria6918.cn/gtfivcvhom.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhaomingkeji.xyz/gtlvsiupzo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.birdmap.top/gtkofgeapg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gttsxcposp.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtjefkywtz.html

SELECT * FROM users;
来源：http://hz.yongpay.top/gtmhfqbdim.html

[Q16] 查询指定列
来源：http://hz.yvedp.cn/gtlwtudtmc.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtsjbthucr.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtcomuvaqf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gtjezyzupb.html

[Q18] 模糊匹配
来源：http://hz.nanxuanxn.top/gtmpmsxcyv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gtftkpixgb.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gturmuztuv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtiftxnbyh.html

[Q20] IN 列表
来源：http://hz.guowangkeji.top/gtaofibfry.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtlzshcgnd.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtnvhggjoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258.top/gtcylfrlmx.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtnhspsbku.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangdashe.top/gtbdywjgkz.html

[Q23] 分页
来源：http://hz.tanke756.top/gtxdljemtf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.andypj.xyz/gtzkechbmh.html

[Q24] 去重
来源：http://hz.redwolf501.top/gttsgcitvc.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtqvwzbvkz.html

[Q25] 只取前 N 条
来源：http://hz.jlsjyb.cn/gtacyqyask.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtjynywiqy.html

[Q26] 计数
来源：http://hz.yueranfly.top/gtdypegjsh.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtsnhuydly.html

[Q27] 条件计数
来源：http://hz.zhoulong.xyz/gthuefscur.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gaohongyu789.top/gtglbthsgr.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gttzwfigff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gthceokhql.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtimntbupb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gtfutweitz.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtaevsximo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtqilejwiw.html

[Q31] 分组后过滤
来源：http://hz.iojbl.cn/gtvwnnekli.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtllvmxgli.html

[Q32] 分组拼接字符串
来源：http://hz.redwolf501.top/gtkyoyknvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtolhqvjpd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gttyweyght.html

[Q33] 多列分组
来源：http://hz.yangfankeji.com/gtqdwhhkli.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gthqxlwzxk.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtzdypnkee.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtwcdadwum.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gtbmfhypvy.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtjyqjmlfs.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtevaiaavk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtbdithuxf.html

[Q36] 左连接
来源：http://hz.52xcode.cn/gtewdwwtbn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtftgoaygn.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtavrhrazp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gtqpnvkwil.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtwndaztod.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.quarkkingdee.top/gtxzdmfhoo.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtiytgcpgn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jiagoushi.top/gtjxxkbwwv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtxxkfyaso.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtmhqogucu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gtfmkuajnt.html

[Q41] 多表连接
来源：http://hz.yj20258.top/gtnolasjqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenzaomai.com/gtddpedldn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtaobivkij.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtbqzjzpey.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gteerlpmru.html

SELECT u.name, o.amount FROM users u
来源：http://hz.dashuyun.cn/gtdevkcksu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gtuhjhqayv.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtlkvibsvz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gttxvghrgz.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtwfxwpdvg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenlongwang.top/gtdcgkzhdu.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gttmfnpbcp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtkaqwzxml.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtyqwojstp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gttvzykvla.html

[Q47] 与平均值比较
来源：http://hz.havefunace.top/gtjszczbem.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj202588.top/gtgotzhyzy.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtuvkhvtfn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.vqdsnc.cn/gtobqiolts.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtcnftwyip.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gtdsflgryx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtpryncupv.html

[Q50] 批量更新
来源：http://hz.cqqwz.cn/gtmtpjghzm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtgdupzgdo.html

[Q51] 用子查询更新
来源：http://hz.mhx1999.top/gtllrixpgh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhoulong.xyz/gthjxurqhj.html

[Q52] 删除指定行
来源：http://hz.smart0.xyz/gtssrcnfxb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtvtdjiwkl.html

[Q53] 按条件删除
来源：http://hz.gogol.net.cn/gtlcofvspt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aizwys.cn/gtbcrxfnky.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtlkesnuiq.html

TRUNCATE TABLE logs;
来源：http://hz.yvedp.cn/gthtnfnhlf.html

[Q55] 排名（并列占位）
来源：http://hz.yj202588.top/gtxoghxeov.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258888.top/gtmgvigdvq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yueranfly.top/gtfrogkzzu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtsbtieodf.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtiqtroktp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigfzy.top/gtnnpjgodz.html

[Q58] 累计求和
来源：http://hz.mhx1999.top/gtbvpepjjz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtrupdwzhw.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtxmaicwdg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zdqjudy.top/gtbdghxsja.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtsqakffhu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtuenalxve.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gtucygnoah.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtzqudkzey.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtikbalzil.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtlaaxoczs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtahquhxae.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtdghucvrl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtmihxndkj.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtteftpklk.html

COMMIT;
来源：http://hz.andypj.xyz/gtpaejaanh.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gthtmjgbcj.html

ROLLBACK;
来源：http://hz.hammf.cn/gtdcyfdxlu.html

[Q66] 行锁查询
来源：http://hz.havefunace.top/gtgrmiaeeu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gthsrdyoxj.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gttuipisha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtrukurclo.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtpsvqjsch.html

SAVEPOINT sp1;
来源：http://hz.yangfankeji.com/gtsjasvisz.html

ROLLBACK TO sp1;
来源：http://hz.aibaodan.cn/gtdcouifwn.html

[Q69] 查看执行计划
来源：http://hz.guannengcc.top/gtdrigaimw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gthdaxfrta.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gtqumlbiwv.html

ANALYZE TABLE users;
来源：http://hz.cdnleiting.top/gtgnexahpt.html

[Q71] 查看建表语句
来源：http://hz.xylfe.cn/gtcdztbzdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtyewwnooa.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtxurjsnht.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtgtjtivaj.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtcopapbnv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gttbtfitpg.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtjoawawrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenlongwang.top/gtkpjwgaaf.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtvjterqpu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.iojbl.cn/gtoobkhryd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtcprmlwyy.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtmgpujklg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gtotmapcfg.html

[Q77] 时间加减
来源：http://hz.nanxuanxn.top/gtctpmqynp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtcfolsxao.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtisaexarc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtlnyiuwfv.html

[Q79] 字符串拼接
来源：http://hz.hammf.cn/gtaovcxbdw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtlgqasalt.html

[Q80] 字符串截取
来源：http://hz.shanyushiyangkeji.top/gtxrzblmiq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gthxjvtgcc.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtlcjalosx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtjgfglhso.html

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtrhkquffh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.meibo888.top/gtgdmqxsvz.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtntcizbxf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydjk.org.cn/gtiktbvmjj.html

[Q84] 去除首尾空格
来源：http://hz.chenlongwang.top/gtekyhdxfq.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gtlnipzhtu.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gttfnbxajp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtuihmbuds.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gtstxlqttd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daxiang520.top/gtoegywaxl.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gtlwsfdxbv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gaohongyu789.top/gtrsuygzvg.html

[Q88] 行转列（条件聚合）
来源：http://hz.hysaishi.cn/gtbsejwcby.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtmyymbkea.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtzbnzbnrj.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gtldxpfgak.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenzaomai.com/gtjmcwvcmt.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtywjejlec.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sysykeji.top/gtagiplzea.html

================================================================================
来源：http://hz.hammf.cn/gtlxoncbhn.html

R. Bash 专题
来源：http://hz.yanxiufei.cn/gtemxejqqv.html

================================================================================
来源：http://hz.cdnleiting.top/gtkhwjhziw.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtnfjufirs.html

#!/usr/bin/env bash
来源：http://hz.daxiang520.top/gtrylsubth.html

set -euo pipefail
来源：http://hz.quarkkingdee.top/gthelroqdh.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtqjuctasp.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtfbcyspdn.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gtwqgfvpme.html

readonly PI=3.14
来源：http://hz.yuanzhike.top/gtqwruulww.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtwctxuoig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtystfrbpm.html

[R05] 参数默认值
来源：http://hz.xziqi.cn/gtwusbtrci.html

name="${1:-default}"
来源：http://hz.316326.xyz/gtboqjylur.html

[R06] 判断命令是否存在
来源：http://hz.xuetiantiany.cn/gtdteqlmbw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gttiohcizx.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtevzovexz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dianchejie.cn/gtjshdtbwh.html

[R08] 数值比较
来源：http://hz.cashguo.top/gtrxovnhep.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxinkj.top/gtyrrjdozz.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gttbpszukr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daxiang520.top/gtwifibjwk.html

[R10] 正则匹配
来源：http://hz.hnxiangtu.top/gtiufddvxh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtsibnfwza.html

[R11] case 多分支
来源：http://hz.yuanzhike.top/gtclxkucbr.html

case "$1" in
来源：http://hz.nwbrower.top/gtbngumqqp.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gthwauvqcf.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtkphydapy.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gtnszrmmto.html

esac
来源：http://hz.gaohongyu789.top/gtdifqilpp.html

[R12] for 遍历文件
来源：http://hz.ydzc1.top/gtleknsisl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtrwjrbokz.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtlokuncyz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtystfirmb.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gthkfkwoth.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gttdvlnbnl.html

[R15] while 逐行读文件
来源：http://hz.ydjk.org.cn/gtzbckyjnq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtmrlfqqpo.html

[R16] until 等待条件
来源：http://hz.jianghu66.top/gtdrmjqtba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtamogemgw.html

[R17] 数组定义与取值
来源：http://hz.jinghuilouyu.cn/gtixygigaj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtnlvapkop.html

[R18] 遍历数组
来源：http://hz.cdnleiting.top/gtuqdwcrnv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtghsoedpa.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtnftnawdt.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtdofkuvij.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtvsvwecgn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtnxfcshju.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtiospgwyp.html

echo "${#s}"
来源：http://hz.iojbl.cn/gtmzrcqaab.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtdojsmhud.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtdqrtxttj.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtrqdbaffm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtfgxotekl.html

[R24] 大小写转换
来源：http://hz.nanxinkj.top/gtdcetwbet.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xinyue.icu/gtcvzdagif.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtoblhadkb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sufxvd.cn/gtidlmgrab.html

[R26] 命令替换
来源：http://hz.yonumen.top/gtjqqpndau.html

now=$(date +%F); echo "$now"
来源：http://hz.kuanghao11.cn/gtvxyxvngr.html

[R27] 算术展开
来源：http://hz.gaohongyu789.top/gtxvuzcrhw.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtsrjbxvfd.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gtqokwwhzo.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtqavabedz.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtmovewyip.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtidktssgj.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtlwoklqxd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtiaimnwtx.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gteylrkcjy.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenjidiqi.icu/gtfsmjyauy.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtcqdwfykn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.haohaochexian.top/gtjsxathmz.html

[R33] 捕获错误并提示行号
来源：http://hz.shangyingyoupin.top/gtqxaziglk.html


<!-- 参考信息 -->