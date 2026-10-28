代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtjauttcbq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yonumen.top/gtulkpiwbu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhongyouzk.top/gtcufdrpyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtyqrydyea.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtavzzhcex.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.0kj1m.cn/gthtcxdzvi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtbojqrbxv.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtyfptqudi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj20258.top/gtsxnylbah.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.haohaochexian.top/gtqpovjjdt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtbqgzvszq.html

PHP:  if (empty($x)) {}
来源：http://hz.yangfankeji.com/gtoirzqqto.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgufenzy.top/gtquonxulu.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtvocsbecl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nwbrower.top/gtudamlyuv.html

Go:   if x == nil {}
来源：http://hz.jinqigufen.top/gtipjfysci.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtziylaifh.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtjbpdqxse.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtsprwzfap.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtzxsftxmq.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gttydozein.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtpwtuyotq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtfdtkdcmm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtmmtnxhcd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gttmulrzmq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.9152youxi.cn/gtqpbstkyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnqzz.top/gtfvqmmjla.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gtabqhzfuk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jqgfzy.top/gtzditfzxb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtldbniflp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtcrzmyskd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtxulxumoc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shuidangran.top/gtjfmpryfl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gttvolegqx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenlongwang.top/gtqdphcbqu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtgonjbdfb.html

================================================================================
来源：http://hz.sysykeji.top/gtzgkohudi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtucrhdaob.html

================================================================================
来源：http://hz.jianghu66.top/gtuilqerur.html

[Q01] 创建表
来源：http://hz.zhaomingkeji.xyz/gtthoevklj.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtbcfxowls.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtkrriemdw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtvtxvvmvc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtlytjseqm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtnckeplhr.html

);
来源：http://hz.ydzc1.top/gtptayfhfx.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gtjvzyydkg.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gtqmajaieu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.feifeiyinyue.top/gttsgmyucz.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtidtyhswt.html

amount DECIMAL(10, 2),
来源：http://hz.yonumen.top/gtwoeyoslz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnqzz.top/gtiallwdxs.html

);
来源：http://hz.yanxiufei.cn/gteqlgkkgf.html

[Q03] 增加列
来源：http://hz.dashuyun.cn/gtspjrxueu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daxiang520.top/gtisjfzpbb.html

[Q04] 修改列类型
来源：http://hz.ppjwa.cn/gtwgzmoxed.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gtdwmtappa.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtnqhdqwig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gttarxfrvl.html

[Q06] 删除列
来源：http://hz.xinyue.icu/gtciqairxf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtfdwhyooe.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtptdnhqrl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yanxiufei.cn/gtdlmjelsy.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtbxmdziue.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnqzz.top/gtrjkteopg.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtsbeammii.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtgfcadbxs.html

[Q10] 插入单行
来源：http://hz.zhixingplan.top/gtxewjbzbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jiagoushi.top/gtbogmhmih.html

[Q11] 一次插入多行
来源：http://hz.guowangkeji.top/gtmzmfrtmt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtakihyjva.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtwirzmkfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtfqysdxey.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shuidangran.top/gtaxdqpmsb.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtynfrphfc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtlgkxbewn.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgfzy.top/gtlqnmczcb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xinyue.icu/gtwanrlati.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gthwvmzopv.html

[Q15] 查询全部
来源：http://hz.jinghuilouyu.cn/gtsyoknlro.html

SELECT * FROM users;
来源：http://hz.ehwqpu.com/gtpiyfyzqr.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtdhkpwyzg.html

SELECT id, name FROM users;
来源：http://hz.nanxuanxn.top/gtlqazsoob.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtrfgiaimj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cheryme.top/gtpgbdwtxt.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtwdtwwnwz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtnvpwuynh.html

[Q19] 范围查询
来源：http://hz.mhx1999.top/gtglarmnth.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtiksnlwvh.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtsqrcvshm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtndyqysgf.html

[Q21] 空值判断
来源：http://hz.ydzc1.top/gtfbethmuf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.52xcode.cn/gtvhmjslmd.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gtzdanitjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtatmpuujx.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gthgpavadh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.fzhhl.top/gtpqenjiwy.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gttcglsazo.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtqzymtbic.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangkeji.top/gtlcntjwbn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gteliazzti.html

[Q26] 计数
来源：http://hz.yangfankeji.com/gtmlaiqmcv.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtqglremtd.html

