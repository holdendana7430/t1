代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtygqencit.html

C#:   if (x is null) {}
来源：http://hz.cqqwz.cn/gtkkjikyct.html

[P07] 防抖与节流
来源：http://hz.yueranfly.top/gtescjjulo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangdashe.top/gtmeykvwaj.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtssycfqzv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtnidkcbjv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtwngwogzr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yanxiufei.cn/gtybtbwlqo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtxbssoich.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtfhcxnnwm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtkaauwtem.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gthgaboqnw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtlpnmkwua.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtvubvshlj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gthbgvsjki.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtuunzwgfh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtwdaqzedm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nwbrower.top/gtdrazokrq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtxvgvbblg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtssnywbcu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthaoicrzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtetupdfpb.html

================================================================================
来源：http://hz.hammf.cn/gtqcsfybgh.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtlfsihotm.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gttvualfef.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtjncimalj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtcvmyolwr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.c1oappe.top/gtpptpydfy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhixingplan.top/gtfobppnvb.html

);
来源：http://hz.yvedp.cn/gtohdliekb.html

[Q02] 创建带外键的表
来源：http://hz.ivvv.top/gtovamnwrc.html

CREATE TABLE orders (
来源：http://hz.aizwys.cn/gthedqvnyi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtkidukesw.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtypjauzjp.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtkkhrehus.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.svipenyu.cn/gthvcixxew.html

);
来源：http://hz.xziqi.cn/gtwnnnbqgb.html

[Q03] 增加列
来源：http://hz.52xcode.cn/gtaxlgdzcx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtzicghved.html

[Q04] 修改列类型
来源：http://hz.hongshengwenyu.top/gtjhdxxpap.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtikgbrelp.html

[Q05] 重命名列
来源：http://hz.zhijiandao.cn/gtfjbicuet.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtrlwvudcc.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtrkziocfb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtyiipbuxx.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtmqmrdznt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtcbyciszh.html

[Q08] 创建普通索引
来源：http://hz.ehwqpu.com/gtcersjnzx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtextdxgis.html

[Q09] 创建唯一索引
来源：http://hz.sxryk.cn/gtyezvtupq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xinyue.icu/gtwnohyeuw.html

[Q10] 插入单行
来源：http://hz.52xcode.cn/gtnhsjglkk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtudwsydlb.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtdzvtvvyc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtdvnvmfxg.html

[Q12] 插入后取自增 ID
来源：http://hz.jlsjyb.cn/gtbeaomzeg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hongshengwenyu.top/gtuykuuuao.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtboxdxyfv.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtolpexixf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gogol.net.cn/gtnthwvgyf.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtttoqxzgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenzaomai.com/gtuymjievj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtfcmtbkni.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtocwtfneg.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtebbchkfi.html

[Q16] 查询指定列
来源：http://hz.gzhubu.top/gtkzmjsrot.html

SELECT id, name FROM users;
来源：http://hz.ybcxt.top/gtichkciaq.html

[Q17] 条件查询
来源：http://hz.yvedp.cn/gttjzxryvu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtyybrighl.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gtpqwywehy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hysaishi.cn/gtktrjpnfs.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtheqzilkk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtouflyxrb.html

[Q20] IN 列表
来源：http://hz.nanxinkj.top/gtmdnjkcpe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtdubfyaij.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtjpevknbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenzaomai.com/gthevrzbmo.html

[Q22] 排序
来源：http://hz.wangdashe.top/gtnureazom.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daria6918.cn/gtsydtsmut.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtnqedobwl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gttndaqhnu.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gtpsoihymh.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtoqepudux.html

[Q25] 只取前 N 条
来源：http://hz.nanxuanxn.top/gtefroynsx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gtxfcubebe.html

[Q26] 计数
来源：http://hz.hfpthk.cn/gtzfansrux.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtoowbxdko.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtaiywnpxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xziqi.cn/gtepoghwhp.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtbbfqgmfc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtvvkevefm.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtplucdsum.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gtcueimqha.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtxsdmrdqs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtebpuuxmw.html

[Q31] 分组后过滤
来源：http://hz.hysaishi.cn/gtabqeusfm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtniwfakib.html

[Q32] 分组拼接字符串
来源：http://hz.yvedp.cn/gtetukcljh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gttlcbsjtv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.redwolf501.top/gtwkoblell.html

