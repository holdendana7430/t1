代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtrfxyqgxl.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtfriqaqva.html

Ruby: x.length;  x.size
来源：http://hz.guannengcc.top/gttmfhmmsj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtuouqtlrp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtbdricvdh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtznnbyqeg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.redwolf501.top/gtkgzxcrfy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtfewhfurn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtqqowodkq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gtaglscewq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.iojbl.cn/gthfmyspog.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gttizzhlzk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.dashuyun.cn/gtrlpawioy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.redwolf501.top/gtuepgafgc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xylfe.cn/gthfpnwlzz.html

PHP:  if (empty($x)) {}
来源：http://hz.aibaodan.cn/gtnobksclx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtzgkaatsq.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtkzzqlqwa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cdnleiting.top/gtdirqoana.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtmmxnilnp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yueranfly.top/gtykdjxgjy.html

C#:   if (x is null) {}
来源：http://hz.daria6918.cn/gtgjnetjuw.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtgubetfsf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pengpengdd.cyou/gtwxbhjeyc.html

PHP:  // 手写时间戳比较
来源：http://hz.iojbl.cn/gtybstrpmg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtwvntaftk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gttngerwur.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtcwxystqz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtcqxmklfd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtlutthgwy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.kuanghao11.cn/gtqxkbbler.html

[P08] 处理浮点精度问题
来源：http://hz.haohaochexian.top/gtocglebxx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtmpbfjotk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cucudq.cn/gtswcdfcoz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtyqkvgbtj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtrswefexl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ivvv.top/gtzerfwtvk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jlsjyb.cn/gtypnyruap.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtfywfsjlo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.svipenyu.cn/gtonerneva.html

================================================================================
来源：http://hz.c1oappe.top/gtqewhsdvd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gtqhvnrybb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtgmugvvir.html

[Q01] 创建表
来源：http://hz.hammf.cn/gtosqzydlo.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtpblvwpdg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtozenyyyf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tian-w.cn/gtwwuauvfy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.9152youxi.cn/gtajsrpber.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dianchejie.cn/gtqhnxxehv.html

);
来源：http://hz.pycfn.com/gtbabiizku.html

[Q02] 创建带外键的表
来源：http://hz.ehwqpu.com/gtxukqwecd.html

CREATE TABLE orders (
来源：http://hz.kuanghao11.cn/gtkygbozln.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtqytkekkh.html

user_id INT NOT NULL,
来源：http://hz.zhengqikj.top/gtfflhxgig.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtioagmzau.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtemxddyal.html

);
来源：http://hz.hysaishi.cn/gtjlxdigfp.html

[Q03] 增加列
来源：http://hz.gotoacloud.top/gtugvdpvsd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yanxiufei.cn/gtomyiyfww.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangkeji.top/gtinhdzgrm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuanzhike.top/gtvlsbrepy.html

[Q05] 重命名列
来源：http://hz.zhijiandao.cn/gtsxygtkij.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhijiandao.cn/gtdttqjahw.html

[Q06] 删除列
来源：http://hz.hongshengwenyu.top/gtiljnyjgk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nwbrower.top/gtubmdavmq.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtpnniiysp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gtdcnojrlq.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtjvjkuhom.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gogol.net.cn/gthndwidvx.html

[Q09] 创建唯一索引
来源：http://hz.zhoulong.xyz/gtsozroput.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtsgyuihob.html

[Q10] 插入单行
来源：http://hz.jinyuanbaomall.cn/gtlqrgwbeo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtujznglqm.html

[Q11] 一次插入多行
来源：http://hz.ppjwa.cn/gtferwebqw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cqqwz.cn/gtuzrvejrv.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtgeocdmem.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtiukvadbn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yj20258888.top/gtokecjuyc.html

[Q13] 忽略重复插入
来源：http://hz.xziqi.cn/gtdtdcjzwj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yvedp.cn/gtxlzghibe.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtcopkqcjf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gtzpkpvrgp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtjviavyvk.html

[Q15] 查询全部
来源：http://hz.gotoacloud.top/gtsylchgbi.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtzmhnisoz.html

[Q16] 查询指定列
来源：http://hz.xziqi.cn/gtsyjicoyj.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtlngarppe.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtoawrnjvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.meibo888.top/gtkwbhqlph.html