[Q27] 条件计数
来源：http://hz.andypj.xyz/gtpqpzttqz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtgnexowzp.html

[Q28] 求和与平均
来源：http://hz.meibo888.top/gtccyewnlh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxinkj.top/gtciuhbfgb.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtkqswbzxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jiagoushi.top/gtspbshmtk.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtvrnnbfjp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtidicebld.html

[Q31] 分组后过滤
来源：http://hz.52xcode.cn/gtitfxwujh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gteqghjadw.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gteeqvlipo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtuunjuiol.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gtabevncnb.html

[Q33] 多列分组
来源：http://hz.haohaochexian.top/gtlevcjdas.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gtqyepciqy.html

[Q34] 每组取第一条
来源：http://hz.haohaochexian.top/gtraaorhcn.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtkmcnvelb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gtjiqpnxrd.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtgviwevfi.html

[Q35] 内连接
来源：http://hz.gzhubu.top/gtfatyocuv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtalpuzxmc.html

[Q36] 左连接
来源：http://hz.mhx1999.top/gtenrcqlal.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtzjbtcfjf.html

[Q37] 右连接
来源：http://hz.fzhhl.top/gtbgmcimee.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtvdirbjyt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.meibo888.top/gtnrgxfndp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gtcghciemd.html

[Q39] 自连接（查上下级）
来源：http://hz.ppjwa.cn/gtvohqgnku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gtyranabfd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtgudcbpdu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtyagpqhpu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtrcezualz.html

[Q41] 多表连接
来源：http://hz.yanxiufei.cn/gtridpdznc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guowangkeji.top/gtwpbjkkds.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gtyzesizsy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cqqwz.cn/gtalidjxbw.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtddwwiugj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtknxiuxwr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xinyue.icu/gtgorxwhtk.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtiwmwwckp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.52xcode.cn/gtvettovyp.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gticsgtyoi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtfirwheqd.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtglcocyoq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtrbrmthqo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.andypj.xyz/gtqxoltjpr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtxldouwuj.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtjgcvclcs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtyvdodnbt.html

[Q48] CTE 公用表表达式
来源：http://hz.yuanzhike.top/gtldkrxchd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtgpitdqpl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtyuqlcimq.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtvbmkjpul.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtfxlcmhch.html

[Q50] 批量更新
来源：http://hz.ppjwa.cn/gttujwhjvn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtqizpwque.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtnbkctmov.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gthcbegjdy.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtlmfvwqky.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtpkqmsvic.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtwenpjenn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuanzx.com/gtqzpjfurb.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtqqmsgvfk.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtmlxphbay.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtmmwynrfb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtdhbzcusk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gthvcqbzam.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gtoqjhdkyn.html

[Q57] 行号
来源：http://hz.cqqwz.cn/gthfwvpxnk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtkmqshtpi.html

[Q58] 累计求和
来源：http://hz.svipenyu.cn/gtprabspcy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtmdetqhay.html

[Q59] 分组内累计
来源：http://hz.ydzc1.top/gtconwmwvs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtypezmryu.html

[Q60] 取上一行 / 下一行
来源：http://hz.tian-w.cn/gttqzopdgj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cheryme.top/gtzosecfpm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtftuhmeel.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtfdsidxzo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtzbtmmuyv.html

[Q62] 分组占比
来源：http://hz.hfpthk.cn/gttpzbtxbx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtbqoltwfq.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtvckdmwgh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtsvarfzby.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtkqhnefny.html

COMMIT;
来源：http://hz.tian-w.cn/gtspauieaj.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtmxxgqoql.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtwcmggebj.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtoyqosppu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.kuanghao11.cn/gtjabmrxeo.html

[Q67] 设置隔离级别
来源：http://hz.smart0.xyz/gtvhlfrzaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtznfcykts.html

[Q68] 保存点
来源：http://hz.jyoumei.cn/gtxjyefdgj.html

SAVEPOINT sp1;
来源：http://hz.jyoumei.cn/gtntmcwrej.html

ROLLBACK TO sp1;
来源：http://hz.daria6918.cn/gtkdffgine.html

[Q69] 查看执行计划
来源：http://hz.zhixingplan.top/gtgfrghkor.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtanjsselr.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtbxlnoxfk.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtucpsmruq.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtcywgmfjg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gtmafbjyxi.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtoswwxwcq.html

