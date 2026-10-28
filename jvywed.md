代发 wailian999

PHP:  // 手写时间戳比较
来源：http://hz.chenlongwang.top/gtvvutodwu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtzrtzyorv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtzufktgii.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.havefunace.top/gttowteupp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtxsihqrii.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhixingplan.top/gtqpzmtwpm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gtigumcdzw.html

[P08] 处理浮点精度问题
来源：http://hz.yuxming.cn/gtljlsqlwt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtjdgtlpoq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.bjfxy.top/gtgnbzzyzx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zdqjudy.top/gttdddcgjr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gtvwjbtokj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtkxydljyq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gteeuazajt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtzlgdvzdj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtopsipedf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgnvgxqmy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtwpibiipw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtifcodtyr.html

[Q01] 创建表
来源：http://hz.andypj.xyz/gtnfybfher.html

CREATE TABLE users (
来源：http://hz.nanxinkj.top/gtjxrjcnwi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gtvdelucrm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gogol.net.cn/gttjrjruva.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xinyue.icu/gtacuwuimz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtofeaagik.html

);
来源：http://hz.wangshuangyany.cn/gtjqsklxqg.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtucvmctjx.html

CREATE TABLE orders (
来源：http://hz.zdqjudy.top/gtfaniwyzx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtjjdqmhlf.html

user_id INT NOT NULL,
来源：http://hz.gaohongyu789.top/gtqfcebtjf.html

amount DECIMAL(10, 2),
来源：http://hz.xuetiantiany.cn/gtaxuuavnb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gtvvgjpnwz.html

);
来源：http://hz.hongshengwenyu.top/gttbayrwuc.html

[Q03] 增加列
来源：http://hz.tanke756.top/gtjskqsanp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jianghu66.top/gtqufejpyd.html

[Q04] 修改列类型
来源：http://hz.zdqjudy.top/gtkmujwmcu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgufenzy.top/gtjpxkpqey.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtwnlsmtkz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhengqikj.top/gthcvshqnn.html

[Q06] 删除列
来源：http://hz.gaohongyu789.top/gthwvctpnb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgufenzy.top/gtmatvggaq.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtioyxmski.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gthoaxhylz.html

[Q08] 创建普通索引
来源：http://hz.xuetiantiany.cn/gtozselnin.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gtkygfbwcj.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtvsjgimxb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.feifeiyinyue.top/gtkoziufye.html

[Q10] 插入单行
来源：http://hz.xuanzx.com/gtriedmcis.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tanke756.top/gtkaownghv.html

[Q11] 一次插入多行
来源：http://hz.wangshuangyany.cn/gtuayzbonj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guowangkeji.top/gterrjlvzz.html

[Q12] 插入后取自增 ID
来源：http://hz.cqqwz.cn/gtkuuumhnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gogol.net.cn/gtmgjsnxwu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtbsobiobv.html

[Q13] 忽略重复插入
来源：http://hz.zhengqikj.top/gtcbdweofu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhiwuduotai.top/gtrqqlaind.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtesptqpxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.meibo888.top/gtnleoirwd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yangfankeji.com/gtphjtnfnb.html

[Q15] 查询全部
来源：http://hz.fengsongda.top/gtsfeolxpq.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gtavlqgenm.html

[Q16] 查询指定列
来源：http://hz.jinqigufen.top/gteklpniam.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtinveodhi.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gtcgprkugs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtadowuezw.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtffbboejb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtzzmjvixx.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtemstqazd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtbwssnboz.html

[Q20] IN 列表
来源：http://hz.fzhhl.top/gtxmoasyhk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtrcserkot.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gthyalutjs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hywenlv.cn/gtmuprjdyb.html

[Q22] 排序
来源：http://hz.cheryme.top/gtwtoaunim.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtsahaymxt.html

[Q23] 分页
来源：http://hz.ivvv.top/gtpniigsur.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hongshengwenyu.top/gtglfcjadl.html

[Q24] 去重
来源：http://hz.hnxiangtu.top/gtllpwzfbz.html

SELECT DISTINCT city FROM users;
来源：http://hz.yvedp.cn/gtjwbjhpwg.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtdipeuaml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gttuhaqmyc.html

[Q26] 计数
来源：http://hz.ivvv.top/gtmoaavljj.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gtyaytffnt.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtvgxnhyfz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtehrbxmnh.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gthohpzzqr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zycfv.cn/gtgvqpdfdi.html

[Q29] 最大最小值
来源：http://hz.svipenyu.cn/gtkgujsrpt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pycfn.com/gtavddyqtr.html

[Q30] 分组统计
来源：http://hz.yuxming.cn/gtsxmmfhff.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtpbujzboj.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtlgkbnceb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtuvmwfeew.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gttckvrtgn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtceaebpfq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gttveihifa.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtayjaascv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gttdnccnsj.html

