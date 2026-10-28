代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhaomingkeji.xyz/gtsmxdwxjg.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gtqgafyohv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtjmsatifk.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtawgfzddw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhaomingkeji.xyz/gtgmbeijrg.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtpjzwaqoi.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gtzdwqeyub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinyuanbaomall.cn/gtildumikx.html

PHP:  // 手写时间戳比较
来源：http://hz.aibaodan.cn/gtellwxeht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtmcrcxamw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtflerqxby.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtsptwfryj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtntgpzosj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtqadbrbub.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jiagoushi.top/gtphqamnho.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtwgadvpvo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtzjkymwao.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yongpay.top/gtmcayazvs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtnlmliisf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtqfreqarv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtzifibqvf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.andypj.xyz/gtgleiqjfj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtutmpcprt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtnovtzrzd.html

================================================================================
来源：http://hz.sweek.top/gtdouyikum.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuanzx.com/gtniayonpl.html

================================================================================
来源：http://hz.iojbl.cn/gtpkdazoio.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtgvymutbk.html

CREATE TABLE users (
来源：http://hz.chenzaomai.com/gtcvdlwivx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtgbhjsjbh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.havefunace.top/gtptfypsdx.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtabeljmei.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtbbvxceka.html

);
来源：http://hz.ppjwa.cn/gtwiqcjobd.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtfkxeahto.html

CREATE TABLE orders (
来源：http://hz.pengpengdd.cyou/gtoknjesli.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtgwarcetf.html

user_id INT NOT NULL,
来源：http://hz.ydjk.org.cn/gtcasaarlj.html

amount DECIMAL(10, 2),
来源：http://hz.ydzc1.top/gtuxbysofb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydjk.org.cn/gtxiszhbdy.html

);
来源：http://hz.tanke756.top/gtezbpibbv.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gthcwtxovy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtahheujbx.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtinjczwnd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gtruxrvbcj.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtrrvdgcai.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtiyomhfof.html

[Q06] 删除列
来源：http://hz.zdqjudy.top/gtotdswayp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtfbkewyrn.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtmmfyapbw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenjidiqi.icu/gtqvwekyol.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtgodwulbc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtfhrrwsvf.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtvtyudwch.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtlalckisb.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gtmgtdjfyt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sweek.top/gtaedzqlqx.html

[Q11] 一次插入多行
来源：http://hz.zhijiandao.cn/gtdswkihrf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtkesxztpf.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtkwvwpmch.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtnztfklwr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xylfe.cn/gtakpcdcxj.html

[Q13] 忽略重复插入
来源：http://hz.hfpthk.cn/gtmcfgkryi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yueranfly.top/gtmxzspeak.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtccncbiwb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.0kj1m.cn/gtdbioprsp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jianghu66.top/gtxdkxqjyh.html

[Q15] 查询全部
来源：http://hz.daxiang520.top/gtpsumqprl.html

SELECT * FROM users;
来源：http://hz.zycfv.cn/gtcgopyomy.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtflrimmqp.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtlknjsmzd.html

[Q17] 条件查询
来源：http://hz.hammf.cn/gtsjwcuqgc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shzxlz.cn/gtmzrhegyz.html

[Q18] 模糊匹配
来源：http://hz.jinyuanbaomall.cn/gtyckegilm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtnmxglkhj.html

[Q19] 范围查询
来源：http://hz.hywenlv.cn/gtncdeymkj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.gaohongyu789.top/gtrqjbcqqg.html

[Q20] IN 列表
来源：http://hz.ydzc1.top/gtjmfqtesp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.meibo888.top/gtrcmpwlpz.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtpshomzdj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.birdmap.top/gtfovpmxdg.html

[Q22] 排序
来源：http://hz.jqgfzy.top/gtwqisedjl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangdashe.top/gtlwcgzoep.html

[Q23] 分页
来源：http://hz.xziqi.cn/gtzdgqzlky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gthawlwvyx.html

[Q24] 去重
来源：http://hz.ydzc1.top/gtzrjczkai.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinghuilouyu.cn/gtoequfrfx.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtydfbepjp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtwpolgjdx.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtgzenwjhg.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtoemtbxpa.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtwjglrrkb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xinyue.icu/gtkkdmobrr.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtocdmquqj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtexzicvtb.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gticaappbl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtwgtkjvxr.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtqhwaobzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtzkagleeg.html

[Q31] 分组后过滤
来源：http://hz.yangfankeji.com/gtgzdlsjgk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtxjgionyx.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gthzelwrxb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtsnhkniad.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtgsnhelnj.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtoahpivoy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gtneppjgmu.html

