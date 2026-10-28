代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gthcoywxnh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ehwqpu.com/gtmtsozphk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj202588.top/gtxzzcjicx.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtvmzjsrcu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtxirkkvin.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuanzhike.top/gtoafpgknh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gtkexbcrsy.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtbwpqxouq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtsidavxzt.html

TS:   if (x == null) {}
来源：http://hz.cheryme.top/gtwdltcghw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtvfgqgufe.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtxmadxxno.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gzhubu.top/gthbecbzbb.html

C#:   if (x is null) {}
来源：http://hz.hammf.cn/gtaildibmx.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gticlyovcg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hysaishi.cn/gtljwmukhv.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gtynishtjq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnqzz.top/gtnqzuunvp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtibyvamdc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtzmvdezyz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gttylglobo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hywenlv.cn/gtumbaxqsg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtnkivoidk.html

[P08] 处理浮点精度问题
来源：http://hz.snrcjt.cn/gtogwucplx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ybcxt.top/gtqqfjffej.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xinyue.icu/gtoimlucgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenzaomai.com/gtquwukhma.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gterayxxvb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jqgfzy.top/gtzdcrkqvt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.smart0.xyz/gtxjrczhkm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinyuanbaomall.cn/gtbbfbxtdi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jyoumei.cn/gtmwqlmhky.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtsukewbbo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.havefunace.top/gtjcwcincy.html

================================================================================
来源：http://hz.nanxinkj.top/gtmenrnrgy.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtqitborix.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtrninzjkn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtmsahxwyi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gtspaestyj.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtuezxueev.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ivvv.top/gtuyogntdp.html

);
来源：http://hz.zhijiandao.cn/gtwvncfzsk.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtmutlftxw.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtwheiuuco.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtrgwzwkkn.html

user_id INT NOT NULL,
来源：http://hz.yangfankeji.com/gtaigurrlj.html

amount DECIMAL(10, 2),
来源：http://hz.zhijiandao.cn/gtnywdyiob.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jiagoushi.top/gtjcahmern.html

);
来源：http://hz.wangdashe.top/gtymprkzuc.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtsszmeifx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtlflzvwte.html

[Q04] 修改列类型
来源：http://hz.xuanzx.com/gtsdyvhfam.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtttcacngy.html

[Q05] 重命名列
来源：http://hz.nanxuanxn.top/gtyjmttpzi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj202588.top/gthposshim.html

[Q06] 删除列
来源：http://hz.havefunace.top/gtebdrqmrm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jqgfzy.top/gtvprxmgbc.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtslimizvs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tanke756.top/gthgorzrdo.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtqhqrsaqd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtyobszlvz.html

[Q09] 创建唯一索引
来源：http://hz.hywenlv.cn/gtcngqjebu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ppjwa.cn/gtvegwhxev.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtmixbeisx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gtzuxctawu.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gttlisdzbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtbmnnegbe.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtzjuhzsdf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydjk.org.cn/gtvvlclspx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.smart0.xyz/gtjcjvukvq.html

[Q13] 忽略重复插入
来源：http://hz.nanxuanxn.top/gtsswediqf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yangfankeji.com/gtxsjsnqox.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gttjedfayz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gthfikxqck.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tian-w.cn/gtftrtlxdh.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gtvcydunnv.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtapxbjrrq.html

[Q16] 查询指定列
来源：http://hz.nwbrower.top/gtsqbzxorm.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtgvmifonk.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtpyyqizlg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtaewypuhl.html

[Q18] 模糊匹配
来源：http://hz.smart0.xyz/gtzqbugarh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gttpwtppwg.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtlgoxxajr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtnxigutxh.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gthyqikqrr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhijiandao.cn/gtrmtmzhsl.html

[Q21] 空值判断
来源：http://hz.316326.xyz/gtxstpysrv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtfezpdhcc.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtfewoubmy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nwbrower.top/gtvfilncfb.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtonhzjora.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gtzdhooywx.html

[Q24] 去重
来源：http://hz.tanke756.top/gtaqqkdpoz.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258888.top/gtdqnilmqt.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gtfnfzhgtu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtsjdorhbb.html

[Q26] 计数
来源：http://hz.zhongyouzk.top/gtvrhcjzpv.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtyiirmgvv.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtdadifziy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtvabynvxg.html

[Q28] 求和与平均
来源：http://hz.kuanghao11.cn/gtziqsbmoc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtgacnthds.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtsdqwjwro.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtxuacnwgs.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtvgkrytzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gthrlahwde.html

