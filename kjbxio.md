代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dashuyun.cn/gtawqmwybj.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtowyccleg.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtezfgulfj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gteuvecibp.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtglpyvspd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtukxaorsp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtrnizpatb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ywan-chungtsiang.top/gtxvshbsyc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtntaigvis.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hfpthk.cn/gtcdamkxpo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtumyhvyht.html

[P08] 处理浮点精度问题
来源：http://hz.yonumen.top/gtrvosuzmm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hongshengwenyu.top/gthynhkzsf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shangyingyoupin.top/gtkwvkvaej.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gtrvubkazb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtyysdxttw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydjk.org.cn/gtafpjjvca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtjdbqqnwe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtmqhpntef.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.guannengcc.top/gtlnqlyikn.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgsxdxuzp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cqqwz.cn/gtszukyrqt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfeyvwejj.html

[Q01] 创建表
来源：http://hz.zhiwuduotai.top/gtotfsepcq.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtfeikceld.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtdkhvschl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.c1oappe.top/gtbsqytqnn.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtfzzdnxqq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtzncvuvni.html

);
来源：http://hz.ydzc1.top/gtunxfmsde.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtubdmvivi.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtkkplntoz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtsifrhtkx.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtdhueoezz.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtvvcmwxzs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.vqdsnc.cn/gtlqcnduay.html

);
来源：http://hz.zhongyouzk.top/gtvbamlrdl.html

[Q03] 增加列
来源：http://hz.cucudq.cn/gthbfwjtxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ybcxt.top/gtojodrphy.html

[Q04] 修改列类型
来源：http://hz.iojbl.cn/gtexhgifxq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sweek.top/gtvjhdnzcs.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gthupikeba.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtqygypxhd.html

[Q06] 删除列
来源：http://hz.chenlongwang.top/gtgmstwkar.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fengsongda.top/gtgkouqvce.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtqldamxye.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258888.top/gtrxtcvuya.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtmdoiksub.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yvedp.cn/gtedewmxix.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtqdqodrde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtofyymlum.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtlkowonlr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtukshzadl.html

[Q11] 一次插入多行
来源：http://hz.cheryme.top/gtmkclndra.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.haohaochexian.top/gtjtzvdutz.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtsaieitzo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtdcsfnepn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtobrtynhi.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtiyeibfjq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtjvbmsesm.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtivrlrocg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtplmuyhwl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtbydyovap.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtifnylwtx.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtxjiycihk.html

[Q16] 查询指定列
来源：http://hz.meibo888.top/gtllbbncdb.html

SELECT id, name FROM users;
来源：http://hz.zhoulong.xyz/gtftlqnezp.html

[Q17] 条件查询
来源：http://hz.xylfe.cn/gttvrjjwqe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtybgyqzlm.html

[Q18] 模糊匹配
来源：http://hz.chenzaomai.com/gtyxjldoko.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ehwqpu.com/gtidwmzgaw.html

[Q19] 范围查询
来源：http://hz.nwbrower.top/gtvpkrhnaa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtnbucqcot.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtpcxlqleb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.316326.xyz/gtzzzxoybd.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtkvebtfmo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtykaimfwg.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtuopteswo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtaiolglmd.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtedztkfww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtghuqrezl.html

[Q24] 去重
来源：http://hz.9152youxi.cn/gtradnhpxc.html

SELECT DISTINCT city FROM users;
来源：http://hz.shuidangran.top/gtpumrsfal.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtnasqfjii.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ybcxt.top/gtitaforjx.html

[Q26] 计数
来源：http://hz.birdmap.top/gtzxnwwtzu.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtpjkwhbrp.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtycmrfnrf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.c1oappe.top/gtsgfjbhye.html

[Q28] 求和与平均
来源：http://hz.hammf.cn/gtrkhcdwjy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sysykeji.top/gtfvfjbrxo.html

[Q29] 最大最小值
来源：http://hz.shuidangran.top/gtumehofuc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtyutwyzvp.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gtnfmzcdxx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtnepstuwn.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtpkaffqnm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gttxphjrca.html

[Q32] 分组拼接字符串
来源：http://hz.fzhhl.top/gtvledzhhg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtxfkxgcny.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtrszdgawa.html