[Q33] 多列分组
来源：http://hz.zhiwuduotai.top/gtmyxjtazj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigfzy.top/gttfmzizhp.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtcvrrhxor.html

SELECT * FROM (
来源：http://hz.9152youxi.cn/gtkfsaxulh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtvysrdrid.html

) t WHERE rn = 1;
来源：http://hz.cqqwz.cn/gtamwgmdrc.html

[Q35] 内连接
来源：http://hz.yangfankeji.com/gtaxmosaaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gthzfjjoes.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtyofdldrb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtbfhwtmmf.html

[Q37] 右连接
来源：http://hz.fengsongda.top/gtwkepdgtz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtjlltvsax.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gtasmwgxiu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gtunppqjkn.html

[Q39] 自连接（查上下级）
来源：http://hz.zdqjudy.top/gtagymvqim.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtkjwfimyy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtgooyhkmd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtnxhtomtp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtplbhcnho.html

[Q41] 多表连接
来源：http://hz.cashguo.top/gtbfvnxfip.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtgectnlxm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gtgvegbmnc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gttstvfwnm.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gttvfuqsqy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtszusmobw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ybcxt.top/gtekjfxagi.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtgrfteubm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtyuxjhzcx.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtcmvouaft.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sufxvd.cn/gtcfgghqgd.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgfzy.top/gtwfobdxak.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtmndfeddo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtovhfqnez.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtcwjavwmk.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gtzrxaivvp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtnpktwuaa.html

[Q48] CTE 公用表表达式
来源：http://hz.tianlin.xyz/gtyifpvxpx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtekzilbvv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtzbcccflq.html

[Q49] 更新单行
来源：http://hz.yuxming.cn/gtkpiflvpm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shzxlz.cn/gtywssstvt.html

[Q50] 批量更新
来源：http://hz.zhiwuduotai.top/gtchjsyshl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtbzqrmjkz.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtiftoxiun.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shanyushiyangtech.top/gtqvexbheh.html

[Q52] 删除指定行
来源：http://hz.dashuyun.cn/gtkosmyyww.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gttdoujkvu.html

[Q53] 按条件删除
来源：http://hz.gzhubu.top/gtauqautwl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtsvavkfpf.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtepsxudhj.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtyvskluci.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtaczwrohu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtukjhfvkr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yueranfly.top/gtpnqscsod.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.0kj1m.cn/gtamsolruh.html

[Q57] 行号
来源：http://hz.aizwys.cn/gtiygglpxx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtmkfsncmz.html

[Q58] 累计求和
来源：http://hz.jiagoushi.top/gtxrzehglb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtxopadzxz.html

[Q59] 分组内累计
来源：http://hz.hfpthk.cn/gtieruwgbj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jiagoushi.top/gtlcvswmcr.html

[Q60] 取上一行 / 下一行
来源：http://hz.andypj.xyz/gtlefzfotj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtesfofise.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxinkj.top/gtfshnwzmd.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtqojsgonl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cqqwz.cn/gtebczgycb.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtjofxuceo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtzfxofhpp.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtdnsxueyu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtrpetamhu.html

[Q64] 提交事务
来源：http://hz.ybcxt.top/gtznepqcgk.html

COMMIT;
来源：http://hz.cqqwz.cn/gtekawirzp.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtifgynzkg.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtmwgvjndf.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gtrxvptldo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.redwolf501.top/gtyaexalcb.html

[Q67] 设置隔离级别
来源：http://hz.chenjidiqi.icu/gtxluddquw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtmluucill.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtdbhvjfse.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtrpuojwbt.html

ROLLBACK TO sp1;
来源：http://hz.ywan-chungtsiang.top/gtljgmwlje.html

[Q69] 查看执行计划
来源：http://hz.dashuyun.cn/gtihjhqngk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daxiang520.top/gttcvpvkkq.html

[Q70] 更新统计信息
来源：http://hz.hongshengwenyu.top/gtfzmkdygb.html

ANALYZE TABLE users;
来源：http://hz.snrcjt.cn/gtnntdrexq.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtbinfzqzm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj202588.top/gtxmujywfh.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtyjkpwfvt.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtzqdhesob.html

[Q73] 查看表状态
来源：http://hz.havefunace.top/gtwphzavup.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtulueykui.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtowzkatsp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gthkuandvd.html

[Q75] 日期格式化
来源：http://hz.haohaochexian.top/gtxzlddkoq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gtuhjxjoui.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtjeysxfek.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gttimkoahr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.bjfxy.top/gtykdopphl.html

