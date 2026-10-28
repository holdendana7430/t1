代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtebuyqsyq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hysaishi.cn/gtcwvdzbqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhengqikj.top/gtgdvatwab.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtxbfsuyop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtwlbtnttu.html

TS:   if (x == null) {}
来源：http://hz.hnqzz.top/gtvqfwpfwi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtxxfqildw.html

Go:   if x == nil {}
来源：http://hz.jinqigufen.top/gtxijcoizw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnqzz.top/gtfskcnkld.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gteelfsweo.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtoovpufgt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cdnleiting.top/gtqujmwewa.html

PHP:  // 手写时间戳比较
来源：http://hz.tian-w.cn/gtfnwkahwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtopqncdgt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtnkvqnqbc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtvqnlzois.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnxiangtu.top/gtnxxdvrib.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtlmctqswd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gtkbbiwsmb.html

[P08] 处理浮点精度问题
来源：http://hz.tian-w.cn/gtiftdrsgd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtelxwuegp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtudwcbbou.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shzxlz.cn/gtorurqrkz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtwakcspjt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtfhuitzjz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xylfe.cn/gtoayrftxl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtbjgmahta.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtzlmcdfzj.html

================================================================================
来源：http://hz.daxiang520.top/gtkmjimway.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tanke756.top/gtgnyeleki.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdqrhjtiz.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtwdddaugk.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtjwjrdtjm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gtaqfrnyrl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtvkefvtdj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hongshengwenyu.top/gthxjwfcsr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtubnihqzm.html

);
来源：http://hz.bjfxy.top/gtivywxvok.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gthkkxbhsi.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtaytpqysk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtyinwxlgd.html

user_id INT NOT NULL,
来源：http://hz.birdmap.top/gtvemauunh.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtfhidvqmu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtdfxvzkip.html

);
来源：http://hz.xuetiantiany.cn/gtfxevbaro.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtmnyqypte.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtbzbqkdmz.html

[Q04] 修改列类型
来源：http://hz.sxryk.cn/gtidvquubr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtyqqacljj.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtcfmjpnoy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gtrusbgkoe.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtcybdrttw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuanzhike.top/gtefvhwisb.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtslietbdn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gogol.net.cn/gtpogxucrp.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtktjmpypf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtzjwigyiz.html

[Q09] 创建唯一索引
来源：http://hz.smart0.xyz/gtiyqnwapu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtcflazvhi.html

[Q10] 插入单行
来源：http://hz.zhiwuduotai.top/gtgcuppqxx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.52xcode.cn/gtvtcucoze.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtmsncrhbi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnqzz.top/gthqofyunn.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtbaodppzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.kuanghao11.cn/gtaveykqgj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtdejqvdai.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtlsgjbrhf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtzbxrlgiz.html

[Q14] 存在则更新（upsert）
来源：http://hz.aizwys.cn/gtypmircmt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258888.top/gtdvxjtvtm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtopgqtiuo.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gthqongkke.html

SELECT * FROM users;
来源：http://hz.chenjidiqi.icu/gtajbqwfcl.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtqhiwwchp.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtuvwepxri.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtrjyylbom.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shzxlz.cn/gthrgmagtf.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtqjjsyxnr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gtolhhhfoa.html

[Q19] 范围查询
来源：http://hz.ehwqpu.com/gtlejklbkf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtslzrafnn.html

[Q20] IN 列表
来源：http://hz.xuanzx.com/gtgjdhmunn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.9152youxi.cn/gtqrbyznty.html

[Q21] 空值判断
来源：http://hz.ivvv.top/gtthtokgir.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtmiqtulam.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtqliyusur.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtvwrmacsk.html

[Q23] 分页
来源：http://hz.zhixingplan.top/gthdnvvyus.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtcqlusktu.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtkzbvyuev.html

SELECT DISTINCT city FROM users;
来源：http://hz.52xcode.cn/gtdqmgntpk.html

[Q25] 只取前 N 条
来源：http://hz.ydzc1.top/gtokzridld.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtbyldjevi.html

[Q26] 计数
来源：http://hz.chenzaomai.com/gtsxhovkri.html

SELECT COUNT(*) FROM users;
来源：http://hz.redwolf501.top/gtcvggsltw.html

[Q27] 条件计数
来源：http://hz.xziqi.cn/gtscqpndsr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hongshengwenyu.top/gtegbrqqox.html