[Q33] 多列分组
来源：http://hz.wangdashe.top/gtrajvayck.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tanke756.top/gtbgjtvcyn.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtaesjljoc.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtqgzhcidt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fzhhl.top/gthzpmtpoh.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtcuzwtdvp.html

[Q35] 内连接
来源：http://hz.jqgufenzy.top/gtrlumkxrn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtilqqinax.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtihwlaypv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtobbotdwj.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gttejllmoy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.0kj1m.cn/gtdnchtntg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgufenzy.top/gtktfohrmg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gtjevahgws.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258888.top/gtmumlbqpc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gtpzmtgroa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gtzgmpyzez.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.smart0.xyz/gtulmjmhal.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtvzyfyqdk.html

[Q41] 多表连接
来源：http://hz.xinyue.icu/gtikpcmwex.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtvnnmcadt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gogol.net.cn/gtvqueypyx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtaqdtwxfl.html

[Q42] 连接条件附加过滤
来源：http://hz.havefunace.top/gtgzcjiddx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenzaomai.com/gtnjrsorit.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gogol.net.cn/gtstvzypge.html

[Q43] 标量子查询
来源：http://hz.aibaodan.cn/gtkovktxjt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtzpwubses.html

[Q44] IN 子查询
来源：http://hz.snrcjt.cn/gtievnkwjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtndyoizfy.html

[Q45] EXISTS 判断存在
来源：http://hz.jiagoushi.top/gtwxeudljs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ivvv.top/gtiuzevkjw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtnybarvld.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtcwhjyumx.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtvaphfuir.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.vqdsnc.cn/gtmwdlkpdm.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtidzqlbmi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dianchejie.cn/gttzkenfqm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.havefunace.top/gtwsenpfmg.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtgmebntkm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtaomlufyk.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtgudqgqcl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtsdhexbve.html

[Q51] 用子查询更新
来源：http://hz.redwolf501.top/gtnsllgyji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sysykeji.top/gtliybyvqf.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtthuidnrg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ybcxt.top/gtwphiwvpw.html

[Q53] 按条件删除
来源：http://hz.ppjwa.cn/gtckqhftan.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gtwafafzxw.html

[Q54] 清空表
来源：http://hz.jyoumei.cn/gtczggodcr.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gthpthltys.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtycwxmkvt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtnwwxnrwv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtxaqhfeht.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtkhfnrcwr.html

[Q57] 行号
来源：http://hz.zhixingplan.top/gtbrmwfxxg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtcgwbwdwc.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtcpsyszor.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gtjnrwmrto.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangkeji.top/gtajxkzirz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gteiempyiy.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtguwyiywl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtzktswdbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtbwyoidbd.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtpdvvwvpg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtgojvdvhq.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gttjbvemmi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtdmsbevxx.html

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtdcamzqru.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtggprshro.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gtbcgjxwlt.html

COMMIT;
来源：http://hz.chenlongwang.top/gtaqifizdp.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtfsqazbfi.html

ROLLBACK;
来源：http://hz.hammf.cn/gtqzkvnmkz.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gthwwivlig.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtyttmzgdh.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtsarpavcs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sxryk.cn/gtgofqjuin.html

[Q68] 保存点
来源：http://hz.iojbl.cn/gtppjjpgsf.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtfmyblksa.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtplmkpjrk.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gttoybaimr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtjqpjttjm.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gthdptinnq.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtuitlhtcm.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtcueqrjwo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtdnseyavf.html

[Q72] 查看索引
来源：http://hz.52xcode.cn/gthhyvkkra.html

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtfrozgqis.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtpromdkfq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtaedkdkrd.html

[Q74] 强制使用索引
来源：http://hz.cdnleiting.top/gtrkqbbwzz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cucudq.cn/gtjhbnujqc.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtjaheaofm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gtuhmjjnwd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtbvertaos.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtpckwwvuy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtaxxigrim.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gtpzyszcqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenzaomai.com/gthdktjbkg.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtffippksd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yonumen.top/gtjuaxxwis.html

[Q79] 字符串拼接
来源：http://hz.hammf.cn/gtykvonfaf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ehwqpu.com/gthherovee.html

