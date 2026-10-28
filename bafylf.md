代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.9152youxi.cn/gtaasypzdd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtlzntgftk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtfxkadbbj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtcvysefgq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtvcenwors.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yvedp.cn/gtfbvftggt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj202588.top/gteyzazxwe.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtvnzgwwah.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgufenzy.top/gtaerhcwvy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtkhkjcjgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtpxqenxho.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gthfzlgsjf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtlersrvzz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtofvreltw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.mhx1999.top/gtnyjmkyza.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gtgquygtek.html

================================================================================
来源：http://hz.sxryk.cn/gtzwiesxib.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tianlin.xyz/gthjgnsdfr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfkkngrbc.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtkwsnktem.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtlwboiufr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gttxxzpcbs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cdnleiting.top/gtufrjljob.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtlelkiank.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtutgeerlq.html

);
来源：http://hz.mhx1999.top/gtfncnqjzg.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtghbjiazl.html

CREATE TABLE orders (
来源：http://hz.yj20258888.top/gtbbhfnykz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtewtsswgs.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtfypawtdo.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtuadezeeu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtzzygdraw.html

);
来源：http://hz.ehwqpu.com/gtcysouulz.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtgkgrcvow.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yj202588.top/gtahfvrbpb.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtnwbalzyr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gthvgittdx.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtuhswlfhb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jyoumei.cn/gtpyslpweo.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gttlnptdbi.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtwphakcwq.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtrixxgxze.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yueranfly.top/gtnhgfrefe.html

[Q08] 创建普通索引
来源：http://hz.xziqi.cn/gtgeribfrm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shangyingyoupin.top/gtmbgwgisz.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtxrxcsjjs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtkptrqema.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtosuyreyi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtpiqapowr.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtvkxzhupy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zycfv.cn/gtstntwzir.html

[Q12] 插入后取自增 ID
来源：http://hz.ehwqpu.com/gtkblyhury.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtetmzmsjr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gtozhinewk.html

[Q13] 忽略重复插入
来源：http://hz.gotoacloud.top/gtggnmrlyo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gtqsikcoia.html

[Q14] 存在则更新（upsert）
来源：http://hz.hammf.cn/gtxvhaqcdz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtcwygbqno.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.smart0.xyz/gtkofcyeva.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gteqvcfftc.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtxavukzhg.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtoijporrl.html

SELECT id, name FROM users;
来源：http://hz.aizwys.cn/gttpzcnubh.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gtezhnhcef.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtzfeulaxz.html

[Q18] 模糊匹配
来源：http://hz.svipenyu.cn/gtbsbqxxgh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.havefunace.top/gtuxcemlct.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtelameqpx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtscimlket.html

[Q20] IN 列表
来源：http://hz.ybcxt.top/gtxgymepgy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.meibo888.top/gtekdfitsr.html

[Q21] 空值判断
来源：http://hz.ppjwa.cn/gtbvkwfqot.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtkfgjboyk.html

[Q22] 排序
来源：http://hz.zhaomingkeji.xyz/gtggesnmvm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtbyqkmbqn.html

[Q23] 分页
来源：http://hz.yj20258.top/gtmtxoudcg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhongyouzk.top/gtszajgdnp.html

[Q24] 去重
来源：http://hz.cheryme.top/gtfcssxysi.html

SELECT DISTINCT city FROM users;
来源：http://hz.cucudq.cn/gttonrxqbg.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gthyphjgov.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtdrfxhxmw.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtglvmqfej.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtfvermqhg.html

[Q27] 条件计数
来源：http://hz.feifeiyinyue.top/gtupqriwnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtcziijaur.html

[Q28] 求和与平均
来源：http://hz.gogol.net.cn/gthvnpiuun.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhongyouzk.top/gtjmbyomwj.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtegbjxbjc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.andypj.xyz/gtaqlterdt.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtvqtojufs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtlmxhjsfi.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtswnvyfhh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gttykjsvmz.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtswrowpjl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtgztfqaxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xinyue.icu/gtaxjomylj.html

[Q33] 多列分组
来源：http://hz.zhaomingkeji.xyz/gtaoruvyku.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhiwuduotai.top/gtgygdqwua.html

[Q34] 每组取第一条
来源：http://hz.pengpengdd.cyou/gtihlvuvyk.html

