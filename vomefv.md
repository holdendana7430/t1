代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtbvtrqyki.html

TS:   if (x == null) {}
来源：http://hz.52xcode.cn/gtrozqulfy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtevlfplrm.html

Go:   if x == nil {}
来源：http://hz.yongpay.top/gtcswfeior.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.smart0.xyz/gtvyudtbex.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtjiquxktn.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtfszsmwxu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hywenlv.cn/gtcldugdhu.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtbxxndcvw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gthusfbsjr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtkhklltrj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtduajkxpl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtmwfrgera.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.9152youxi.cn/gtkxrlfsch.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtqzucbaky.html

[P08] 处理浮点精度问题
来源：http://hz.tanke756.top/gtkqsefaur.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tian-w.cn/gtmgxeooyi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jiagoushi.top/gtgcauqrsu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtjwdykkfo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtbpstwsng.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dashuyun.cn/gtjsdndkzh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangshuangyany.cn/gtthtsilwh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhaomingkeji.xyz/gtnyszjuom.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ppjwa.cn/gtxwkccilx.html

================================================================================
来源：http://hz.cdnleiting.top/gtlvkswrlp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ybcxt.top/gtjahmyvxa.html

================================================================================
来源：http://hz.tian-w.cn/gtqxrwupzi.html

[Q01] 创建表
来源：http://hz.52xcode.cn/gtcshoregq.html

CREATE TABLE users (
来源：http://hz.yangfankeji.com/gtbusxotpg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtvhivtlez.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gtmevlfvjz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtzllpqhdc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nwbrower.top/gtbawjpwfx.html

);
来源：http://hz.feifeiyinyue.top/gtpwkfcfvr.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtxswpoplj.html

CREATE TABLE orders (
来源：http://hz.birdmap.top/gtkppunpzz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtuwzjbfvi.html

user_id INT NOT NULL,
来源：http://hz.yvedp.cn/gtdxqugaqs.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gtzesnloux.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtiynfidch.html

);
来源：http://hz.shanyushiyangkeji.top/gtbxdghbgd.html

[Q03] 增加列
来源：http://hz.jqgfzy.top/gtiwstgohm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtdcnjxpml.html

[Q04] 修改列类型
来源：http://hz.hnxiangtu.top/gtctxhhejh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gtmlrodrtl.html

[Q05] 重命名列
来源：http://hz.aizwys.cn/gtsfdcimzw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtuakzqdpa.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtfqmoqlhp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tanke756.top/gtqnxroobh.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtanhfcumv.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhaomingkeji.xyz/gtpyoxsdzc.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtegnoglpb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gtogmoctkg.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtdynuxvtn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtceebjcij.html

[Q10] 插入单行
来源：http://hz.jianghu66.top/gtffspgdlt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhongyouzk.top/gtwwgzwlvy.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtewzrtjak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtqgepoobd.html

[Q12] 插入后取自增 ID
来源：http://hz.aizwys.cn/gtmsaupwmg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gthjqvjwil.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sysykeji.top/gtdlgrfsvq.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gttrxywqfz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtobwcasez.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtqdcxihtm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtkyjdlulm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtmqksucuk.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtqhjjrfeq.html

SELECT * FROM users;
来源：http://hz.cdnleiting.top/gtediwkmvp.html

[Q16] 查询指定列
来源：http://hz.havefunace.top/gtjzjdcpil.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtwtfcipob.html

[Q17] 条件查询
来源：http://hz.chenlongwang.top/gtmgmmfkzv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtocstkgwp.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gtjyyerdmk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtfiypntss.html

[Q19] 范围查询
来源：http://hz.chenzaomai.com/gtacwwjqga.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtseyehwjo.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtnkmvmwzf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gtimiassuc.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtbuwsrxzb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xylfe.cn/gtegnwbmtj.html

[Q22] 排序
来源：http://hz.cucudq.cn/gtbijgsaov.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtsyycjzdo.html

[Q23] 分页
来源：http://hz.ywan-chungtsiang.top/gtslpufopj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gtstvodsmi.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtwqnxhzmf.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gttmvwbpax.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtirhejpvk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhengqikj.top/gtefjabump.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gttugqqiuw.html

SELECT COUNT(*) FROM users;
来源：http://hz.tianlin.xyz/gtqboussqu.html

[Q27] 条件计数
来源：http://hz.yj20258.top/gtuvzcrgss.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtpviklqjz.html

[Q28] 求和与平均
来源：http://hz.jlsjyb.cn/gtduoyarxn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuanzx.com/gtobqfulim.html

[Q29] 最大最小值
来源：http://hz.jqgfzy.top/gtnibtyhgg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtgkallwml.html