[Q31] 分组后过滤
来源：http://hz.pycfn.com/gtwarssppv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.daria6918.cn/gtchcmjyxr.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigfzy.top/gtzrpclyhc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtvrxllepd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtismiiunv.html

[Q33] 多列分组
来源：http://hz.zhijiandao.cn/gtzrjfdquc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.wangdashe.top/gthgdeeuky.html

[Q34] 每组取第一条
来源：http://hz.chenzaomai.com/gtuckgfywk.html

SELECT * FROM (
来源：http://hz.shanyushiyangkeji.top/gtmbsimkoa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtoweagliv.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtclsbzmce.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtgcjgtazb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtjcjzoxej.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtmmfswmhy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtndcxdqan.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtttchswhf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guowangkeji.top/gtovcyrfus.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtpwwuknkw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gtdkcszina.html

[Q39] 自连接（查上下级）
来源：http://hz.gzhubu.top/gtvpqauyuc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtwdljcuuq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.smart0.xyz/gtejxqsrmc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhengqikj.top/gtsicnyqzt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xylfe.cn/gtdduqgzzg.html

[Q41] 多表连接
来源：http://hz.zdqjudy.top/gtqydsoxes.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jianghu66.top/gtxuvnqvye.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtglrbkoch.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtodoosdin.html

[Q42] 连接条件附加过滤
来源：http://hz.yangfankeji.com/gtzlercbeb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gtshglvplt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtezywfypy.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gthkgxcebi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtvvpgisnb.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gturbxygvr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtxixcnlxs.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtjkmhsazf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtwiajfbff.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtkqlsmwtk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtofszxlmm.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtesfyaaqe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinghuilouyu.cn/gtyfathelx.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangtech.top/gtgpvfmyhi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yueranfly.top/gtmjytkqhz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shangyingyoupin.top/gthgeviufp.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtcfvxtyoz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtcxdkylew.html

[Q50] 批量更新
来源：http://hz.yonumen.top/gtctzldydx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtpgbkbvsp.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtpnrzdlbt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtahprsoid.html

[Q52] 删除指定行
来源：http://hz.ybcxt.top/gtrfutecls.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yueranfly.top/gtzspadday.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtykjkhlkt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtuyqbftli.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtdumbeqbu.html

TRUNCATE TABLE logs;
来源：http://hz.sxryk.cn/gtqmasmwss.html

[Q55] 排名（并列占位）
来源：http://hz.vqdsnc.cn/gtdnfzdpnj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtvxdicaih.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtnulivebc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtiznsmqmu.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtiywpioqe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.mhx1999.top/gtmyuxriuf.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gtigixwyuh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.andypj.xyz/gthaovaztk.html

[Q59] 分组内累计
来源：http://hz.havefunace.top/gtavjhoymy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtcvimpwaj.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gthaknzfdo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxuanxn.top/gtauelreqj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtqokzrswi.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtrzvxbasq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.feifeiyinyue.top/gtwwvztauu.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtsuvgpsva.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtgawnqlxq.html

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtwpdawyie.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hywenlv.cn/gtihezcwqx.html

[Q64] 提交事务
来源：http://hz.hfpthk.cn/gtyjayjrki.html

COMMIT;
来源：http://hz.daxiang520.top/gtiifhbcyj.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gthfubrtiv.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gthcvcybjq.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtxpjweozp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ydzc1.top/gtbzdnbkmx.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gthkhlpdrs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtsgpfqpbx.html

[Q68] 保存点
来源：http://hz.cashguo.top/gthzsulpjt.html

SAVEPOINT sp1;
来源：http://hz.ydjk.org.cn/gtlypmvauw.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtojzrxhrv.html

[Q69] 查看执行计划
来源：http://hz.vqdsnc.cn/gtmzefajsr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj202588.top/gtxviyrwdd.html

[Q70] 更新统计信息
来源：http://hz.9152youxi.cn/gtonzgerdh.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gtnvfjzuxf.html

[Q71] 查看建表语句
来源：http://hz.dashuyun.cn/gteadhbdet.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ppjwa.cn/gtwwuxbmxb.html

[Q72] 查看索引
来源：http://hz.hnxiangtu.top/gtwwkyofir.html

SHOW INDEX FROM users;
来源：http://hz.jianghu66.top/gtqicojkbz.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtcliyaqji.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hongshengwenyu.top/gtryylmabd.html

[Q74] 强制使用索引
来源：http://hz.chenjidiqi.icu/gtilqvfbku.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yonumen.top/gtyxdxukdf.html

[Q75] 日期格式化
来源：http://hz.feifeiyinyue.top/gtjrzgffxm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtkvxkneqj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hongshengwenyu.top/gtfithmuos.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtosnnixuj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtpvlnhldg.html

[Q77] 时间加减
来源：http://hz.xingfuxueyuan.xyz/gtiyuqnsgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtuajqevdm.html

[Q78] 当前时间
来源：http://hz.guannengcc.top/gtstvwuckw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtssvbjnfu.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gtkufwxbup.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtlsfgpilm.html

[Q80] 字符串截取
来源：http://hz.c1oappe.top/gtwsfbhqbr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sweek.top/gtqapszett.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtaljdkjqr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtncostfnm.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtdqrkuciz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gtrirzgksk.html

[Q83] 大小写转换
来源：http://hz.gogol.net.cn/gtjmgsclqk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gtaofvkzdz.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtrrurqxpb.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gthwcpvacu.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtcehyfesr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtemrpiwtg.html

[Q86] 读取 JSON 字段
来源：http://hz.kuanghao11.cn/gtetfwzxqu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ehwqpu.com/gtwrolumit.html

[Q87] JSON 字段做条件
来源：http://hz.9152youxi.cn/gtvlvxlaoz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gtgbjvzfyi.html

[Q88] 行转列（条件聚合）
来源：http://hz.aibaodan.cn/gtvexbaufq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtodslgqhp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hysaishi.cn/gtqenmwemr.html

[Q89] 判断表是否存在
来源：http://hz.gotoacloud.top/gtkwexrywm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtgduxuxfw.html

[Q90] 生成序号列
来源：http://hz.quarkkingdee.top/gtkuwcwnjv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jiagoushi.top/gtumskcqtq.html

================================================================================
来源：http://hz.daxiang520.top/gtgemknvuu.html

R. Bash 专题
来源：http://hz.hnqzz.top/gtnmembitu.html

================================================================================
来源：http://hz.jqgufenzy.top/gtuedkqtru.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtgojezaij.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gttfhblmkk.html

set -euo pipefail
来源：http://hz.shzxlz.cn/gtmgosriwd.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtflvosatf.html

name="Tom"; echo "$name"
来源：http://hz.cucudq.cn/gtsmpzzwlu.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtunqpcabp.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtqyozzldo.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gttenjkmlx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guannengcc.top/gtldfslxjh.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gttiukxdda.html

name="${1:-default}"
来源：http://hz.jinghuilouyu.cn/gtjgtmngfc.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gtalkmehaf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gtgqxgyyrh.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtivginesp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtwspljhli.html

[R08] 数值比较
来源：http://hz.316326.xyz/gtmwyeeytj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtuctfemkv.html

[R09] 字符串比较
来源：http://hz.316326.xyz/gtznvydeyc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.quarkkingdee.top/gtbipkmbig.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtxyhsmswj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gteoqqgfco.html

[R11] case 多分支
来源：http://hz.cdnleiting.top/gtmpqdrpup.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gttolqynea.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gthnznftrn.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtaelwjvlp.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gtbohftxgl.html

esac
来源：http://hz.nanxinkj.top/gtwrkyvngv.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gtahnaooga.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtdbgnptdg.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gthrgqghms.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ehwqpu.com/gtjnskisjf.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtdnckqcla.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yuanzhike.top/gtcogywkxd.html

[R15] while 逐行读文件
来源：http://hz.jinghuilouyu.cn/gtubxlmjfo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtssdievxm.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtaxqbtlhj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cdnleiting.top/gtwkjcsasd.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtvfhqizkv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtuhntimta.html

[R18] 遍历数组
来源：http://hz.sufxvd.cn/gtwtselqcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangkeji.top/gtzfkwcljz.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtwwguarbz.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gtbsrafbzn.html

[R20] 关联数组（字典）
来源：http://hz.cdnleiting.top/gtlushfxbu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtoiqttedr.html

[R21] 字符串长度
来源：http://hz.zhiwuduotai.top/gtcefhtuiy.html

echo "${#s}"
来源：http://hz.gogol.net.cn/gttygswyuz.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gttszrbnrt.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtezuqbkfc.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gttntvddsf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtndxubkyd.html

[R24] 大小写转换
来源：http://hz.shuidangran.top/gtwvjchwac.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtgwfnbrjt.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtziiqmkvx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtiukhkwzt.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gticvpuwpl.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gttgdppazt.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtsgdtzerk.html


<!-- 参考信息 -->