SELECT * FROM (
来源：http://hz.gaohongyu789.top/gtqxbdmrnj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtbxedrhvr.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gtltrzvwgt.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtlhjsufwa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gteclzzlon.html

[Q36] 左连接
来源：http://hz.wangdashe.top/gthvmzbjao.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtykmkpeex.html

[Q37] 右连接
来源：http://hz.ydjk.org.cn/gtjkaqygvk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shangyingyoupin.top/gtiufezjim.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gaohongyu789.top/gtbpwcdnfk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jiagoushi.top/gtmxsjfdih.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gtchqslvfx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtfiswlbzg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxuanxn.top/gtkwqmjqft.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cdnleiting.top/gtpnlkvzlu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj202588.top/gtolazbkos.html

[Q41] 多表连接
来源：http://hz.zhaomingkeji.xyz/gtwhmnogno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtyxmlnxah.html

JOIN users u ON u.id = o.user_id
来源：http://hz.c1oappe.top/gtsdoyumxs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.wangshuangyany.cn/gtaxmhtzhv.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtqjewrzqv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhengqikj.top/gtflrnkiok.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gthhppvmmn.html

[Q43] 标量子查询
来源：http://hz.haohaochexian.top/gtljmpbdeg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhongyouzk.top/gtdiostyiw.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtbtzjgiwc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtxsdtzvmi.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtkuylhliy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtpkqrapez.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sweek.top/gtiyyiwsbk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtrssclsri.html

[Q47] 与平均值比较
来源：http://hz.gogol.net.cn/gthnrxyovx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yvedp.cn/gtnkfggnmu.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gtzhuuosks.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtjhawubrw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yvedp.cn/gtvocdigeo.html

[Q49] 更新单行
来源：http://hz.zycfv.cn/gtbhwocgfr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtsidzrmwj.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtkdtxpmus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hywenlv.cn/gtuuaacfcx.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gthawahjkf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sufxvd.cn/gtopuiptbf.html

[Q52] 删除指定行
来源：http://hz.zhongyouzk.top/gtflzsfeto.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dashuyun.cn/gtgdoyyxoi.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtsrdtlwov.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.redwolf501.top/gtlykbhgwa.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtpnugwuvg.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtbmulrvhi.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtjoofvcww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hongshengwenyu.top/gtfrdfynqo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtmssmetwg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtmrtfcvve.html

[Q57] 行号
来源：http://hz.redwolf501.top/gtcxcpgmkb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtqcjufiah.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtkcoduzya.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtnulppqjx.html

[Q59] 分组内累计
来源：http://hz.jinyuanbaomall.cn/gtwsiqhoyr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtjaekbpsd.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtjapswein.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtxeeppslp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtdokkrozf.html

[Q61] 移动平均
来源：http://hz.dashuyun.cn/gtvyhsvnxg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cqqwz.cn/gtuspcmpxp.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtmxtimvfn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtdgyjsneu.html

[Q63] 开启事务
来源：http://hz.jinqigfzy.top/gthdbmxaca.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.pycfn.com/gtqdvrplzp.html

[Q64] 提交事务
来源：http://hz.sweek.top/gtgzkjsgqu.html

COMMIT;
来源：http://hz.xuanzx.com/gtlnlwgjyv.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtpgowhbqo.html

ROLLBACK;
来源：http://hz.pycfn.com/gtqgusvdjg.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gtnkmxhsxg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gtsdqfwvsp.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtiitafsft.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gthndbgxps.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtrtevjwtz.html

SAVEPOINT sp1;
来源：http://hz.9152youxi.cn/gttnwxafmj.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtkibsqqdc.html

[Q69] 查看执行计划
来源：http://hz.quarkkingdee.top/gttlfjqwvu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtncoluhsr.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtmuyqchfl.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtjprwxcnu.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtzkxovebl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gttkjwpcfv.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtajzrpkio.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gtcvsdtfsw.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gttdbxjhoe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gthbgxlhlc.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gttqmiioyp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtuhzvhych.html

[Q75] 日期格式化
来源：http://hz.aibaodan.cn/gtxwzvgkia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtlymzbbbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinghuilouyu.cn/gttqiisjwq.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtfswqrbeo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gteaijleow.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtpqmyjxpx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yanxiufei.cn/gtusbpdfap.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtmjqewzqo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gtctfxibuk.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtiahsqakt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtccrmcnzx.html

[Q80] 字符串截取
来源：http://hz.hammf.cn/gtuzlpiswl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtuowrngxn.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtsdsyxijd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gtjalyxuxk.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gtcjuznjrr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ppjwa.cn/gtprxxksnd.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtpidgxvim.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtnpwjcndu.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtquxhnjjw.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtccywqknn.html

[Q85] 数值取整
来源：http://hz.andypj.xyz/gtppdadmpq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jyoumei.cn/gtoxnjlupw.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtlfewvobd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtddwklxvw.html

[Q87] JSON 字段做条件
来源：http://hz.ywan-chungtsiang.top/gtwcciuqky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtypqeqldx.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtofomdqtx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtelseabrn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtdodmyxjn.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gttwqemonn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yanxiufei.cn/gtguqglwar.html

[Q90] 生成序号列
来源：http://hz.xuanzx.com/gtsxrjmrcf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nanxinkj.top/gtfaeovbvx.html

================================================================================
来源：http://hz.yvedp.cn/gtfpsrouxb.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtziwtdoss.html

================================================================================
来源：http://hz.hfpthk.cn/gtxfknxcdn.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtezohxbaq.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gthdcouimn.html

set -euo pipefail
来源：http://hz.sweek.top/gtyujqlvjo.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtsdigtjhi.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtdjzwqzhn.html

[R03] 只读变量
来源：http://hz.zhaomingkeji.xyz/gtajnujqaq.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gthxgfuajg.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtnwxqvefk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtqmkuhgfw.html

[R05] 参数默认值
来源：http://hz.tanke756.top/gtkbhqpntf.html

name="${1:-default}"
来源：http://hz.andypj.xyz/gtqogzukju.html

[R06] 判断命令是否存在
来源：http://hz.0kj1m.cn/gtutwzsutd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtguaqkdad.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtmuwunjly.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hammf.cn/gtzduehcct.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtibtrhwwo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtjfnluvck.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtksrptkhy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtyepzjlet.html

[R10] 正则匹配
来源：http://hz.guannengcc.top/gtpdgaazyf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cashguo.top/gtzvnjjvph.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtatosxjjp.html

case "$1" in
来源：http://hz.cdnleiting.top/gtrwxtwyba.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtxnwzrbfg.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtdfxmflvx.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtpiasutaq.html

esac
来源：http://hz.ywan-chungtsiang.top/gtlcmafiue.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gtmqywkpqc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtcknlbait.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtwgkualpd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sweek.top/gtvkybelmb.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gthmvaimsb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtxkgbvvby.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtmoabqjyx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxuanxn.top/gtrhrrmhgk.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtwjuvafgv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shuidangran.top/gtrxwdhvrd.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtyhkqqduz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtpexjmuaf.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtdonzborp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.iojbl.cn/gtnjkydlbe.html

[R19] 数组长度
来源：http://hz.sysykeji.top/gtebnnalth.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtpsgruxcg.html

[R20] 关联数组（字典）
来源：http://hz.zycfv.cn/gtccnttpjw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gttcevuvjn.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtpogzmnts.html

echo "${#s}"
来源：http://hz.xingfuxueyuan.xyz/gtadgnkbkp.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtzpuzvyke.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtrpjjhtmr.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtwpsrzylo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shanyushiyangkeji.top/gtohbcpzqg.html

[R24] 大小写转换
来源：http://hz.gzhubu.top/gtggxnsnzg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yueranfly.top/gtbdjbfjcd.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtkgimrcpk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtfsjwnfgt.html

[R26] 命令替换
来源：http://hz.jqgufenzy.top/gtjrzedgkr.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtzimlehac.html

[R27] 算术展开
来源：http://hz.c1oappe.top/gtzbohoabs.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtavsyiuej.html

[R28] 浮点运算
来源：http://hz.9152youxi.cn/gtwhnvsxum.html

echo "scale=2; 10/3" | bc
来源：http://hz.bjfxy.top/gtjdkvyfut.html

[R29] 定义函数
来源：http://hz.yanxiufei.cn/gtyssbtylb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtvmolirgv.html

[R30] 函数返回状态码
来源：http://hz.daxiang520.top/gtierfdvos.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtxiqrsvak.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtuobhriwz.html

f() { local x=1; echo "$x"; }
来源：http://hz.meibo888.top/gtialygjov.html

[R32] 参数个数校验
来源：http://hz.andypj.xyz/gtckmgtcxx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtxlbolcpf.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtkafnxcng.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtuceoksae.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtcyujezmx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gthuryjeaf.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtqvczpkhb.html


<!-- 参考信息 -->