代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gtpnaczdzc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtebyjkutv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xinyue.icu/gtxhhqopux.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtbihvmdha.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cheryme.top/gtqryqiqpl.html

TS:   if (x == null) {}
来源：http://hz.yueranfly.top/gtlwylmqzg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jianghu66.top/gtstxajkyf.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gttwtwxgzg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.52xcode.cn/gtsmlkwzfb.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gtiqcolqsj.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gthikjkcfd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cucudq.cn/gtkyqmutey.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtuctykckx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtqsflbtfv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtfifikkwq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtwknevpbn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gttkpnussg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhaomingkeji.xyz/gtvethsglt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhoulong.xyz/gtahnscopr.html

[P08] 处理浮点精度问题
来源：http://hz.ehwqpu.com/gtpxbcnwyn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenzaomai.com/gtalyobrkb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shzxlz.cn/gtvggizjxu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtgccubfjh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aibaodan.cn/gtnowgolgx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtwbmidcii.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ppjwa.cn/gtkpsddqti.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aizwys.cn/gtvbaxcsce.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhijiandao.cn/gtwfntqnki.html

================================================================================
来源：http://hz.hywenlv.cn/gtwrzhckek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtlglxrvsh.html

================================================================================
来源：http://hz.yangfankeji.com/gtifuncami.html

[Q01] 创建表
来源：http://hz.andypj.xyz/gtfiteghgn.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtzwcpiimm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtyuylmqyp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sysykeji.top/gttrqrsspp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtivrwsjzl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtqiwjfarj.html

);
来源：http://hz.yj20258888.top/gteuiyrwtr.html

[Q02] 创建带外键的表
来源：http://hz.sxryk.cn/gtgxmhwhvu.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtgxeemgxl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtptqdzwto.html

user_id INT NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtbkewawjf.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gttnungpsq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hammf.cn/gtxfcchzuq.html

);
来源：http://hz.ppjwa.cn/gtoyjrdblw.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtvpjfcxpi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtquqqemzk.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtzrckpcdc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gtvgahokjs.html

[Q05] 重命名列
来源：http://hz.yj202588.top/gtfyfqazin.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtqrroidxf.html

[Q06] 删除列
来源：http://hz.jinghuilouyu.cn/gtuhhgfaen.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.andypj.xyz/gtrpckbytu.html

[Q07] 删除表
来源：http://hz.yuanzhike.top/gtreasopzk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hammf.cn/gtnsvgnmeg.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gttckydjyn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtxdzgyaqf.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtwwzmzpgh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.havefunace.top/gtwenovhhm.html

[Q10] 插入单行
来源：http://hz.ydzc1.top/gtkbjsfhdx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtsxfghhcp.html

[Q11] 一次插入多行
来源：http://hz.andypj.xyz/gtbpiykjnz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ivvv.top/gtmmzolryd.html

[Q12] 插入后取自增 ID
来源：http://hz.iojbl.cn/gtsfjmicpq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnqzz.top/gtnvzhrdiu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sysykeji.top/gtstegjdka.html

[Q13] 忽略重复插入
来源：http://hz.cucudq.cn/gtamdzqrvp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pengpengdd.cyou/gtcyivzcjo.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gthjrdwyja.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gtblellsag.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtvtklniel.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtiqwgtyat.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtgzgmxkzn.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtawkhmkrx.html

SELECT id, name FROM users;
来源：http://hz.jqgfzy.top/gthsxwgeup.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtitzjzfqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnxiangtu.top/gtqlaiutpo.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gtvdpfweek.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtuhewwuvo.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtohargxbg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxinkj.top/gttylejnpn.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtnxzabwxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cheryme.top/gtvixhhmjt.html

[Q21] 空值判断
来源：http://hz.smart0.xyz/gtnnrymhxb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtusbejijt.html

[Q22] 排序
来源：http://hz.jianghu66.top/gtboocexzu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtbsywqblk.html

[Q23] 分页
来源：http://hz.shanyushiyangtech.top/gtwamrzpix.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.bjfxy.top/gtfzsitxpk.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtxsgucazr.html

SELECT DISTINCT city FROM users;
来源：http://hz.tianlin.xyz/gtksazzwxn.html

[Q25] 只取前 N 条
来源：http://hz.xingfuxueyuan.xyz/gtkiayxmzg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtxmgnaqig.html