[Q28] 求和与平均
来源：http://hz.sweek.top/gtztiixjkn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cashguo.top/gtmoyrhswk.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtiujnbydb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shuidangran.top/gtsomapyld.html

[Q30] 分组统计
来源：http://hz.ehwqpu.com/gtrjpoietr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtsdrbddlp.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtsheiooxb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guannengcc.top/gtyuiaqpzj.html

[Q32] 分组拼接字符串
来源：http://hz.jyoumei.cn/gttocgwaas.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtqhlobhqf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xinyue.icu/gtomixnqlt.html

[Q33] 多列分组
来源：http://hz.jianghu66.top/gtwmtfolpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhaomingkeji.xyz/gtvtsosumc.html

[Q34] 每组取第一条
来源：http://hz.guannengcc.top/gtmuqfcvux.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gthetbplbq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shzxlz.cn/gtbkwtlnqn.html

) t WHERE rn = 1;
来源：http://hz.sxryk.cn/gtjaxkroux.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtpubrdrqq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtmqgqmtvm.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtyxincxzl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtnqssxxzc.html

[Q37] 右连接
来源：http://hz.chenjidiqi.icu/gtbtvibjxs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sysykeji.top/gtdksvxfpo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangtech.top/gtgmxfluoe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtbxqhbdxd.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigfzy.top/gtsiilehwz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zdqjudy.top/gtenxavpqb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aibaodan.cn/gtdkicqfqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtjqliqqvj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtdbcgqupp.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtmzvsdgyo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtuteessdj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gttmzodoxt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtabmidotx.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtvstldcgv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gtidlimqpj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj202588.top/gtlnieenxj.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gttyrxaycl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhaomingkeji.xyz/gtnyvmvmgz.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtgrtewepb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtjocndviv.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtbwmnoidl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtwjxmbrhe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zdqjudy.top/gtjcyontmp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtlrjkjmhw.html

[Q47] 与平均值比较
来源：http://hz.vqdsnc.cn/gtpqaifpic.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtprwewrnf.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gtsjzuxnnx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtdoaaosso.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtxccohucg.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtqgxqdoae.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydjk.org.cn/gthymrfwvo.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtvanohisp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnxiangtu.top/gtjqpifhzg.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtzowyvxbx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtwutyormu.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtykxphike.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtstglcjqs.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtsfqrjtts.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnqzz.top/gtihndhcrx.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtfehvbzwh.html

TRUNCATE TABLE logs;
来源：http://hz.yj20258.top/gtgvzptslc.html

[Q55] 排名（并列占位）
来源：http://hz.316326.xyz/gtieuqwaol.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtreabklox.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtejplcjcx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuetiantiany.cn/gtxofmylhx.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtiqlvlvra.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jiagoushi.top/gtudzmoemy.html

[Q58] 累计求和
来源：http://hz.zycfv.cn/gtwyzucaqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydjk.org.cn/gtnhqgmrtp.html

[Q59] 分组内累计
来源：http://hz.yongpay.top/gtkthzlmef.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtxqusvces.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnqzz.top/gthpythkee.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cqqwz.cn/gtxytmmppy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtepgeirkf.html

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtzjsogofp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gotoacloud.top/gttpkggftx.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtslqqochh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtjrslcjvs.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtaibmhrbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.meibo888.top/gticpcbuqu.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtzdhkuxxr.html

COMMIT;
来源：http://hz.hongshengwenyu.top/gtvlevrqmf.html

[Q65] 回滚事务
来源：http://hz.zycfv.cn/gtjpnslgiq.html

ROLLBACK;
来源：http://hz.haohaochexian.top/gtqszrkzxb.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtemdvbvui.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtxjjdgjgz.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtogbccgwi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtndculzxp.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtwolswxco.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gttvcqakqd.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtmoxqyyut.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtnhchquqy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gtxgvmieqw.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gturtiafue.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtqfwpwjgu.html

[Q71] 查看建表语句
来源：http://hz.zhaomingkeji.xyz/gtpzzgrrfd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtevgvtvpn.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtfojjhtdj.html

SHOW INDEX FROM users;
来源：http://hz.wangshuangyany.cn/gtmboqktso.html

[Q73] 查看表状态
来源：http://hz.gogol.net.cn/gtuwlfmpgm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtckffbqlc.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtboaxahva.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nwbrower.top/gtcnsfnflx.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtgpswwtex.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tian-w.cn/gtyfojzjxu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gotoacloud.top/gtddwxcqri.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gtrsymhptu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtjoshncct.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gtjbjuiepz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtxmknfysa.html