[Q34] 每组取第一条
来源：http://hz.tian-w.cn/gtevoqxpwx.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gttnlwwpvm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhongyouzk.top/gtdlogabzm.html

) t WHERE rn = 1;
来源：http://hz.cucudq.cn/gtsitvqpol.html

[Q35] 内连接
来源：http://hz.cucudq.cn/gteynygwll.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtwfrmxhao.html

[Q36] 左连接
来源：http://hz.guowangkeji.top/gtuxraxchy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtqmltphja.html

[Q37] 右连接
来源：http://hz.hongshengwenyu.top/gtjifxcpir.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258.top/gtzwrugcdn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtpuxlbvds.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtdeclijxr.html

[Q39] 自连接（查上下级）
来源：http://hz.jyoumei.cn/gttvpbncwg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtmnzrdtew.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gotoacloud.top/gtctfulrce.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtuqcwdhou.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jyoumei.cn/gtjkhjrigf.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtvugqoagg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhixingplan.top/gtkkxuuvca.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yanxiufei.cn/gtqimxiouj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtdnrzxuuo.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtpmcrnbxm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtxpsvmrvr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hammf.cn/gtjgyhykxa.html

[Q43] 标量子查询
来源：http://hz.ydjk.org.cn/gtmnhnbkss.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gtoskmqkbj.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtmhomvsxx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gthzgcqsvq.html

[Q45] EXISTS 判断存在
来源：http://hz.meibo888.top/gtvojbudka.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtfxbsfwyo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenzaomai.com/gtznzwwrfm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gteuexebhm.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtfxprkbya.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtinapjxpe.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtnqzrufsx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhiwuduotai.top/gtxjkmalmg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtjmrfbxct.html

[Q49] 更新单行
来源：http://hz.jiagoushi.top/gtvzfgflmm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hywenlv.cn/gtzfepgjfn.html

[Q50] 批量更新
来源：http://hz.xylfe.cn/gtbxpwdchf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhongyouzk.top/gtbvfyxugk.html

[Q51] 用子查询更新
来源：http://hz.yangfankeji.com/gtjzglnnpj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtbrzrmrnv.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtcgiyvqhp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtbwycjcnr.html

[Q53] 按条件删除
来源：http://hz.redwolf501.top/gtcsufczfy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sweek.top/gtsfszpjhr.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtoaczzzvt.html

TRUNCATE TABLE logs;
来源：http://hz.gogol.net.cn/gtbfgfhykd.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtcstnlmwi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtwaqmhpuc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtsxfyiugj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtyqppmsjl.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtqwitnjrn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtpuftweod.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gteiwfkxno.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtscmoekvk.html

[Q59] 分组内累计
来源：http://hz.tianlin.xyz/gtfpkgcgty.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jlsjyb.cn/gtqasehsmq.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtbxogqftc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtuvczyobq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.kuanghao11.cn/gthgzymefo.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gttoxyfupp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtczkytzna.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gtaabjizqf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtbsdpzcit.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtsnhghkps.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtzauqlpqk.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtpriuzmpz.html

COMMIT;
来源：http://hz.hfpthk.cn/gtwcygxgxx.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtjgfujwrv.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gtddutiibt.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtrruipplw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xingfuxueyuan.xyz/gtgueavnoy.html

[Q67] 设置隔离级别
来源：http://hz.yongpay.top/gtrlickdoy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.52xcode.cn/gtwyhgvszm.html

[Q68] 保存点
来源：http://hz.fzhhl.top/gtzryyvwrm.html

SAVEPOINT sp1;
来源：http://hz.yuxming.cn/gtxvujmbvk.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtxwctupav.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtgfvwbtsi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.havefunace.top/gtdbptrfrf.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtohkqauut.html

ANALYZE TABLE users;
来源：http://hz.zhixingplan.top/gtqqwwkrjl.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtpzkuzgtg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtgeguwwkv.html

[Q72] 查看索引
来源：http://hz.zhaomingkeji.xyz/gtbochafzb.html

SHOW INDEX FROM users;
来源：http://hz.cucudq.cn/gthhvgbpve.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtsunryfzj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuanzx.com/gtaqjokoqy.html

[Q74] 强制使用索引
来源：http://hz.yanxiufei.cn/gtahzgqxzc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtkhknwxpe.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gtxrpdmlmr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fengsongda.top/gtponebcam.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtasauqooi.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtsqwvfesa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yangfankeji.com/gtgrvfnjws.html

[Q77] 时间加减
来源：http://hz.hammf.cn/gtnxuqcigt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xinyue.icu/gtcljfbjxa.html

[Q78] 当前时间
来源：http://hz.zhoulong.xyz/gtnkrradas.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtzgcppkol.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtqwhplfdc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtumiucjfo.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtbejeufpn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtzscvxfwq.html

[Q81] 字符串替换
来源：http://hz.c1oappe.top/gtiszlmdiz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtenxywcse.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtnnvmiocw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtarrjaeqv.html

