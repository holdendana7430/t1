代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxinkj.top/gtpiuluziz.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtahjlnpdy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtycwefivs.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtciisbaqf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigufen.top/gtfayrqpgo.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtbyqnloqs.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtvstnstpl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtqduvwchv.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtvrcnosjf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtoirzqpnv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtjiqefsen.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.c1oappe.top/gtlcqetwtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtzmwppwhv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.andypj.xyz/gtdcntscou.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gtmznllnng.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gtpteyakrl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtiqrkxwee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cdnleiting.top/gtmqvmjhoq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtegqkyblp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtgwraggsp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtswwlregq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gtslwgwjdf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zycfv.cn/gtoamvhlra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtsogtglst.html

================================================================================
来源：http://hz.cheryme.top/gtddtitlff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuanzx.com/gtvjsbwjxe.html

================================================================================
来源：http://hz.cqqwz.cn/gtjbjeenzw.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtmkwfgzfr.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtikngqjbz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtpabqrvro.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258888.top/gtagfisgqc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtrdjaryhh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aizwys.cn/gtltpxawen.html

);
来源：http://hz.guannengcc.top/gtzqqrdzkr.html

[Q02] 创建带外键的表
来源：http://hz.kuanghao11.cn/gtigjvkzgi.html

CREATE TABLE orders (
来源：http://hz.sufxvd.cn/gtwktqrvmc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtvcdiuoao.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtovynfbnx.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtrapmeqib.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gtflxjbixo.html

);
来源：http://hz.sysykeji.top/gtdcjqvpyf.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtxtwjxfom.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtpvimqgxp.html

[Q04] 修改列类型
来源：http://hz.52xcode.cn/gtaohhmtim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtbnyfwski.html

[Q05] 重命名列
来源：http://hz.yangfankeji.com/gtyssnlatf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtzbfarvhm.html

[Q06] 删除列
来源：http://hz.cashguo.top/gtsbwisqsx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtulvzynbk.html

[Q07] 删除表
来源：http://hz.haohaochexian.top/gtmihcsfhe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtgmpqjfbi.html

[Q08] 创建普通索引
来源：http://hz.smart0.xyz/gtpbvnhbsd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.9152youxi.cn/gtyquvgluc.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtccjqghul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ydjk.org.cn/gtrsqwfwef.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtiddwksyp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hammf.cn/gtvadaxhkt.html

[Q11] 一次插入多行
来源：http://hz.nanxinkj.top/gtplhwgfnz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtmsudfiag.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gtsgsdliue.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtvmvbeohn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gthttuzvza.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gthmehrzfs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zycfv.cn/gtuhnygnvz.html

[Q14] 存在则更新（upsert）
来源：http://hz.yueranfly.top/gtdgqhxlnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjfxy.top/gtcjgqiwdf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtnuefoxyv.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtvaqddfsl.html

SELECT * FROM users;
来源：http://hz.hfpthk.cn/gtymshafnj.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtgqbwpzzr.html

SELECT id, name FROM users;
来源：http://hz.ydjk.org.cn/gttywvndpx.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtyfxjzbwk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtvujjykax.html

[Q18] 模糊匹配
来源：http://hz.hammf.cn/gttikdypsc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtejolhciu.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtdwaxytwg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuanzhike.top/gthunnswgr.html

[Q20] IN 列表
来源：http://hz.shuidangran.top/gtphmmuncg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.0kj1m.cn/gtcpdwwqjx.html

[Q21] 空值判断
来源：http://hz.hywenlv.cn/gtdaswlqrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhengqikj.top/gtrqjvtmti.html

[Q22] 排序
来源：http://hz.shuidangran.top/gttewvstqp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtmzysmehf.html

[Q23] 分页
来源：http://hz.nwbrower.top/gtdtmeyrlo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtwfxanfsp.html

[Q24] 去重
来源：http://hz.cucudq.cn/gtdrhucjuc.html

SELECT DISTINCT city FROM users;
来源：http://hz.c1oappe.top/gtxvuibxsd.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtbcdarqfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtzmfmnlic.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtkizpdmiv.html

