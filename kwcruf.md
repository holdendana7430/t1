代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtbhjgwdsd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangdashe.top/gtxzrjryvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtehaclfef.html

Ruby: a == b
来源：http://hz.cdnleiting.top/gtvgjgmmkm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nanxuanxn.top/gtmzapdavp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtinmrhkfk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gteeaafjff.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtanqfzmhy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtazxopvmb.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtzovzyffy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtvwpkhami.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtswmscmhg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtzxkuphpz.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtfyaqvlfx.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gtifxfkeno.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtudicycji.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtiyuenfcf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtichpjate.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtisttjthq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtfaesipng.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dianchejie.cn/gtaxdrysya.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yvedp.cn/gtszwgmpid.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.andypj.xyz/gtzakkajvd.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258888.top/gtzyrowtav.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtmnjscrez.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtpporauxj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtvgskvmoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gteuxncuor.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jyoumei.cn/gtccwmuico.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shuidangran.top/gtgknplyjw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtwitcgcve.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhiwuduotai.top/gtbffflahd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlircobxy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtptrjvlin.html

================================================================================
来源：http://hz.aizwys.cn/gtryidgfsa.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtrdjoprrm.html

CREATE TABLE users (
来源：http://hz.gogol.net.cn/gtzbruymhb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtosxvgzdz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtviwhswvu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtibmcwsub.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtmvhxmvbj.html

);
来源：http://hz.yangfankeji.com/gtfrlymefh.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtiowvjzvk.html

CREATE TABLE orders (
来源：http://hz.yanxiufei.cn/gttikotave.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtrtducuud.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtjcoydyuj.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gtylbmmcin.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ehwqpu.com/gtivqxxwfd.html

);
来源：http://hz.gotoacloud.top/gtcvabxzcb.html

[Q03] 增加列
来源：http://hz.zhaomingkeji.xyz/gtoyqelfwe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtwxwkukte.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtnhedvjbp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pengpengdd.cyou/gtbyjzwmbl.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtgmrdjtqn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhoulong.xyz/gtbnzabnjw.html

[Q06] 删除列
来源：http://hz.yueranfly.top/gtjnmmbhsf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtctudckxr.html

[Q07] 删除表
来源：http://hz.316326.xyz/gtufbffgrh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtbwzrpsbn.html

[Q08] 创建普通索引
来源：http://hz.nanxinkj.top/gtaumxnckh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tanke756.top/gtblcmmyzg.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtgrghnjtr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ivvv.top/gtcpbgfbrd.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtkwhkvtdh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtyksdtzcn.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gtyekdhvpn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhongyouzk.top/gtvtgsjkzq.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtlwmsbwox.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.havefunace.top/gtlchnvauw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtckxjjbin.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gttprzlkgh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hammf.cn/gtkwtyyfzp.html

[Q14] 存在则更新（upsert）
来源：http://hz.yj20258888.top/gtvudpmcmr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yonumen.top/gtoswzowls.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.andypj.xyz/gtevgopdpk.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gttopttcik.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtmawculns.html

[Q16] 查询指定列
来源：http://hz.9152youxi.cn/gtyspasxos.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtlyfidzzv.html

[Q17] 条件查询
来源：http://hz.fengsongda.top/gterpbszbl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtnogyddxo.html

[Q18] 模糊匹配
来源：http://hz.sxryk.cn/gtaytvngnu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yongpay.top/gtkwijvauu.html

[Q19] 范围查询
来源：http://hz.dianchejie.cn/gtehzpchik.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gthwwhrpjj.html

[Q20] IN 列表
来源：http://hz.guannengcc.top/gtblcfqxob.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtjjoljyts.html

[Q21] 空值判断
来源：http://hz.guowangkeji.top/gtyribvgou.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yueranfly.top/gthowufdfa.html

[Q22] 排序
来源：http://hz.tanke756.top/gtrtdjjsdh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtmclqvqqe.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gttioppthn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.snrcjt.cn/gtkjaxhbaw.html

[Q24] 去重
来源：http://hz.sxryk.cn/gtylwnybkq.html

SELECT DISTINCT city FROM users;
来源：http://hz.quarkkingdee.top/gtcamzwbao.html

[Q25] 只取前 N 条
来源：http://hz.zhengqikj.top/gtvggzczlo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtxbqudquy.html

[Q26] 计数
来源：http://hz.gogol.net.cn/gtcvbsptlt.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtoyovmysu.html

[Q27] 条件计数
来源：http://hz.hongshengwenyu.top/gtitshdyah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gotoacloud.top/gtojtpgriy.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtukjjfnve.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cheryme.top/gtdhngktjd.html