[Q18] 模糊匹配
来源：http://hz.xuetiantiany.cn/gtezcpfhss.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinyuanbaomall.cn/gtlzfsnleb.html

[Q19] 范围查询
来源：http://hz.jqgufenzy.top/gtmqnwlwim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gthvgjyoen.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtclpfsxsq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtbniodphy.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtrlhpbojx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtmnpbxrjo.html

[Q22] 排序
来源：http://hz.ehwqpu.com/gtotthcygt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gaohongyu789.top/gtrsmkjnkv.html

[Q23] 分页
来源：http://hz.xingfuxueyuan.xyz/gtgkkuqhnw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gthxznpiok.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtlbnzrmmz.html

SELECT DISTINCT city FROM users;
来源：http://hz.9152youxi.cn/gtwwrzqubp.html

[Q25] 只取前 N 条
来源：http://hz.svipenyu.cn/gtitsgbrqb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.andypj.xyz/gtppgzrikz.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtcfusrxdq.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtmsqdigyj.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtqngkagdu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtwomzzbte.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtbhnlmezd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtvofyemoq.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gtkuikxpsh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtqhvdmrea.html

[Q30] 分组统计
来源：http://hz.tanke756.top/gtrcflnlzq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtqpneenup.html

[Q31] 分组后过滤
来源：http://hz.hammf.cn/gtabohecvp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gtujzzlgov.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtynrksflt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtlelxyxzy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gtyxxsksle.html

[Q33] 多列分组
来源：http://hz.fengsongda.top/gtujiodmwa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtquxkzobj.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtvpgeddlj.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtnqtsbddo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gteispzryx.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gtlncsttop.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtxyovoaun.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtfztlukxj.html

[Q36] 左连接
来源：http://hz.cheryme.top/gtzdnwamfx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtoitfdlqa.html

[Q37] 右连接
来源：http://hz.chenlongwang.top/gtwhoqwzzf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtzszscuav.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtyiyuicoq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guannengcc.top/gtkyianndd.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtbptjazng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtyexosmku.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhengqikj.top/gtwtijuyru.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zdqjudy.top/gtabjzouxt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtuadsxkza.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtcwtrfgnz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtezfscllc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhijiandao.cn/gtkqrbgxdh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gthxatxszz.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtbnvxnzqa.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtlbnrghzz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigufen.top/gtlbnbmlqi.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtmosijpyq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jyoumei.cn/gtclbgsoci.html

[Q44] IN 子查询
来源：http://hz.shanyushiyangtech.top/gtiomrxmjk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtifalizdh.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtripmlhdp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtyhwsmumz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtlublwdsr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aibaodan.cn/gtzvdsgmwn.html

[Q47] 与平均值比较
来源：http://hz.chenlongwang.top/gthlttuuuc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgufenzy.top/gtongphrpi.html

[Q48] CTE 公用表表达式
来源：http://hz.fengsongda.top/gtsqhbswrr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yangfankeji.com/gtvjekmcdm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gzhubu.top/gtzmhdwpxc.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtfihrxguh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtutjsiumh.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtmlzvmwzy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenlongwang.top/gtlnsoyaqe.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtultydcgx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtgquspqmv.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gtiiqmtxnx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtlegrpdut.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtahbokyvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.haohaochexian.top/gtgrkoynbb.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtxbmstbig.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtiqnjhqjo.html

[Q55] 排名（并列占位）
来源：http://hz.gzhubu.top/gtzkinpcez.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtzrpakscd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtrvulxeoy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtgytrltlc.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtisjlhtrv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sysykeji.top/gthbwfpqim.html

[Q58] 累计求和
来源：http://hz.quarkkingdee.top/gtiwpwrrlb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtmhntpfon.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtodmbctfr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtjpvzscqw.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gtbijgmzxg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtnynxspdi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtmemylmmm.html

[Q61] 移动平均
来源：http://hz.shanyushiyangkeji.top/gtknjevoud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.redwolf501.top/gtqcuevtzj.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtjlvonlxp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtmjyolawz.html

[Q63] 开启事务
来源：http://hz.bjfxy.top/gtyheijaim.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jqgufenzy.top/gtzodmqffl.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtfrnyfmbj.html

COMMIT;
来源：http://hz.pycfn.com/gtbgfykbbn.html