[Q77] 时间加减
来源：http://hz.xuetiantiany.cn/gtanwfwwgf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.smart0.xyz/gtxawcypfz.html

[Q78] 当前时间
来源：http://hz.nanxinkj.top/gtyfxsolgj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtsiqcmstt.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtserxywum.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gttuoixuac.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gthzpuefmv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gttspeqbhf.html

[Q81] 字符串替换
来源：http://hz.chenjidiqi.icu/gterlcqoyh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtpvvsjpho.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtjhzflebu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.redwolf501.top/gttjjaicrj.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gthuzsdtaj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gthglpoyux.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtpzaztaan.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gtvpqvjmcp.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gterkgcssj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gttdgllipu.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtorbucyoz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtmrdmltyf.html

[Q87] JSON 字段做条件
来源：http://hz.9152youxi.cn/gtaaxgumeb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.0kj1m.cn/gtudsahvvl.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtakphzasp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gticvqpdfx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gtecjpvydt.html

[Q89] 判断表是否存在
来源：http://hz.andypj.xyz/gtptfmvneo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnqzz.top/gtckhjqzev.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gtxyooyizg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtgzeqksnt.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtvfrlmcgb.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtcsquyouc.html

================================================================================
来源：http://hz.guowangkeji.top/gtpsgdqver.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtzubmslzn.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtortallpd.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtxdqbujfc.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtsigyxvrh.html

name="Tom"; echo "$name"
来源：http://hz.zhaomingkeji.xyz/gtcaliqgrf.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtsgbkcqpq.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtufleydhr.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtwqpnicyk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhixingplan.top/gtahgubsmi.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gthkmoyzbe.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtfsckjjsc.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtqfaipxeh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yonumen.top/gtymqadtms.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtdywfmdec.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sxryk.cn/gtxstwhyoy.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtrilinoms.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtiwpxavgt.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtzvieqena.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.quarkkingdee.top/gtrqyqfgmv.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gtkhadrzuy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.c1oappe.top/gtfhxtkiqx.html

[R11] case 多分支
来源：http://hz.yueranfly.top/gtluswwhrc.html

case "$1" in
来源：http://hz.yj20258.top/gtwopfihpc.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtzvknxkds.html

stop)  echo "停止" ;;
来源：http://hz.pengpengdd.cyou/gtuyqenahe.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtrlxnyoau.html

esac
来源：http://hz.gaohongyu789.top/gtnvzzbnar.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtvanpjsdf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtltselcrs.html

[R13] for 计数循环
来源：http://hz.zycfv.cn/gtyjxcnydi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtasuryqfj.html

[R14] C 风格 for
来源：http://hz.guannengcc.top/gtuvnnuuov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtsznpwsbk.html

[R15] while 逐行读文件
来源：http://hz.dianchejie.cn/gtkahooqcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtqhcigczb.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gthjordunz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtwdoglcxp.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtgcznugod.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zycfv.cn/gtmqekeqzj.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtdcglqqvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gtsudmwril.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtrgiorjup.html

echo "${#arr[@]}"
来源：http://hz.nanxinkj.top/gtlzsksknw.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtzyvgmfuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.kuanghao11.cn/gtzdnarreu.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtyydbjcpk.html

echo "${#s}"
来源：http://hz.xylfe.cn/gtzrukyvdk.html

[R22] 截取子串
来源：http://hz.meibo888.top/gtesyzgcal.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtswpzozbk.html

[R23] 字符串替换
来源：http://hz.cqqwz.cn/gtjffrbmle.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtulqjhxmp.html

[R24] 大小写转换
来源：http://hz.guowangkeji.top/gtrwcmityr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gttgyicyok.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtgdnxmgnt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hammf.cn/gtuoqbnmdg.html

[R26] 命令替换
来源：http://hz.cucudq.cn/gtslsmqxkg.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gterfamcud.html

[R27] 算术展开
来源：http://hz.sysykeji.top/gtinjsytrk.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtvwvebcub.html

[R28] 浮点运算
来源：http://hz.bjfxy.top/gtmtwxsnkv.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtccrenxqj.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtvoxgenjl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtfqrwqyac.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtdznupjwn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtbezfouxa.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gtdftsmhuq.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtepqwucjm.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtiaouhynw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtnniclesr.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtidqgpuau.html


<!-- 参考信息 -->