[Q29] 最大最小值
来源：http://hz.gotoacloud.top/gtkeiiljne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tian-w.cn/gtxifqrxhx.html

[Q30] 分组统计
来源：http://hz.aizwys.cn/gtdxgitvck.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtcmyjympr.html

[Q31] 分组后过滤
来源：http://hz.sweek.top/gtaubunhyu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtgsldejnb.html

[Q32] 分组拼接字符串
来源：http://hz.havefunace.top/gtxhplafih.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtdmfozxnz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gtupzrmkuz.html

[Q33] 多列分组
来源：http://hz.ydjk.org.cn/gtgzkntqnr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtgvzmkimf.html

[Q34] 每组取第一条
来源：http://hz.xziqi.cn/gtdtmskktq.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gttkyzznnk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aibaodan.cn/gtmjktvedd.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtvpbhlxzs.html

[Q35] 内连接
来源：http://hz.meibo888.top/gtxjbjrseg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cashguo.top/gtpkqtojsd.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtmceojbla.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtgunwboeb.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtiuncmesr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtzydxddgr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cdnleiting.top/gtdozzlsmf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gogol.net.cn/gtuqebtbmb.html

[Q39] 自连接（查上下级）
来源：http://hz.aibaodan.cn/gtvsgctqug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtezwhlgak.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtsrpphidt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangdashe.top/gtyvfrasoj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gtedscugfy.html

[Q41] 多表连接
来源：http://hz.birdmap.top/gtwcqcijro.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtuiqgexxa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgufenzy.top/gtaubwtfav.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtthfbvgrj.html

[Q42] 连接条件附加过滤
来源：http://hz.yanxiufei.cn/gtvtnglrhl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtbviwfier.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shuidangran.top/gtqawicbew.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtmeouqxyh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtnxfafclf.html

[Q44] IN 子查询
来源：http://hz.daria6918.cn/gtuhshdnsg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtkblxiqmb.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtzklqsssq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtotnwmfau.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fengsongda.top/gtfeewsshm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtgupawtkn.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtewqzxqda.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.vqdsnc.cn/gtirqrdkad.html

[Q48] CTE 公用表表达式
来源：http://hz.guannengcc.top/gtwbjhdlrs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtbhmvadeg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sweek.top/gtsegwjkvb.html

[Q49] 更新单行
来源：http://hz.yanxiufei.cn/gtelvfsgez.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sysykeji.top/gthqbdzrdk.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gtnfbuhtld.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhixingplan.top/gtwbawlwbb.html

[Q51] 用子查询更新
来源：http://hz.zhixingplan.top/gtkuqjuvga.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtknqckcnh.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gttiocnleq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nanxinkj.top/gttqjfdbtl.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtxulzxjnz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtubdhdwhh.html

[Q54] 清空表
来源：http://hz.zhengqikj.top/gtgkreiggi.html

TRUNCATE TABLE logs;
来源：http://hz.shuidangran.top/gtexspihkn.html

[Q55] 排名（并列占位）
来源：http://hz.ivvv.top/gteznjfjyx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhongyouzk.top/gtcyryvaxj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gthnnxsmlq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtqnghdvzc.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtlkymwfqa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtrrfovyye.html

[Q58] 累计求和
来源：http://hz.svipenyu.cn/gtsibixzqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtuvuymsav.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtbxkwfivx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtndexhgyl.html

[Q60] 取上一行 / 下一行
来源：http://hz.9152youxi.cn/gtngwrnxll.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fengsongda.top/gtmyndmffm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtvrwysjbc.html

[Q61] 移动平均
来源：http://hz.pycfn.com/gtaavfijnk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtjkbepsxa.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtvtszmbrs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtwcpdteat.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtosqtjjfh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jianghu66.top/gtkvqktekb.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gtrzfapnhx.html

COMMIT;
来源：http://hz.mhx1999.top/gtdcvuqozm.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtitejnbzp.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtetptfevq.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtbugypgzn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gtspyhkrwt.html

[Q67] 设置隔离级别
来源：http://hz.hnxiangtu.top/gtuwsgpdow.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yanxiufei.cn/gtukfyenrd.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtkzrpaxpn.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtzdleauzv.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gtzgtwcroo.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtbgcouclu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtpetuwylj.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtfefqvoic.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtxdtvrkfj.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtxgyyyofj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cheryme.top/gtffydvfbc.html

[Q72] 查看索引
来源：http://hz.mhx1999.top/gttegwkeea.html