[Q26] 计数
来源：http://hz.ppjwa.cn/gtvckkrslu.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtzkythqoi.html

[Q27] 条件计数
来源：http://hz.hnxiangtu.top/gtlfndpbfh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtogbyojff.html

[Q28] 求和与平均
来源：http://hz.smart0.xyz/gtkbbzvibe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.9152youxi.cn/gtqqrdxtkc.html

[Q29] 最大最小值
来源：http://hz.cqqwz.cn/gttrllgogg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtjjrvrgea.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtxbpduexx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtzddspclo.html

[Q31] 分组后过滤
来源：http://hz.nwbrower.top/gtslrvknig.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtibszfqqh.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtoibfxwpv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtyrgymobk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gttxqculrw.html

[Q33] 多列分组
来源：http://hz.svipenyu.cn/gtlxfccnjm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gthzzebtzi.html

[Q34] 每组取第一条
来源：http://hz.zhoulong.xyz/gtmgytcmee.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gthseuvvda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhongyouzk.top/gteabonlbv.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtormrzczl.html

[Q35] 内连接
来源：http://hz.shanyushiyangtech.top/gtoncetoow.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtymyomluo.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gtarreaelf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtualauuxw.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gthlnmrsrc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtckrmdtwv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtoqqugvhv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xziqi.cn/gtmuwcccyh.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gtvktztgmk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yuanzhike.top/gtgpvwugzm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shanyushiyangtech.top/gthciowbbb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gtkjvzmxal.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtrxawydqm.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtnpmdvdqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtsyopitcm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gttqnbetyu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtshneqlzl.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtsndpmppk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtwvqlqacb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenlongwang.top/gtswdaorwy.html

[Q43] 标量子查询
来源：http://hz.redwolf501.top/gtxsfwbqrx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fzhhl.top/gtjovmebxl.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtqhxeifuc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ehwqpu.com/gtyrcqjtwv.html

[Q45] EXISTS 判断存在
来源：http://hz.jlsjyb.cn/gtdfilqjas.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtslfsemcg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtpvzrjsiw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gteftaughw.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gtlgqmmbas.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.pengpengdd.cyou/gtinkpgmfk.html

[Q48] CTE 公用表表达式
来源：http://hz.gotoacloud.top/gtdhoztlxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gtqqrrunda.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cashguo.top/gtqqyangvy.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtrfmavfbu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtphpysvpr.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gthspwidab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtbxobebah.html

[Q51] 用子查询更新
来源：http://hz.yanxiufei.cn/gtunlgpvuz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtigpbcwsg.html

[Q52] 删除指定行
来源：http://hz.yonumen.top/gtxmvxvfzx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtsumjnjrw.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtsxgswmru.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gteysaywio.html

[Q54] 清空表
来源：http://hz.nwbrower.top/gtjryfintl.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtwgbgadbu.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtwirvmizd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gtkpxdrnev.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtchkngfcq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtpjkujnsx.html

[Q57] 行号
来源：http://hz.sufxvd.cn/gtscraigpw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvpuxepsr.html

[Q58] 累计求和
来源：http://hz.316326.xyz/gtdeizsjdf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigufen.top/gtacaadzao.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtfwcqbqbs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigufen.top/gtfnnoykzx.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gtqbjlutkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtukrsnuql.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtukrwaxnk.html

[Q61] 移动平均
来源：http://hz.zhijiandao.cn/gtpawsejdy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gtlazugybs.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gtxwoliyrj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtgaxxernj.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtadhyrjmq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtstrvoten.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtrojynuwo.html

COMMIT;
来源：http://hz.mhx1999.top/gtvnpyjfvt.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtroviqbzd.html

ROLLBACK;
来源：http://hz.hywenlv.cn/gtfjdeynta.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtotwkoius.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gthisvdpnd.html

[Q67] 设置隔离级别
来源：http://hz.sysykeji.top/gtqnbqyjxj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtmhrsuxfs.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtbmiuccfp.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtoibthteq.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtzzfnkrlz.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gthndzcsie.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gtbxwzcnpv.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gtfusayoqh.html

ANALYZE TABLE users;
来源：http://hz.hammf.cn/gtpyhvpgrp.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtblfbiirw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtwvhsvcmq.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtlpjaxipk.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtxorerltv.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtomyljmbn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtygwhbgvf.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtcjrivrlm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtysgavlzb.html