SHOW INDEX FROM users;
来源：http://hz.mhx1999.top/gtdwuxdhws.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtsfzdphcc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gtaismfsvq.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtjywxyrwg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cashguo.top/gtaqmwwzyi.html

[Q75] 日期格式化
来源：http://hz.feifeiyinyue.top/gtemqwyrtk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gttcetawap.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtxhjyehhe.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtvoirlmid.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gtdbdnxxrr.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtckwssyxd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhoulong.xyz/gtifixsnsx.html

[Q78] 当前时间
来源：http://hz.shzxlz.cn/gttizjkkce.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtvmntnpax.html

[Q79] 字符串拼接
来源：http://hz.316326.xyz/gtlhwwfdzz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.bjfxy.top/gtosajeafu.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtvfvmajmb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tanke756.top/gtejjqakqt.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtoslznmhb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtpludbaoi.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtajxbxiuc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yonumen.top/gtumrnsoie.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtqaylfvwx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtafpsnwej.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtbkgcrpkb.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtgxayswhm.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtuxtoasfp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtrjepowdi.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtauytnoht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gthhabefrg.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gttncbmqzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cqqwz.cn/gtligfsdoa.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gtvnxipokf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yangfankeji.com/gtxchkzuqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtenwsysfe.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtixfxipiq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yangfankeji.com/gtxfxynrll.html

[Q90] 生成序号列
来源：http://hz.daria6918.cn/gtwstpjbiy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtdrgbvsjb.html

================================================================================
来源：http://hz.yueranfly.top/gtwuxkffyj.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gteyaqumqw.html

================================================================================
来源：http://hz.nanxuanxn.top/gthgazidwe.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtrqficyob.html

#!/usr/bin/env bash
来源：http://hz.aizwys.cn/gtipltroww.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtxkayztpg.html

[R02] 变量赋值与使用
来源：http://hz.guannengcc.top/gtplfmgrnp.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtbkuoddzd.html

[R03] 只读变量
来源：http://hz.yj202588.top/gttniaesad.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtmcpnsewl.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gteloseehr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtyswevyeo.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gtzvcxzjqi.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtaunhtaox.html

[R06] 判断命令是否存在
来源：http://hz.yuanzhike.top/gtyzvgvmak.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtovxmfsss.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtislwgwaz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtykvrcglb.html

[R08] 数值比较
来源：http://hz.52xcode.cn/gtfiracxqs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhiwuduotai.top/gtxaaxepud.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtvcyekmjw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtzzxiozam.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtoeqqpdrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtzoxnravb.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtmvwvlpqw.html

case "$1" in
来源：http://hz.andypj.xyz/gtopwnckes.html

start) echo "启动" ;;
来源：http://hz.yonumen.top/gtaibborzp.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gthwtlbvvx.html

*)     echo "未知命令" ;;
来源：http://hz.zhiwuduotai.top/gthvorymtf.html

esac
来源：http://hz.quarkkingdee.top/gtkkxllkou.html

[R12] for 遍历文件
来源：http://hz.feifeiyinyue.top/gtglkmfmhm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuetiantiany.cn/gtxwbnmhfd.html

[R13] for 计数循环
来源：http://hz.hammf.cn/gtddpikapj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtwawkqsxf.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtlznovuep.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.birdmap.top/gtizhsnibq.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtkllnrymy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtnjfhwkbp.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtbiacckeq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gthkhqedqb.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtcrvctnqz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtedocaasd.html

[R18] 遍历数组
来源：http://hz.wangdashe.top/gtyfjaqtgc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtljzchxit.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtweticnlh.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtyuglptcj.html

[R20] 关联数组（字典）
来源：http://hz.xingfuxueyuan.xyz/gtkcmeegnf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sufxvd.cn/gtvkaeyxqw.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gttyqvwxrv.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtgoybmevj.html

[R22] 截取子串
来源：http://hz.jyoumei.cn/gtngtznyqa.html

echo "${s:0:5}"
来源：http://hz.chenjidiqi.icu/gtssiaqdlb.html

[R23] 字符串替换
来源：http://hz.gogol.net.cn/gtpzbkqzlp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtqoiubkfs.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtiflvtwlv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtsylribzm.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gtctpdtpjk.html


<!-- 参考信息 -->