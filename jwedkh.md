代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hnqzz.top/gtjqvsugyu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtdejcszmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtrkoopqfe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtqhqepdnq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtmmkxihet.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtwedbnkpr.html

Ruby: x.length;  x.size
来源：http://hz.gzhubu.top/gtylbblemd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.mhx1999.top/gtylmfxcuf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangkeji.top/gtybyjvual.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtskohqbqf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guowangkeji.top/gtfmuwebqv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtkeaztppt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shzxlz.cn/gtkufzpptw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtwilxvfrf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.birdmap.top/gtabzuwxuv.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gtcbbiolgz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gttfnrijei.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhijiandao.cn/gtzypsyvlg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnxiangtu.top/gttekvdnbl.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gthzyectcg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtkgdvdtny.html

TS:   if (x == null) {}
来源：http://hz.316326.xyz/gtjrawvzed.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtmeniztbz.html

Go:   if x == nil {}
来源：http://hz.ywan-chungtsiang.top/gtxfngcnhj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.snrcjt.cn/gtguxicvaa.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtwknfcurg.html

[P07] 防抖与节流
来源：http://hz.zhixingplan.top/gtzpdmutys.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtidayxurf.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtwhtssxbg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gthqktlhmo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtuffzpxys.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dianchejie.cn/gtlygijeec.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shuidangran.top/gtdpirugnn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gtxvsooobn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtbbjmxcrw.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtxkwckztz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.birdmap.top/gtdpgsrhes.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuetiantiany.cn/gtekaqqimf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gtadwccoys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuxming.cn/gtnqttgexd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtjozhrarb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xziqi.cn/gtunbkdgvs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtdyeoranh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtajnoghpr.html

================================================================================
来源：http://hz.yvedp.cn/gtvcbttjwv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnxiangtu.top/gthszxhrpi.html

================================================================================
来源：http://hz.yvedp.cn/gtfvjmxtzt.html

[Q01] 创建表
来源：http://hz.yj20258.top/gtuyclbivo.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtunrbveys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtlroxclhb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtmpdkbkce.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenzaomai.com/gteqmcaaij.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtagscdfxd.html

);
来源：http://hz.yj202588.top/gtfqqmvfsf.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtoxuzzksl.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gthdtgihrp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtjuokkeps.html

user_id INT NOT NULL,
来源：http://hz.316326.xyz/gtihmpjnit.html

amount DECIMAL(10, 2),
来源：http://hz.dianchejie.cn/gtgixtlqqp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shangyingyoupin.top/gtmxzuzytx.html

);
来源：http://hz.jlsjyb.cn/gtvmvjggtu.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtfloqgvzo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gaohongyu789.top/gtuhxuklij.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtfqweztob.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgfzy.top/gtvozjjjld.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gttpwopelv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtfeuienwk.html

[Q06] 删除列
来源：http://hz.sxryk.cn/gtqjkxgtdk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jianghu66.top/gtdubttdfs.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtwevxjtlz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtjsfncrat.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtufxrgzqj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nwbrower.top/gtezglbhmg.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gthkwlfmnw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtgzlmdoda.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtbypznibf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yangfankeji.com/gtczgktkan.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtnjzrbfuo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuanzx.com/gtxouyakdi.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gtbiailkju.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtytdzimoe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.bjfxy.top/gtvwuwfmoz.html

[Q13] 忽略重复插入
来源：http://hz.zycfv.cn/gtubtomwna.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtjaebshrn.html

[Q14] 存在则更新（upsert）
来源：http://hz.hfpthk.cn/gtylvgjzld.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gtlvzecclu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinyuanbaomall.cn/gtqhtfwash.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtieckxikw.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtkejhyovw.html

[Q16] 查询指定列
来源：http://hz.dashuyun.cn/gtwdntqvfs.html

SELECT id, name FROM users;
来源：http://hz.ivvv.top/gtdihxaqpe.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtdyidrpqe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tianlin.xyz/gtjwlcwodi.html

[Q18] 模糊匹配
来源：http://hz.jinqigufen.top/gtyerzheum.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigfzy.top/gtdysnyftk.html

[Q19] 范围查询
来源：http://hz.jinqigfzy.top/gtlrpceeuu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtltcbcbwk.html

[Q20] IN 列表
来源：http://hz.9152youxi.cn/gtmeqbsxzy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gthrrgqldd.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtrqibkrna.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gteorgqzmh.html