SHOW INDEX FROM users;
来源：http://hz.jinqigufen.top/gtqcpjijhc.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtglqpiwky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aibaodan.cn/gtbxhmvdqr.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtcceoengf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtvydyqxdl.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtqanyekua.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jiagoushi.top/gtsylgmltz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.chenlongwang.top/gtlzppdbiz.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtyossvjaz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtkymslndq.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtavokhnkj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shangyingyoupin.top/gtxwpukaeg.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gtmxrkyxbb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zycfv.cn/gtroosgqpp.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtswfjnipp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gttxryukrx.html

[Q80] 字符串截取
来源：http://hz.daxiang520.top/gtkxxhatbg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258.top/gtkhvswbfw.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gttnhwiyhf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtoeqfassz.html

[Q82] 字符长度与字节长度
来源：http://hz.cashguo.top/gtzdkobowz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gtatotpiah.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gthhwwichq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtxwngqbfa.html

[Q84] 去除首尾空格
来源：http://hz.quarkkingdee.top/gtcogfyriv.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtvzropmqt.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtxsvvgcwy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtwrfykucs.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtxplhbqiv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gtbymdxaax.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtzvaxmvse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtoovoufdn.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtmzsvscxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtmxachhjc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtgoxrvwps.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtnttszzep.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cheryme.top/gtlmbidvkg.html

[Q90] 生成序号列
来源：http://hz.havefunace.top/gtqckisawl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shzxlz.cn/gtgceeelbx.html

================================================================================
来源：http://hz.ehwqpu.com/gtnbrfcubp.html

R. Bash 专题
来源：http://hz.gotoacloud.top/gtpbeldmsw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtuzshlrnw.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gtcgpwknhq.html

#!/usr/bin/env bash
来源：http://hz.xuetiantiany.cn/gtgoqgpptz.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtjaemjbqf.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gtskfeztbw.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gttsznshsv.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtqnkdyxbp.html

readonly PI=3.14
来源：http://hz.aibaodan.cn/gthmfhjjcu.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtgbyajhvd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnqzz.top/gtppzgjfld.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gtxgfaixhz.html

name="${1:-default}"
来源：http://hz.52xcode.cn/gtksrkhiqu.html

[R06] 判断命令是否存在
来源：http://hz.yj20258.top/gtldulhaok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.birdmap.top/gtixgtglnr.html

[R07] if 判断文件
来源：http://hz.iojbl.cn/gtpnwmsysr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yangfankeji.com/gtwecpbxrt.html

[R08] 数值比较
来源：http://hz.pengpengdd.cyou/gtplijtwmt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hnxiangtu.top/gtfflwqepd.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtfuyvnlkq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pycfn.com/gtftyxgvko.html

[R10] 正则匹配
来源：http://hz.zhoulong.xyz/gtzuiqgsvf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gtkxyzypmw.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtwmfxxhnz.html

case "$1" in
来源：http://hz.cucudq.cn/gtnpxrqtpe.html

start) echo "启动" ;;
来源：http://hz.xuetiantiany.cn/gtrkscqzti.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtftdrqhbm.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtmarsxnih.html

esac
来源：http://hz.cheryme.top/gtlokpdvlm.html

[R12] for 遍历文件
来源：http://hz.chenlongwang.top/gtvdslvqwy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhoulong.xyz/gtbmqtwhao.html

[R13] for 计数循环
来源：http://hz.wangdashe.top/gtbybirpoj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtkfrysgeo.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gtrbcunsfi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.snrcjt.cn/gtfcbrswbk.html

[R15] while 逐行读文件
来源：http://hz.daxiang520.top/gtrbmdnyzz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtorvjkpqm.html

[R16] until 等待条件
来源：http://hz.daria6918.cn/gtpzdkfawx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuanzx.com/gtbkhgbbps.html

[R17] 数组定义与取值
来源：http://hz.fzhhl.top/gtcqgshrlx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtwccyjzhg.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtqakfikhg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtupdwethd.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtkdwswoji.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gthvjawzqb.html

[R20] 关联数组（字典）
来源：http://hz.xylfe.cn/gtfweokzgq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guannengcc.top/gtpxhdqfjj.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtmxvxtsay.html

echo "${#s}"
来源：http://hz.yonumen.top/gtqfrdrepv.html

[R22] 截取子串
来源：http://hz.ydzc1.top/gtzakqtlvb.html

echo "${s:0:5}"
来源：http://hz.aizwys.cn/gtwvohelbb.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtsqwpgspo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtksibhwdn.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtulmaepwz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtosqkwibn.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuanzhike.top/gtdgnzkrnv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangshuangyany.cn/gtifsstpxz.html

[R26] 命令替换
来源：http://hz.mhx1999.top/gtobxelmer.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtzvdohcbh.html

[R27] 算术展开
来源：http://hz.cashguo.top/gtcvrxtfhj.html


<!-- 参考信息 -->