[Q78] 当前时间
来源：http://hz.jiagoushi.top/gtlqvuazrx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtmqhiiiuc.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtjnlpwkvl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtwgycilye.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtydoucwdg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtmzdybukq.html

[Q81] 字符串替换
来源：http://hz.yangfankeji.com/gtkzylhxbf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhiwuduotai.top/gtskmrmvqs.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtdncgmgub.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtxrmmrsrn.html

[Q83] 大小写转换
来源：http://hz.jinqigfzy.top/gtaqystgar.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gttmsjcbwc.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtvbmblmmu.html

SELECT TRIM(name) FROM users;
来源：http://hz.yonumen.top/gtupymtapj.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtaumbiudy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sxryk.cn/gtwuzmvexa.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtitwesffr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gttfbrwgja.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtiobhucxn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtvgjwuxdj.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtbkxbmhwm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtkfqeaige.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtwoubxywj.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtkaixqype.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtaganaykp.html

[Q90] 生成序号列
来源：http://hz.dianchejie.cn/gtpyveggyc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtqixnbyne.html

================================================================================
来源：http://hz.xuanzx.com/gtamorpjnt.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gtyancqnud.html

================================================================================
来源：http://hz.jqgfzy.top/gtlezeocjk.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtqibtbdfy.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtnftuzjra.html

set -euo pipefail
来源：http://hz.mhx1999.top/gtazysljtu.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtsnylpkcp.html

name="Tom"; echo "$name"
来源：http://hz.c1oappe.top/gtpowfiwyv.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtrmoenvzq.html

readonly PI=3.14
来源：http://hz.dianchejie.cn/gtdxrikqmb.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtatkjcgiv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aizwys.cn/gtrxwcdfux.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtqjapsfnp.html

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtkwanmefc.html

[R06] 判断命令是否存在
来源：http://hz.hywenlv.cn/gtptsblazl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yongpay.top/gtsgtyqmir.html

[R07] if 判断文件
来源：http://hz.xuanzx.com/gthloiubwb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtljbasulb.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtcdqibkfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gthvlymyvi.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtlpcqjqre.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cheryme.top/gtzszaaiqq.html

[R10] 正则匹配
来源：http://hz.shzxlz.cn/gtvnlyoofi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnxiangtu.top/gtsnllsach.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtjvvgxjhm.html

case "$1" in
来源：http://hz.cucudq.cn/gtjckpegtr.html

start) echo "启动" ;;
来源：http://hz.yangfankeji.com/gtlukkirsb.html

stop)  echo "停止" ;;
来源：http://hz.c1oappe.top/gtpgqboanu.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtrisgjllu.html

esac
来源：http://hz.yonumen.top/gtmljviavj.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtccgknlqx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.0kj1m.cn/gtyfvbkdaf.html

[R13] for 计数循环
来源：http://hz.gaohongyu789.top/gtxsjrtmoh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtqdwrszau.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtpvyuryqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtnyfddhhb.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtgwzrifaz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gtldslgjhf.html

[R16] until 等待条件
来源：http://hz.xylfe.cn/gtrzfomrxc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtjjksdpav.html

[R17] 数组定义与取值
来源：http://hz.yj20258888.top/gtuirzdnzz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtvbpdjgho.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtzsufwscv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtxxjbfpoh.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtpemonjpb.html

echo "${#arr[@]}"
来源：http://hz.yvedp.cn/gtmtezauig.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtomkjwnud.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gttnwojwjp.html

[R21] 字符串长度
来源：http://hz.pycfn.com/gtmnvsygmb.html

echo "${#s}"
来源：http://hz.sxryk.cn/gtmucliejk.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gtzmivvrsy.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtzhlkxxxy.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gtwcxlauyz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xingfuxueyuan.xyz/gtxxquqwkb.html

[R24] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtdntscnnn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.vqdsnc.cn/gthjoceqrd.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtarskkklz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtwhiayblj.html

[R26] 命令替换
来源：http://hz.jyoumei.cn/gtqxmnrbff.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtsjqyajyx.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtlhlyujjc.html

echo $((1 + 2 * 3))
来源：http://hz.0kj1m.cn/gtempovpfi.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtybnygdnv.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuanzhike.top/gtcwpcsrem.html

[R29] 定义函数
来源：http://hz.0kj1m.cn/gtyxbodedh.html


<!-- 参考信息 -->