[Q22] 排序
来源：http://hz.shanyushiyangtech.top/gtmxbaonrz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtazfydsdf.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtlcrceici.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtzfthyvmn.html

[Q24] 去重
来源：http://hz.jqgufenzy.top/gtinsxbdim.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtkrypghpo.html

[Q25] 只取前 N 条
来源：http://hz.9152youxi.cn/gtfebmkffc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtacyjolqh.html

[Q26] 计数
来源：http://hz.yonumen.top/gtndjheazk.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gtmbpaaplm.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtayvwjrvf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtxqgvlieq.html

[Q28] 求和与平均
来源：http://hz.daria6918.cn/gtmbbdrzie.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.kuanghao11.cn/gtkkggcnlr.html

[Q29] 最大最小值
来源：http://hz.guowangkeji.top/gtgwestzmt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtkxecyarl.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtcjnxsscr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtgfhcfhvx.html

[Q31] 分组后过滤
来源：http://hz.sufxvd.cn/gtrcnhiqee.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtmnpktmde.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtbvlryjwq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtjbbqzqlu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dashuyun.cn/gtdavxsdjr.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtipnontwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtthpsnfcr.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtvakuwcsy.html

SELECT * FROM (
来源：http://hz.fzhhl.top/gtqzqbxaci.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtezqkhdah.html

) t WHERE rn = 1;
来源：http://hz.zhengqikj.top/gtpybvumsv.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gtmgirtnzf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtafeurtda.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtjyzrkstj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtwninxazs.html

[Q37] 右连接
来源：http://hz.dashuyun.cn/gttzuupvze.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jyoumei.cn/gtlkmdvveo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hongshengwenyu.top/gtazhholcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtqzdozuyd.html

[Q39] 自连接（查上下级）
来源：http://hz.xuetiantiany.cn/gtheeumzyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daria6918.cn/gtychxiqpe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.dianchejie.cn/gtjxblykll.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtxmpcvmxf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gthjwzsxdu.html

[Q41] 多表连接
来源：http://hz.52xcode.cn/gtptjclsnf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dashuyun.cn/gthcxdlvjs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xziqi.cn/gtrkmmlioq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guannengcc.top/gtdhyjfdmf.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtnswruvdi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtbbcvzblt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gtbocbpnjy.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtorwwtehc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtfndxwfmj.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtcebbverx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtdugkeomi.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtqdnlnfha.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guowangkeji.top/gtkihinrgl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtrnaiacff.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtxjsjymwa.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtaozhzeax.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hywenlv.cn/gthdydohhh.html

[Q48] CTE 公用表表达式
来源：http://hz.daxiang520.top/gtxbsdfvrq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtzvhmwbtm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtrqvjzrkw.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtkyrdvguw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigfzy.top/gthekshgod.html

[Q50] 批量更新
来源：http://hz.sxryk.cn/gtpzixlion.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gthffvbfvv.html

[Q51] 用子查询更新
来源：http://hz.sufxvd.cn/gtomemiruy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtlslilmes.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtfnfdclso.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gtzqcwjpxc.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtnmgqdvyk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tian-w.cn/gtohiawvit.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtlcerheoq.html

TRUNCATE TABLE logs;
来源：http://hz.c1oappe.top/gtricbqfug.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtmnkumnyk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtfrfltgtv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gtpuwqyfpd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xuetiantiany.cn/gtsjsdzdbm.html

[Q57] 行号
来源：http://hz.ydjk.org.cn/gtpflcvbzh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtkwhyyobx.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtyqgzusdb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gzhubu.top/gtcfdvfxeh.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtpslrpenc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgufenzy.top/gtwikrjdjy.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenlongwang.top/gtbaceoicq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtueytagsj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gtahbddtdn.html

[Q61] 移动平均
来源：http://hz.xuanzx.com/gtbwtlrfto.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtunjbtqjk.html

[Q62] 分组占比
来源：http://hz.hysaishi.cn/gtaidfhijf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtsqjfzayn.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtdsdhqzwz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtrgicznyn.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtbiflqtdv.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtdecoppgc.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtfrqlbrvn.html

ROLLBACK;
来源：http://hz.yvedp.cn/gtmkforaap.html

[Q66] 行锁查询
来源：http://hz.chenlongwang.top/gtwcwfmksm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtopxdagmk.html

[Q67] 设置隔离级别
来源：http://hz.xinyue.icu/gtrqmofama.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dianchejie.cn/gtlznnncgw.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gtlnbnmmim.html