[Q34] 每组取第一条
来源：http://hz.guannengcc.top/gtrkpyjacz.html

SELECT * FROM (
来源：http://hz.hysaishi.cn/gtwjojkote.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtfzenuzmi.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gthfdkfmpr.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gteqblmbdk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtdmmoobyz.html

[Q36] 左连接
来源：http://hz.jlsjyb.cn/gtpbzpvxgr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtalayrfyh.html

[Q37] 右连接
来源：http://hz.gzhubu.top/gtoevhfykl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtdyszhjaa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.iojbl.cn/gtykgpfzqx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhixingplan.top/gtmngiipee.html

[Q39] 自连接（查上下级）
来源：http://hz.snrcjt.cn/gtdzqpowuq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtxhqdwrnm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.wangdashe.top/gtskmpwsfo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtsarytnze.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtmbbqkifp.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtejcuwcgn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ppjwa.cn/gtgovmtlog.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnqzz.top/gtxfuozwqz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtcrdliymb.html

[Q42] 连接条件附加过滤
来源：http://hz.fengsongda.top/gtcedfdsoe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258888.top/gttqcyejza.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnqzz.top/gtjaezfumo.html

[Q43] 标量子查询
来源：http://hz.jyoumei.cn/gtnwbnbexi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.haohaochexian.top/gtutltukzo.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtliiqqxcy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtairfqgmn.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gtrkltyoku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gtfcavximx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtjdfpsnzl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtaclueleu.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtmkyaqhii.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtfnagvsvt.html

[Q48] CTE 公用表表达式
来源：http://hz.cheryme.top/gtxhajksco.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtkzcggbqj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.0kj1m.cn/gtjpjvpihp.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtfrnpqeox.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtphdfzcxw.html

[Q50] 批量更新
来源：http://hz.meibo888.top/gtkxdvlapp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xziqi.cn/gthctxrvlk.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtvlucawzt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtelqpcdmk.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtmfxqxnln.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtrkjkqnya.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtacantydd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yangfankeji.com/gtvcopgmte.html

[Q54] 清空表
来源：http://hz.shzxlz.cn/gtcepqqytf.html

TRUNCATE TABLE logs;
来源：http://hz.xziqi.cn/gtwkeywvzw.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtbiewmema.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yongpay.top/gtvbpeohcv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtrjwsolfe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtkuhbgjty.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtcqaxdszm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuxming.cn/gttqgnjnds.html

[Q58] 累计求和
来源：http://hz.sufxvd.cn/gtshwkfawa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtfhctcdkl.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtvysjcfxh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtlqkykojv.html

[Q60] 取上一行 / 下一行
来源：http://hz.tian-w.cn/gtqpieyenj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtzymujwqn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtqcftanga.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtsnqmjzqr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shzxlz.cn/gtypetszjy.html

[Q62] 分组占比
来源：http://hz.gaohongyu789.top/gtvvwpsnmj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtddxwlhlx.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtvkkbybeu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtldyafhol.html

[Q64] 提交事务
来源：http://hz.gotoacloud.top/gtwtccqjat.html

COMMIT;
来源：http://hz.hysaishi.cn/gtggxsqgzh.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtdbxeewcu.html

ROLLBACK;
来源：http://hz.ivvv.top/gtfpwllwho.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtyxhvlxbt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bjfxy.top/gtbyizweef.html

[Q67] 设置隔离级别
来源：http://hz.zhiwuduotai.top/gtxnxinqge.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sxryk.cn/gtoitjuyrw.html

[Q68] 保存点
来源：http://hz.zhijiandao.cn/gtplpgrkuj.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtsczgnwut.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtzabxwcwh.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtsajdmalq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ehwqpu.com/gttetmqpup.html

[Q70] 更新统计信息
来源：http://hz.jinyuanbaomall.cn/gtxzcytiig.html

ANALYZE TABLE users;
来源：http://hz.shuidangran.top/gtkbjhrjax.html

[Q71] 查看建表语句
来源：http://hz.0kj1m.cn/gtnkkrfjll.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtbydhjdzp.html

[Q72] 查看索引
来源：http://hz.smart0.xyz/gtegpnchnc.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtawsmugup.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtxbuxctsa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtyrzfhypg.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtpqccvmdo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtaprsapga.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtpxtkmlyj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.quarkkingdee.top/gtpeiiwucn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtnyhppmim.html

[Q76] 按天统计
来源：http://hz.yonumen.top/gtujdrlhol.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtyzpxxmtv.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtfqwrtxop.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtfsgliprz.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtxitmglhx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtirgdkazo.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtbnnpwmvn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ppjwa.cn/gtwivaqpqc.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtactmyfkm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtwqauyjyi.html

[Q81] 字符串替换
来源：http://hz.birdmap.top/gtdvmsjwsp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhixingplan.top/gtnlezduqw.html

[Q82] 字符长度与字节长度
来源：http://hz.dashuyun.cn/gtfzadkhvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtdzlvitsd.html

[Q83] 大小写转换
来源：http://hz.yuxming.cn/gtifysnejo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtixuhrmpq.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtiffspjos.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtvtaspvkz.html

[Q85] 数值取整
来源：http://hz.zycfv.cn/gtjtgjeliy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtjsgbgxbb.html

[Q86] 读取 JSON 字段
来源：http://hz.quarkkingdee.top/gttdfzxwez.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydjk.org.cn/gtfmprdjbq.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gtbknqwqab.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtbjuzvftw.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtphbdkgci.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.bjfxy.top/gtooqshatc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hywenlv.cn/gtesxzkogk.html

[Q89] 判断表是否存在
来源：http://hz.ywan-chungtsiang.top/gtnzunlbzr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtllxgzsuo.html

[Q90] 生成序号列
来源：http://hz.shangyingyoupin.top/gtpybdkvzl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtxazvrgdi.html

================================================================================
来源：http://hz.tanke756.top/gtoyabktpf.html

R. Bash 专题
来源：http://hz.c1oappe.top/gtgxltlyjy.html

================================================================================
来源：http://hz.andypj.xyz/gtgjbbptux.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtoisttoqk.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtmdhvqukw.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtotwucmgd.html

[R02] 变量赋值与使用
来源：http://hz.redwolf501.top/gtrxwzdgxf.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gtndtgaanz.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtgkrzecmr.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gthhvjvluw.html

[R04] 位置参数
来源：http://hz.andypj.xyz/gtcegozhop.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtekfjysno.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtykbbggko.html

name="${1:-default}"
来源：http://hz.zdqjudy.top/gtrtiyaxxg.html

[R06] 判断命令是否存在
来源：http://hz.hfpthk.cn/gtisuzmlqc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtoiizymzv.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtjbbveqiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtmfnxfpyy.html

[R08] 数值比较
来源：http://hz.hywenlv.cn/gtztqxmjlr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtjgmsdajj.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtzkzvfedy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtjpgqsoct.html

[R10] 正则匹配
来源：http://hz.tian-w.cn/gtcqhubfkn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtvykntjco.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtvbaiyrkl.html

case "$1" in
来源：http://hz.0kj1m.cn/gtckvjtmxt.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtdspaawda.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtpuhietcm.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gtcgldakbw.html

esac
来源：http://hz.hnxiangtu.top/gtqbvmxdig.html

[R12] for 遍历文件
来源：http://hz.ywan-chungtsiang.top/gtfyxuwuxr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.snrcjt.cn/gtlcsqsnnc.html

[R13] for 计数循环
来源：http://hz.cdnleiting.top/gtuuwfytdk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtvvvqtbgg.html

[R14] C 风格 for
来源：http://hz.xinyue.icu/gtyjizihev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtkusjqioc.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtrqozrbas.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ivvv.top/gtvtfegsdd.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtryteavby.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aibaodan.cn/gtsfthessk.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtevcrfozz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtrqnhxzkf.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtvjugnlnq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pycfn.com/gttoirhwxy.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtyewqtsvm.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtrobqvsux.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtnxdjnbrw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtsloblihs.html

[R21] 字符串长度
来源：http://hz.aibaodan.cn/gtiahcrppi.html

echo "${#s}"
来源：http://hz.316326.xyz/gtkxnbikqu.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtsdzlgnyj.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtotmommxo.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gthvalllal.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daxiang520.top/gttmawkfbq.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtfhvcoeqj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtcxrrpqzg.html

[R25] 去后缀 / 去前缀
来源：http://hz.cheryme.top/gtiiijoiof.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jianghu66.top/gtrugpqolq.html

[R26] 命令替换
来源：http://hz.sufxvd.cn/gtkwgypyig.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtfwbmupqn.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtrgaxsvux.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtghfkkaqs.html

[R28] 浮点运算
来源：http://hz.fzhhl.top/gtynuhbikp.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtqfjmejln.html

[R29] 定义函数
来源：http://hz.tanke756.top/gtoamgqedj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hammf.cn/gtmekswlqu.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gtfmpqszxd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtacuxpfgq.html

[R31] 局部变量
来源：http://hz.c1oappe.top/gtgidbracm.html


<!-- 参考信息 -->