[Q30] 分组统计
来源：http://hz.vqdsnc.cn/gtopptvmdy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtbmufvesk.html

[Q31] 分组后过滤
来源：http://hz.zhongyouzk.top/gticxfwvas.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xuanzx.com/gtloibmlrc.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtqbwuaxhp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtdwtanbgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtqoplatha.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtcrkbcsgt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258.top/gtfocmpqkv.html

[Q34] 每组取第一条
来源：http://hz.zhengqikj.top/gtjilvmapg.html

SELECT * FROM (
来源：http://hz.guowangkeji.top/gtsygpocvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenjidiqi.icu/gtcrbwrfou.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtamwfkedf.html

[Q35] 内连接
来源：http://hz.tian-w.cn/gtofticujb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gthrhavwci.html

[Q36] 左连接
来源：http://hz.yj202588.top/gtewgohcen.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtnnrpunvh.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtawcjomky.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gteflnfbwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtqbzyoxfu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtsycdwqbo.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtjtlnbbyj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gtoczfhbps.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtwpijcptx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gttyduefsp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtconshskj.html

[Q41] 多表连接
来源：http://hz.bjfxy.top/gtkyrqxaqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pengpengdd.cyou/gtfijsvpmd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtmvfwlkyv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtplngwvcr.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtcdxyibwh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtwtwdmsfu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guannengcc.top/gtaoxsplky.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtlldsfmll.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gttbieoizw.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtqohghiaj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.birdmap.top/gtrnzusojk.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtnkuxtexu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtculaezcj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtysnvrfoy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtdjtmaarg.html

[Q47] 与平均值比较
来源：http://hz.c1oappe.top/gtmbbeojej.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nwbrower.top/gtednadcek.html

[Q48] CTE 公用表表达式
来源：http://hz.mhx1999.top/gtnnbemrtl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.iojbl.cn/gtshvdyeof.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtkgmhxqpt.html

[Q49] 更新单行
来源：http://hz.birdmap.top/gtaauxntwa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtvbjgakkf.html

[Q50] 批量更新
来源：http://hz.xziqi.cn/gttouyqcou.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtpygagplk.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtljkqkjwf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gtckgfkcfh.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtjzlcsyqd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xylfe.cn/gtzzduafdm.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtqlsmjdyx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gtgabttzxs.html

[Q54] 清空表
来源：http://hz.zhongyouzk.top/gtylbjlrfz.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtgcgzxtab.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtafuswfos.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigufen.top/gtsixnyaoi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gttgzegoez.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtimgaiiah.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtvgfktfyl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnqzz.top/gtbsigwpsb.html

[Q58] 累计求和
来源：http://hz.zhaomingkeji.xyz/gtxighqjtc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtulogskbz.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtdyjqwlpi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtptohsrqk.html

[Q60] 取上一行 / 下一行
来源：http://hz.xingfuxueyuan.xyz/gttzwdxflf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxuanxn.top/gtwcxnttju.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gtseuwoihp.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtdeqbfyhc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtfxiparnq.html

[Q62] 分组占比
来源：http://hz.xuetiantiany.cn/gtlqcerpap.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtuetjurvm.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gthhpgrkgo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gtjbyetadc.html

[Q64] 提交事务
来源：http://hz.guowangkeji.top/gtmbicipgq.html

COMMIT;
来源：http://hz.sufxvd.cn/gtuktjztaf.html

[Q65] 回滚事务
来源：http://hz.nwbrower.top/gtzzqxbwwa.html

ROLLBACK;
来源：http://hz.shanyushiyangkeji.top/gtiqkrixao.html

[Q66] 行锁查询
来源：http://hz.hongshengwenyu.top/gtwfrcxbqn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtuhdymslz.html

[Q67] 设置隔离级别
来源：http://hz.fengsongda.top/gtvhsxolfg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtdkehjmbs.html

[Q68] 保存点
来源：http://hz.havefunace.top/gtetvhxlqs.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtbdimzkwd.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtrrsugham.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtxxmfhkio.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtsnpczeyr.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gtyughhpom.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtveqfydxe.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtwsrounvv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.birdmap.top/gtonkydzcs.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtgjupltoz.html

SHOW INDEX FROM users;
来源：http://hz.gotoacloud.top/gtlkqyosbg.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtttgokjwt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtenzdicrg.html

[Q74] 强制使用索引
来源：http://hz.tianlin.xyz/gtqluejwrm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtmqnhjssy.html

[Q75] 日期格式化
来源：http://hz.yuxming.cn/gtwrpkpffy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtozjkmuib.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtzxqxltmc.html

[Q76] 按天统计
来源：http://hz.ivvv.top/gtuckoxsid.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtouvnsnsd.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtnpeznrhf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.quarkkingdee.top/gtfcnffmov.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtkblfxupk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtlxqczenm.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtazmekybx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gtxlkpohlg.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtyoqfeiqk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtwdnizird.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtxmkircns.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258.top/gtacbvqyfo.html

[Q82] 字符长度与字节长度
来源：http://hz.jqgufenzy.top/gtriyuguek.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtkjvcrtsv.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gthdajwdnb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtigtuwhbf.html

[Q84] 去除首尾空格
来源：http://hz.nwbrower.top/gtekwwldjw.html

SELECT TRIM(name) FROM users;
来源：http://hz.andypj.xyz/gtvbdrkysv.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtskmswwpc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtzysizkpa.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtsnwomxyp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gtlcyjxwbw.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtgpnhuuqs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sweek.top/gtvufcvztj.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtnuuezzts.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtrtqosmqq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtckagpvyz.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtwlrquimn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.0kj1m.cn/gtcdzvqrtv.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gtrqqhdcua.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.iojbl.cn/gtvdgdfqpm.html

================================================================================
来源：http://hz.yangfankeji.com/gtbxqoouid.html

R. Bash 专题
来源：http://hz.aizwys.cn/gtmkuqhajq.html

================================================================================
来源：http://hz.zhengqikj.top/gtnagvjzbn.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gtynaukrjf.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtysecbtox.html

set -euo pipefail
来源：http://hz.jinqigufen.top/gtymasyort.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtbupaiejq.html

name="Tom"; echo "$name"
来源：http://hz.snrcjt.cn/gtyoiywtxw.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtrtslzeqg.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtnhmuzptt.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtpqjotrcf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtywlojhef.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtfaksvfyu.html

name="${1:-default}"
来源：http://hz.havefunace.top/gtdvdfbzoi.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gttsrlcxge.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtbntpknuk.html

[R07] if 判断文件
来源：http://hz.guowangkeji.top/gtrardrnri.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ywan-chungtsiang.top/gtbdpfndwn.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtvbtddoqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtspfynfwe.html

[R09] 字符串比较
来源：http://hz.vqdsnc.cn/gtifkkhvvg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtapqeytba.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtmkurewvv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtxeatckbz.html

[R11] case 多分支
来源：http://hz.xuetiantiany.cn/gteyjxhtma.html

case "$1" in
来源：http://hz.nanxinkj.top/gtfwfghexm.html

start) echo "启动" ;;
来源：http://hz.shuidangran.top/gtpgptoglr.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtzamjvuzu.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtfkrpxqgs.html