SELECT COUNT(*) FROM users;
来源：http://hz.tian-w.cn/gthdcybvvh.html

[Q27] 条件计数
来源：http://hz.gotoacloud.top/gtwgwqyuen.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yvedp.cn/gttxolsyrs.html

[Q28] 求和与平均
来源：http://hz.xingfuxueyuan.xyz/gtmbzyzmkf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gthiilkukb.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtnugmutyi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gteelpikbh.html

[Q30] 分组统计
来源：http://hz.xingfuxueyuan.xyz/gtenfzxuzp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtflafugpp.html

[Q31] 分组后过滤
来源：http://hz.jinqigufen.top/gtydposcqt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gaohongyu789.top/gtceihpexa.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtrvoqvdwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gttotfxjti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.9152youxi.cn/gtkghvqevr.html

[Q33] 多列分组
来源：http://hz.shanyushiyangtech.top/gtiaytmduj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtvoteenxl.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtdzmqnknm.html

SELECT * FROM (
来源：http://hz.wangshuangyany.cn/gtrxmbhmjv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhijiandao.cn/gtwhnwaaxx.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtpaevflbb.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtbeyejlcg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtdguttlny.html

[Q36] 左连接
来源：http://hz.316326.xyz/gtnkrvqazf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtsnkyvagi.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gtwfvqomgf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtilhfemsa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xingfuxueyuan.xyz/gtbjfhprwi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtqmtoccmy.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtokqdukmq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gtbbpyjbym.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtalorqbij.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtyydttqwf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtnqecozmz.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtwgohqwso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.birdmap.top/gtafhvislz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtlxsenchz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hfpthk.cn/gtezhkkdsi.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtnujaqgbw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.wangshuangyany.cn/gtpjjkawjb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtbqtqwcwm.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtcfpsybiu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dashuyun.cn/gtzpuymvpw.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtdbtttoxr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nwbrower.top/gtbkeitdzz.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtimgtrvop.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gttwhplsge.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gthgvuehys.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jlsjyb.cn/gtuzjqdnmt.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtobzgqpfn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuanzx.com/gthssunzcw.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtaubkyyiv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtkikboarr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtiyxnqgys.html

[Q49] 更新单行
来源：http://hz.nwbrower.top/gthimjmnlu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tian-w.cn/gtmxdhduze.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtuxxtbpnj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cucudq.cn/gtnfgnzlbt.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtjjsgzozi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gttybwrgwk.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gttzrvgprl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtmzybopan.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtdoervgun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtxjacmaxa.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtpboebjeu.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gthllgveow.html

[Q55] 排名（并列占位）
来源：http://hz.hongshengwenyu.top/gtfylcyeqs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtibpnheiw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.meibo888.top/gtenrclhno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtzgkhrhlg.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtdvpjnaqe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnxiangtu.top/gtrfopaxjq.html

[Q58] 累计求和
来源：http://hz.chenlongwang.top/gtklgjwacy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtrjwquyrn.html

[Q59] 分组内累计
来源：http://hz.cashguo.top/gtfrjwixgm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cheryme.top/gtygoernsn.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtijotbpgo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtuwruyqqt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnqzz.top/gtjdwktvar.html

[Q61] 移动平均
来源：http://hz.cucudq.cn/gtftwhcuuw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtlzdluqbv.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtrbiyynqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtlbqydsxl.html

[Q63] 开启事务
来源：http://hz.9152youxi.cn/gtaflgkuxc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtyrzdtuvc.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtutimgeqi.html

COMMIT;
来源：http://hz.ivvv.top/gttoomodca.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtjgzsxkyy.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtaounbxzi.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtlldocoht.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtgemvzziz.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gterofmqnw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gteyhampsp.html

[Q68] 保存点
来源：http://hz.dianchejie.cn/gtgnleqvov.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtkcntvszj.html

ROLLBACK TO sp1;
来源：http://hz.xziqi.cn/gtxnsbfwgo.html

[Q69] 查看执行计划
来源：http://hz.cheryme.top/gtamvdktze.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtpsuonwfc.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtuwotdbmd.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtzpbgkorz.html

[Q71] 查看建表语句
来源：http://hz.jqgufenzy.top/gtfehlqnft.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtkuauhkqq.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtnotuomca.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gthagntqdi.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtzgqlfteu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gtrrmabqhd.html

[Q74] 强制使用索引
来源：http://hz.sxryk.cn/gthtxsliow.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtrizsznsk.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtsyzznsey.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgufenzy.top/gtyerrgckn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtxfikdydr.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtclcrdsrf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtrqtqxiap.html

[Q77] 时间加减
来源：http://hz.fengsongda.top/gtpisgukah.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtlkgblbti.html

[Q78] 当前时间
来源：http://hz.shzxlz.cn/gthznoegzt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtkfwamwus.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtcfujexcg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gtaloysmfx.html

[Q80] 字符串截取
来源：http://hz.jlsjyb.cn/gtxyvdvnpg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtfitagkwf.html

[Q81] 字符串替换
来源：http://hz.chenlongwang.top/gtofblpuww.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cashguo.top/gtinzfnbkh.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtkoqmarwp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtlbvjmhyj.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtbkhnwsii.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtbmgoldxj.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtqpyuejup.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtvchcioio.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtiudithww.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gtjvattyer.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtulmlguok.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pengpengdd.cyou/gtfgmtakxw.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtwlbylity.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gtbtvwcros.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtyrlophah.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtrepwakhf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtdveznozi.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtuttxquth.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtpamdahsi.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtaxaenmre.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pycfn.com/gtvdslhmwx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjpgzxqtq.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gtryxrmwzh.html

================================================================================
来源：http://hz.hywenlv.cn/gtoxkqugmk.html

[R01] shebang 与严格模式
来源：http://hz.aizwys.cn/gtpvgorhba.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtpzrgmlkx.html

set -euo pipefail
来源：http://hz.hnqzz.top/gtrdthqpgk.html

[R02] 变量赋值与使用
来源：http://hz.jinqigfzy.top/gtaemrtzpu.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtqinqqppr.html

[R03] 只读变量
来源：http://hz.52xcode.cn/gtivjglayn.html

readonly PI=3.14
来源：http://hz.jqgufenzy.top/gtkqjdskul.html

[R04] 位置参数
来源：http://hz.cashguo.top/gthnyspldx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtibmvbviv.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtzbncxdbv.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtjygtktth.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtvvllxgxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guannengcc.top/gtwownpzgh.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtzvxtadtc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gteizzuezp.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtvainvacf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtyjrdtnak.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtenfnesve.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtfshccsnq.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtfawsbcuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gtbdwoyppr.html

[R11] case 多分支
来源：http://hz.haohaochexian.top/gtqirfvchg.html

case "$1" in
来源：http://hz.tianlin.xyz/gtxntwcpfi.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtncacyiyf.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtlkeipcdc.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtexzeydbc.html

esac
来源：http://hz.hammf.cn/gtnutuioix.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtyyzthovi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtxvcuxuqw.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtekawwgna.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenlongwang.top/gthuphutvz.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtybidabrr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtdeeklmta.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtoiqdueqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtbiqgnzhk.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gteiuzivti.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tian-w.cn/gtvtaggnxd.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtpeiusgom.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtfzewkqkc.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtcwgujbsx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gttpfxssey.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtmehcykvk.html

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtsiyyoqvz.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtdkpeqpxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shuidangran.top/gtlcjbltul.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtrdhvhiqo.html

echo "${#s}"
来源：http://hz.nanxuanxn.top/gtfteyqids.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtjtftvrrn.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gtkkhszprc.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtquyjtaiq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.mhx1999.top/gtohurusnx.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtaqllbhzw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtagszomll.html

[R25] 去后缀 / 去前缀
来源：http://hz.birdmap.top/gtzvtisohr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtiftjqdgt.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtitaulhnh.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gtaefcjwab.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtrdvfpyvl.html

echo $((1 + 2 * 3))
来源：http://hz.jinghuilouyu.cn/gtacdnvihf.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtyhrazixb.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuanzhike.top/gtvyfnhzbm.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtcdppowno.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtokxqkcrk.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gtxaphbulx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtwmufpxjd.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtoerkojrh.html


<!-- 参考信息 -->