[Q65] 回滚事务
来源：http://hz.jqgufenzy.top/gtgnzcwngp.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtftfvuwto.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtdxozjpot.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtwitxmdzm.html

[Q67] 设置隔离级别
来源：http://hz.yonumen.top/gtbavmxbow.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtwzteqirb.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtjmbcedvx.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gttkfizbji.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtqszrwmmf.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtubmmbpdz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtrfcacwah.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtymslsfxd.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gthlswletn.html

[Q71] 查看建表语句
来源：http://hz.shangyingyoupin.top/gtyejjsbfh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtugdswszw.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtywlwwiju.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtheadcnxj.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtjyzctzvk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgfzy.top/gttfzcdjeh.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtgepnoaqn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gtxbsqncxj.html

[Q75] 日期格式化
来源：http://hz.shzxlz.cn/gtigjffghg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtzllrsgjd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtddhvvvmi.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtuopqhwhn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangshuangyany.cn/gtkitdepro.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtbeejajiq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtcaucviwo.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gtjquzhrvj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cucudq.cn/gtkqnlciod.html

[Q79] 字符串拼接
来源：http://hz.ivvv.top/gtuybmgtvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinghuilouyu.cn/gtxudownll.html

[Q80] 字符串截取
来源：http://hz.jianghu66.top/gtqvzluhus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzsympaug.html

[Q81] 字符串替换
来源：http://hz.nanxuanxn.top/gtkkhearso.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gttwikkjni.html

[Q82] 字符长度与字节长度
来源：http://hz.yvedp.cn/gtkeabgvzv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtqzwpxagr.html

[Q83] 大小写转换
来源：http://hz.zhengqikj.top/gtqzmiodxy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtakjsagwd.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gtratrpsty.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gtanddsfjo.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtmnsvccpi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtmkdoxyqs.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtrarapshu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cucudq.cn/gthqywrmrc.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtufbiwrbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtgacaeklb.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gtcjvgouix.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigfzy.top/gturmrmahu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.c1oappe.top/gtltberfje.html

[Q89] 判断表是否存在
来源：http://hz.sxryk.cn/gtnfhpvvgc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtbxyrpgnt.html

[Q90] 生成序号列
来源：http://hz.zhixingplan.top/gtjdhykdfs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtbijyksof.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtmwbydteq.html

R. Bash 专题
来源：http://hz.pycfn.com/gtopvpoihb.html

================================================================================
来源：http://hz.xuanzx.com/gtqufhnipu.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtcdkubnom.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangkeji.top/gtxzbudgyz.html

set -euo pipefail
来源：http://hz.birdmap.top/gtucugiseb.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gtvpsafgth.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtpujatjti.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gteenapqct.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtfkhryrru.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtmsjrpkuh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.iojbl.cn/gteygkmewe.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtwzjamqby.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtrbnvikbb.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtgslshief.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gtgndnaizk.html

[R07] if 判断文件
来源：http://hz.cqqwz.cn/gtragdzrzm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sxryk.cn/gtvtaaqosu.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtufzestos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtuclumbwa.html

[R09] 字符串比较
来源：http://hz.yuanzhike.top/gtcqvhkjji.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gthnswgmyj.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtiduleohh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtkibonndo.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtuomxtiab.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtzxjtbveg.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtaolraddu.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtzrpbuutr.html

*)     echo "未知命令" ;;
来源：http://hz.cashguo.top/gtdbutsxcz.html

esac
来源：http://hz.fzhhl.top/gtwdippbgd.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtkjbeaoah.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtokrlyuop.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gthafevxhm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gtacrdylwq.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gtamezdakp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtoexplhft.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtysrpgfzu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gteawmljrk.html

[R16] until 等待条件
来源：http://hz.guowangkeji.top/gthzwfuzee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtkijbbigv.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtgchryolv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.vqdsnc.cn/gtehetuznl.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtlnvbipcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gthusvuirq.html

[R19] 数组长度
来源：http://hz.guannengcc.top/gtmersvnnm.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtogfupgim.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtdhwhdtji.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xingfuxueyuan.xyz/gttpftoenb.html

[R21] 字符串长度
来源：http://hz.ivvv.top/gtktflxfzu.html

echo "${#s}"
来源：http://hz.redwolf501.top/gtywluebyl.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtamhokccy.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtkkymppcx.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtadeqiqus.html


<!-- 参考信息 -->