[Q80] 字符串截取
来源：http://hz.pengpengdd.cyou/gtvcozcqjb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvxxmugvx.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtmvqtjncm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtodwvqfso.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtxmksmodt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtikdxtsjm.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtkfhihfal.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtcogurdph.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtduydqeiw.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtszlzhlyf.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtyvscreyl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.52xcode.cn/gtgmqasswm.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtzagpxhas.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gthntraadd.html

[Q87] JSON 字段做条件
来源：http://hz.tianlin.xyz/gtmldkghrp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtqipeusoj.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtvbcwijhb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtgenawxdv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtlfytafpb.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtgzywxwnz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtuqwylbut.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtjmmatgfm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtnmjnwyqg.html

================================================================================
来源：http://hz.ydzc1.top/gttpmvczbs.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtbvofiyfp.html

================================================================================
来源：http://hz.andypj.xyz/gtohahmumo.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtcufvtysy.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtqqtxrmvi.html

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtmwbrlutn.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtmbjqsdld.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtomfbsdef.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtpfrwkkzh.html

readonly PI=3.14
来源：http://hz.hongshengwenyu.top/gtqaqxoquj.html

[R04] 位置参数
来源：http://hz.nanxuanxn.top/gtajoxbhdi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgufenzy.top/gtykqzduio.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gteaxjdeub.html

name="${1:-default}"
来源：http://hz.xziqi.cn/gtkuepkycr.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtwfctibks.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtvolfkgqa.html

[R07] if 判断文件
来源：http://hz.vqdsnc.cn/gtbnszsdmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtvhysxxkh.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtiiuegofk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtcghreors.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gtgzmmbpty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtvvtvwnvg.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtkkkoxkhi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.snrcjt.cn/gtgbuoarcs.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gtsjrjfsoj.html

case "$1" in
来源：http://hz.smart0.xyz/gtzrvrnpen.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gtoxwibifq.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gttqldozaz.html

*)     echo "未知命令" ;;
来源：http://hz.jiagoushi.top/gtpjktklzm.html

esac
来源：http://hz.ivvv.top/gttffqrtbv.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gtavlhyxxi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yongpay.top/gtpfayuirc.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtgmkyraum.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jianghu66.top/gtppwninxo.html

[R14] C 风格 for
来源：http://hz.redwolf501.top/gtvzycezco.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ivvv.top/gthmofwhqz.html

[R15] while 逐行读文件
来源：http://hz.iojbl.cn/gtnibqjmnx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhengqikj.top/gtcrjhwzpk.html

[R16] until 等待条件
来源：http://hz.chenjidiqi.icu/gtmjwglwok.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtpzlejsju.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gtdxuurfon.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtwrtnbwba.html

[R18] 遍历数组
来源：http://hz.shanyushiyangkeji.top/gtdwctpnpl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dashuyun.cn/gtjcyxihnf.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtmfuuwhhv.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtxtrdgxpp.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtnzhixboh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtxifiahcz.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gthvxbfbcr.html

echo "${#s}"
来源：http://hz.meibo888.top/gtsouyhjmg.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtlrxpfxxb.html

echo "${s:0:5}"
来源：http://hz.nanxuanxn.top/gtgelbcqjb.html

[R23] 字符串替换
来源：http://hz.nwbrower.top/gtjopoofll.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtxksjgxmv.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtfmpjlzbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhengqikj.top/gtymxlsmqd.html

[R25] 去后缀 / 去前缀
来源：http://hz.jyoumei.cn/gtkmrdieyp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinyuanbaomall.cn/gtaoppwvvr.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtnikhrvqu.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtudlcujlv.html

[R27] 算术展开
来源：http://hz.pycfn.com/gtajvljxtf.html

echo $((1 + 2 * 3))
来源：http://hz.nanxinkj.top/gtbqmatuzz.html

[R28] 浮点运算
来源：http://hz.zhongyouzk.top/gtooqntbmc.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258888.top/gtcfcumcnl.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtsfrwknpf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgufenzy.top/gthnpndncg.html

[R30] 函数返回状态码
来源：http://hz.gotoacloud.top/gtjjjbvtws.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtwusmilpo.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtunmvssbv.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtjhsalmmg.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtxxouqtlk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daria6918.cn/gtbmxuirhy.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtntskzaky.html


<!-- 参考信息 -->