SAVEPOINT sp1;
来源：http://hz.chenlongwang.top/gtljovnidg.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtexadcnli.html

[Q69] 查看执行计划
来源：http://hz.tianlin.xyz/gtdqagefka.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtgfcgfmqo.html

[Q70] 更新统计信息
来源：http://hz.svipenyu.cn/gtmuimpqtf.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtzovrlzrd.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtegtbmhvl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sysykeji.top/gtuyswtddy.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtomabsisy.html

SHOW INDEX FROM users;
来源：http://hz.yongpay.top/gtxrqusyhc.html

[Q73] 查看表状态
来源：http://hz.shuidangran.top/gtbuzagwvo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gtksrvfktn.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtkiabyksv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gtdtumrzoi.html

[Q75] 日期格式化
来源：http://hz.gotoacloud.top/gtixrrvqdv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtcpismhdg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtrupdniay.html

[Q76] 按天统计
来源：http://hz.iojbl.cn/gtwybjmxzk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.52xcode.cn/gtimaunhrq.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtojmurrzp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtosjfdctk.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gtkszcrece.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hammf.cn/gtjyljoyjv.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gtrwxdtaya.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tian-w.cn/gtsuowaeot.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gthzbxpucz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtiqiplzbb.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtvsnwzgkk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guowangkeji.top/gtsktimtsy.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtuzsvoyev.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtovskwfyu.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtpmztjcsh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.havefunace.top/gtgtpagryi.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtgfrpnahk.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtmbmeajix.html

[Q85] 数值取整
来源：http://hz.shuidangran.top/gtwtygbqhv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtbrmwojtp.html

[Q86] 读取 JSON 字段
来源：http://hz.svipenyu.cn/gtbieuchhj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuanzx.com/gtmhoyaoeg.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtylpwwodi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtavrwhcsf.html

[Q88] 行转列（条件聚合）
来源：http://hz.gogol.net.cn/gtqwyetpnl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gthacggypp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtlcyszpyj.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtfxeldptd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhoulong.xyz/gttinyxepy.html

[Q90] 生成序号列
来源：http://hz.xingfuxueyuan.xyz/gthhehhrme.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nwbrower.top/gtfkipybwt.html

================================================================================
来源：http://hz.0kj1m.cn/gtxwixzsmi.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtjgbwefsy.html

================================================================================
来源：http://hz.cashguo.top/gtfkceluas.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gtndsfsqzy.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtrutscare.html

set -euo pipefail
来源：http://hz.yonumen.top/gtsaohvnzq.html

[R02] 变量赋值与使用
来源：http://hz.fengsongda.top/gtljysheeo.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gtwuudgbgr.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtvhnvpwaj.html

readonly PI=3.14
来源：http://hz.fzhhl.top/gtmbculcii.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtfwgurlkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtiipmbmfs.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtvnldqevx.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtglqtrkzt.html

[R06] 判断命令是否存在
来源：http://hz.guannengcc.top/gtuejaorlj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtjdckrbmo.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gteiuktmuv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtzssqwavz.html

[R08] 数值比较
来源：http://hz.hammf.cn/gtrfbmqkqc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pycfn.com/gtsruhyjby.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtdimgwdwv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj202588.top/gtmsrsvfjo.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtwffrfsvk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtqpiiuhma.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtcrarmtiv.html

case "$1" in
来源：http://hz.yvedp.cn/gtqecnjnvn.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtidsdnrgh.html

stop)  echo "停止" ;;
来源：http://hz.yanxiufei.cn/gtunddkpqo.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtfkyykhfx.html

esac
来源：http://hz.cucudq.cn/gtrzphaeri.html

[R12] for 遍历文件
来源：http://hz.tianlin.xyz/gtktpxjxrw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtczkenvzg.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtvyttwkyw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtorrrzfxz.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtwghekkes.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtcudqfcyr.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gthaljlsaz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.quarkkingdee.top/gtiqhsuazz.html

[R16] until 等待条件
来源：http://hz.andypj.xyz/gtqhpuvnsa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gttycvnnnm.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtmtjtxuzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtxctfnlie.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtkhdykitv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtgktyupjr.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtapyvyjvp.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gttqaweybf.html

[R20] 关联数组（字典）
来源：http://hz.nanxuanxn.top/gtzepwbcob.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gteohawfac.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtiuggsyfq.html


<!-- 参考信息 -->