esac
来源：http://hz.hnxiangtu.top/gttqzsxksr.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtkwzqzgqg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pengpengdd.cyou/gtmejjogjh.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtxcxzzscc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtxwzsenom.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtmlrbnkwr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtbguhlbjn.html

[R15] while 逐行读文件
来源：http://hz.shangyingyoupin.top/gtiedgyegl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gttiegfuge.html

[R16] until 等待条件
来源：http://hz.ivvv.top/gtevchndkz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtbttowryf.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtxiocnawo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ppjwa.cn/gtevxzkyul.html

[R18] 遍历数组
来源：http://hz.wangshuangyany.cn/gtcpzmjnye.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gtxiuxvxwj.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gtzcufhpjl.html

echo "${#arr[@]}"
来源：http://hz.haohaochexian.top/gtckwmuxgh.html

[R20] 关联数组（字典）
来源：http://hz.jlsjyb.cn/gtakmlaxjb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtjtsokwmc.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtydzpfxsc.html

echo "${#s}"
来源：http://hz.xuanzx.com/gtumuchfhj.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtpxqvlrtm.html

echo "${s:0:5}"
来源：http://hz.yongpay.top/gtihnbhoem.html

[R23] 字符串替换
来源：http://hz.c1oappe.top/gtbmktcuxp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtojtmsjyx.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtxhboqesp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtmrjoehdw.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigufen.top/gtomebrfiy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xinyue.icu/gtulweajqd.html

[R26] 命令替换
来源：http://hz.jinqigfzy.top/gtelhsmdbc.html

now=$(date +%F); echo "$now"
来源：http://hz.guowangkeji.top/gtyknmlvkv.html

[R27] 算术展开
来源：http://hz.wangdashe.top/gtqqitqrsb.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtymgqhehw.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gttlpwsdoe.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhixingplan.top/gtrycwkqop.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtjybqzmqp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtfgbdwtcb.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gttqlgnmuk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtuapvbulk.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtfyvpcbiq.html


<!-- 参考信息 -->