[Q83] 大小写转换
来源：http://hz.ehwqpu.com/gtduipanbx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtkbomlbvj.html

[Q84] 去除首尾空格
来源：http://hz.feifeiyinyue.top/gtajosvsqb.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtdbsngzab.html

[Q85] 数值取整
来源：http://hz.ybcxt.top/gtvzbcxvpf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtayekitmq.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtcijdexvd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenjidiqi.icu/gtkcbrxzsv.html

[Q87] JSON 字段做条件
来源：http://hz.aizwys.cn/gtlyqeylmn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtucmwcasy.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtasmoelja.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gtibbymkjl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.haohaochexian.top/gtyvmgtzsc.html

[Q89] 判断表是否存在
来源：http://hz.316326.xyz/gtaifmufbq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtpskuolkk.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gtlunnbsbe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gaohongyu789.top/gtamymwzcm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcenfzpzj.html

R. Bash 专题
来源：http://hz.smart0.xyz/gtcqzkqmkr.html

================================================================================
来源：http://hz.fengsongda.top/gtvnmnnrtq.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtnorcxjvd.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtcqmrifde.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtgjdwyvgk.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtrlydptzn.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtgjjjipvc.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gthfkjlgmi.html

readonly PI=3.14
来源：http://hz.xinyue.icu/gtprzcpsaq.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gtdlqibmcz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtodvmakji.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtydzjsrqn.html

name="${1:-default}"
来源：http://hz.wangdashe.top/gtijitpjet.html

[R06] 判断命令是否存在
来源：http://hz.cdnleiting.top/gtbufreiof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.iojbl.cn/gtlqlhhqgu.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtdlrxlawd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtryhmyhjf.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtwufhmren.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj202588.top/gtoxngxzat.html

[R09] 字符串比较
来源：http://hz.dianchejie.cn/gtabtcslxf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.smart0.xyz/gtvfxavspg.html

[R10] 正则匹配
来源：http://hz.c1oappe.top/gtfoewglco.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenlongwang.top/gttfimzhfc.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtbkjkgpxi.html

case "$1" in
来源：http://hz.jianghu66.top/gtusftrbmf.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtjbfqroth.html

stop)  echo "停止" ;;
来源：http://hz.hysaishi.cn/gtzicbtjbh.html

*)     echo "未知命令" ;;
来源：http://hz.shangyingyoupin.top/gtnzawuxic.html

esac
来源：http://hz.yonumen.top/gtcqtecgms.html

[R12] for 遍历文件
来源：http://hz.gogol.net.cn/gtlaeootzs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nwbrower.top/gtpokdxwfu.html

[R13] for 计数循环
来源：http://hz.cheryme.top/gtibwccpag.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtozjumngw.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtpiwdltkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tian-w.cn/gthwkwkzeb.html

[R15] while 逐行读文件
来源：http://hz.xylfe.cn/gtbqkeprgp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.haohaochexian.top/gtbrgitujm.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtportkmiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jianghu66.top/gtyqkkdrhp.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtsweqlhar.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtxagrgquq.html

[R18] 遍历数组
来源：http://hz.52xcode.cn/gtritfxcvf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtjrgexrbg.html

[R19] 数组长度
来源：http://hz.cqqwz.cn/gttwfdwexn.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtydwlejxj.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtupfyiyue.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guowangkeji.top/gtshsxzhgm.html

[R21] 字符串长度
来源：http://hz.yanxiufei.cn/gtkleddxye.html

echo "${#s}"
来源：http://hz.ehwqpu.com/gtaowxdbhu.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtnykfvurb.html

echo "${s:0:5}"
来源：http://hz.tianlin.xyz/gtpnkmwdhx.html

[R23] 字符串替换
来源：http://hz.cheryme.top/gtttdrbrno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtpxctkzks.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gtaalpkcjt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sysykeji.top/gtxobuhxjq.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtidfrascg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtzrhtbuxt.html

[R26] 命令替换
来源：http://hz.316326.xyz/gtwxzlfpfg.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtjysztsdw.html

[R27] 算术展开
来源：http://hz.yongpay.top/gthrqhfwxm.html

echo $((1 + 2 * 3))
来源：http://hz.ydjk.org.cn/gtyyxmvyqj.html

[R28] 浮点运算
来源：http://hz.hfpthk.cn/gtzfxgshux.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtvxsizxpa.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtbvhtccbr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtplxagmhw.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gtnvxvsmxm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gttdbuqxqb.html

[R31] 局部变量
来源：http://hz.cashguo.top/gtkrrsejxp.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtbfxpjkgv.html

[R32] 参数个数校验
来源：http://hz.tianlin.xyz/gthpnqecuf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gtkiogiqns.html

[R33] 捕获错误并提示行号
来源：http://hz.pengpengdd.cyou/gtnhdbyebo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtcwwrjjzz.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtgkgwscvx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtyizfojck.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtirtjclpz.html


<!-- 参考信息 -->