[Q75] 日期格式化
来源：http://hz.0kj1m.cn/gtrptcnlbf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtbdqhojor.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangdashe.top/gtinzjrlrv.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtnbxikyez.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gtlahwcudn.html

[Q77] 时间加减
来源：http://hz.andypj.xyz/gtoanvwooy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangdashe.top/gtccjwrfcn.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtbcqbefwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gthaddnwtn.html

[Q79] 字符串拼接
来源：http://hz.gogol.net.cn/gtrygauicr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtaxmcjlgk.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gticxljksh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhijiandao.cn/gtevuaclwp.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtaenzkpoa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtbzlzdtof.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gttzdbbqob.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtlxfpbxbs.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtvvrcdjte.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtjtyuzulq.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gtfrvcoczg.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtrvvezzkc.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gttxcmxzoy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtvffadfaq.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gtebryxnoc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtvuzmupzd.html

[Q87] JSON 字段做条件
来源：http://hz.hnqzz.top/gtsfmuzlly.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gthbverdhj.html

[Q88] 行转列（条件聚合）
来源：http://hz.dianchejie.cn/gtccztxxby.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gtsgyksxng.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.kuanghao11.cn/gtmstzjqto.html

[Q89] 判断表是否存在
来源：http://hz.yj20258888.top/gthdyzttnx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtgsdkjtnb.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gtwwrvbntg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinghuilouyu.cn/gtgrljntzc.html

================================================================================
来源：http://hz.yueranfly.top/gtefkzuial.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtqwqrguwl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvjnqtrxk.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtpclkpovn.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtqzlkdmcr.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtpipeftnf.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtnirifdbu.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtamiwqqbe.html

[R03] 只读变量
来源：http://hz.shanyushiyangkeji.top/gtjfqeupig.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtrqdwyivr.html

[R04] 位置参数
来源：http://hz.wangshuangyany.cn/gtoymwftqr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cheryme.top/gtoqgltyla.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtjrzqjcnr.html

name="${1:-default}"
来源：http://hz.haohaochexian.top/gtlscmqibx.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtdwdrccpa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtjyeoheuk.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtegusmwue.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtzsrgzono.html

[R08] 数值比较
来源：http://hz.ehwqpu.com/gtllvgrwqu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtwovpwskr.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtdlbojyux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gteegmntdd.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtgojtbpvi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gthppacmbh.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtojzvwtqa.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtuxewygia.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gttjpwmcoj.html

stop)  echo "停止" ;;
来源：http://hz.nanxuanxn.top/gtfbyzxems.html

*)     echo "未知命令" ;;
来源：http://hz.hammf.cn/gttcuaxqev.html

esac
来源：http://hz.yongpay.top/gtwjlfrmka.html

[R12] for 遍历文件
来源：http://hz.mhx1999.top/gttypsqtbq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtnyctuqeu.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtpwvlmiec.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gtbubryywy.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtgjdqurbu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtkebtjrfv.html

[R15] while 逐行读文件
来源：http://hz.9152youxi.cn/gtfxmkxrhf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtuwwqaqld.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gtpkvltdqh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gteylavcqo.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtqgperujt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtyuehwjnb.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtfpswjwqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258888.top/gtqkpopvpo.html

[R19] 数组长度
来源：http://hz.daria6918.cn/gtltlcvuem.html

echo "${#arr[@]}"
来源：http://hz.wangshuangyany.cn/gtgqcoxvyx.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtuurppueg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gtgmdlqmyz.html

[R21] 字符串长度
来源：http://hz.tianlin.xyz/gtxieqndrf.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtxsucztnv.html

[R22] 截取子串
来源：http://hz.316326.xyz/gtcmglpaiz.html

echo "${s:0:5}"
来源：http://hz.wangdashe.top/gtrwqcitrg.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtlybafbui.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxuanxn.top/gtlzjnzadx.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtyaexirtx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtdxccnlba.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenzaomai.com/gtoyiiywno.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangtech.top/gtjlslgerf.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtkndgxmwb.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtfriqycet.html

[R27] 算术展开
来源：http://hz.andypj.xyz/gtndwonwnd.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtzpdgkzyu.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtkpzcytrz.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtdieygwag.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtagzuwjay.html


<!-- 参考信息 -->