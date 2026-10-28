代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtvcsvkoef.html

Go:   len(arr);  len(m)
来源：http://hz.chenzaomai.com/gtdmtdgkyu.html

Ruby: x.length;  x.size
来源：http://hz.ybcxt.top/gtgktebzlz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hywenlv.cn/gtaqzcegzq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.birdmap.top/gtewqaqoap.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gaohongyu789.top/gthwtswzdy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ehwqpu.com/gtkbvbctel.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtywwiyiia.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtadqgwlsv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtumoatork.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtzqkyzdeb.html

Ruby: a == b
来源：http://hz.chenjidiqi.icu/gtxxqfmhur.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtdlwdzxko.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jianghu66.top/gtqtulhkpf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gtzcuioxba.html

PHP:  if (empty($x)) {}
来源：http://hz.gotoacloud.top/gtgcumyqzd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtlxkyjvja.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtiacijdae.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gtfcpcskbf.html

Go:   if x == nil {}
来源：http://hz.dashuyun.cn/gtgylisisx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtotkfcmaq.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtfnisrbsk.html

[P07] 防抖与节流
来源：http://hz.svipenyu.cn/gtsprlrltd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ywan-chungtsiang.top/gtiljqrlhg.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgufenzy.top/gtemexdygl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtwmudfjww.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtjnjrmqrn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guowangkeji.top/gtzmdplkma.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.birdmap.top/gtbpplymmj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtyukxbcnp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gtvpdwfhfi.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gtzdndqtns.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtosqzohvq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sxryk.cn/gtiuuindst.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtvgezvxvv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtucopshvu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtwztkvtmi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtrwhzrife.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ybcxt.top/gtaegzxkva.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtrizwprdi.html

================================================================================
来源：http://hz.yangfankeji.com/gtnogqxrph.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gtioqruxoz.html

================================================================================
来源：http://hz.ybcxt.top/gtjlbbwikc.html

[Q01] 创建表
来源：http://hz.jinqigufen.top/gthgpcugbe.html

CREATE TABLE users (
来源：http://hz.aizwys.cn/gtmqpqqvox.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtylwrpwrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pengpengdd.cyou/gtjkkuhiqp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtybcvvvjb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhengqikj.top/gtkznynokb.html

);
来源：http://hz.iojbl.cn/gtpewuszqr.html

[Q02] 创建带外键的表
来源：http://hz.tian-w.cn/gtcjydfhcx.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtteeqssbu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtshthyofn.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtponovghl.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtfkycrctl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtjbjrsuag.html

);
来源：http://hz.mhx1999.top/gtsyqvyadv.html

[Q03] 增加列
来源：http://hz.guowangkeji.top/gtiocuujie.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtakdbcfro.html

[Q04] 修改列类型
来源：http://hz.hywenlv.cn/gtfjdlmtdx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtjahtkjoi.html

[Q05] 重命名列
来源：http://hz.52xcode.cn/gtbdqwhywd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zycfv.cn/gtaiziggfh.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtdhratham.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gteyuauuag.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtnkxcjvvb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtutnxjcqr.html

[Q08] 创建普通索引
来源：http://hz.nanxuanxn.top/gtzipksfri.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtszeagifo.html

[Q09] 创建唯一索引
来源：http://hz.daria6918.cn/gtsjhuwjlj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtcjzqjgxr.html

[Q10] 插入单行
来源：http://hz.sysykeji.top/gtwjofeweb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtifjblnae.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gttzwiptst.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgfzy.top/gtgxngurur.html

[Q12] 插入后取自增 ID
来源：http://hz.zhixingplan.top/gtrrcwlpzh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtyqgtsyaj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ivvv.top/gtqmrkcabt.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtczqspmpf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtgivzwlfw.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtilhcgjgr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cqqwz.cn/gtvuhipgbz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtfcnotmwt.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtdfmfverg.html

SELECT * FROM users;
来源：http://hz.aibaodan.cn/gtgabyamdu.html

[Q16] 查询指定列
来源：http://hz.chenjidiqi.icu/gtbpiqnoum.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtaogsirob.html

[Q17] 条件查询
来源：http://hz.redwolf501.top/gtcbrnyfmn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nwbrower.top/gtuihpmjnb.html

[Q18] 模糊匹配
来源：http://hz.bjfxy.top/gteugqcbvr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtdvfkoxna.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtzpcytsrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.feifeiyinyue.top/gtlwzcpphl.html

[Q20] IN 列表
来源：http://hz.xinyue.icu/gtmjvxgcab.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gtxgzijtqi.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gthalwdhnw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.daria6918.cn/gttyvyppnp.html

[Q22] 排序
来源：http://hz.bjfxy.top/gtbjxzukub.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtwtrjhzvc.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtigoxzffz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sweek.top/gtbdwyfpon.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtbfwozyfl.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtbkvsvaer.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtuzplevcd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtxuonrhkr.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtooensrqd.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gtlckoxono.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtwwqgicea.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.iojbl.cn/gthgcioblz.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtkdoztqim.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sufxvd.cn/gtyzrxnalg.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtoxmbukvk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gzhubu.top/gteecobqeo.html

[Q30] 分组统计
来源：http://hz.yongpay.top/gtnikvtbat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtpfsfyolz.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtmiylpyda.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shuidangran.top/gtfffioqis.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gtcvwwnwkg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtsmzlwsoj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtnviznpan.html

[Q33] 多列分组
来源：http://hz.fzhhl.top/gtqmtrlnds.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pengpengdd.cyou/gttpmahlyn.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gteqshrpih.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtvdxnphlw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtdohyzraa.html

) t WHERE rn = 1;
来源：http://hz.xingfuxueyuan.xyz/gtuumyubye.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtxenmoqve.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtanatczkg.html

[Q36] 左连接
来源：http://hz.tian-w.cn/gtdhnzziaa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtgnldjrjz.html

[Q37] 右连接
来源：http://hz.tanke756.top/gteaqjhqye.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gtjfhoxgic.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtfluykvxr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gotoacloud.top/gtpycbvvzw.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtefvjgxdb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtvdpoigzl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhaomingkeji.xyz/gtblwxcnsn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtyqxkadmz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtatwgrwin.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtjepdrmaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtiecuqnyx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sufxvd.cn/gtcnltjvwu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jyoumei.cn/gtgpeogvpy.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtbinptthf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtzjowekfk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.mhx1999.top/gtwewrgguj.html

[Q43] 标量子查询
来源：http://hz.dianchejie.cn/gttzyalzmp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtbqwwzxnt.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtwdmeevwz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.iojbl.cn/gtesupfsgl.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtlcpincxu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtntzzauel.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tianlin.xyz/gtnjrnvjbv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gthtqiujjy.html

[Q47] 与平均值比较
来源：http://hz.zhaomingkeji.xyz/gtfefdvsqk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtnnccmaog.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtbmgnifld.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtlzqfzuja.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtrjbjwmnl.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtqrhsxfnb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtgxudbnki.html

[Q50] 批量更新
来源：http://hz.birdmap.top/gtywnwbobv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtwvhxzitd.html

[Q51] 用子查询更新
来源：http://hz.hnxiangtu.top/gtkzuxajgl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gthgpzqwlq.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gterhumgdf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtzilcmbpe.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtlfinnmjp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtaqksxneg.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtpdtosmbb.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gtfqgqgmxq.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258.top/gtdaunxoza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtsreqpybh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gtqndemdhb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtigzlstvz.html

[Q57] 行号
来源：http://hz.chenzaomai.com/gtzjmdbtld.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xylfe.cn/gtkbdezdti.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtjygctzdm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gthjxgbiwa.html

[Q59] 分组内累计
来源：http://hz.ydjk.org.cn/gtqzlzvkkh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daria6918.cn/gtaqwuqhkq.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gtsazovuqt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtgmfvvejt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtpevnmrsd.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtzairhira.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtrwlgdbqb.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtwudxqyyh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtddsvssmu.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtzxaxfszr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtgphxmxts.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gtelaezqwv.html

COMMIT;
来源：http://hz.jianghu66.top/gtirkcxphr.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtstepkoaz.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gtadzwttbn.html

[Q66] 行锁查询
来源：http://hz.snrcjt.cn/gtvhgjmxfn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gtwddwtohw.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtnagysyun.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gtwsbsmpcn.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtzlxaolhr.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtaktmdagc.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtbqpmjupm.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtmkxrxetw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuanzhike.top/gtxnhzihoi.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtgvzbnjjg.html

ANALYZE TABLE users;
来源：http://hz.feifeiyinyue.top/gttkgsgcdt.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtetxfzhio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhixingplan.top/gtsgnltzmr.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtzigjihex.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtsdjwljli.html

[Q73] 查看表状态
来源：http://hz.hnqzz.top/gtdmaeyfnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhoulong.xyz/gtakytgjnw.html

[Q74] 强制使用索引
来源：http://hz.cheryme.top/gtshxyedst.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gtpwktllda.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtuidjlfnd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.nanxuanxn.top/gtyqlvkzmt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gtvyxpnrim.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gttbnkbzmn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtmzcbztxn.html

[Q77] 时间加减
来源：http://hz.vqdsnc.cn/gtgsjamqvc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xinyue.icu/gtgogxjdwm.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtrefksdhf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtmbrlfrmn.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtandakkvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtfinmchub.html

[Q80] 字符串截取
来源：http://hz.zhaomingkeji.xyz/gtjdloytvr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gtdyzxlpfj.html

[Q81] 字符串替换
来源：http://hz.dashuyun.cn/gtkjxwudpj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtlbvyzwig.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtneowgajs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtsqphulan.html

[Q83] 大小写转换
来源：http://hz.sxryk.cn/gtuexqdsuy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daxiang520.top/gtteclktqf.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtptkufbpp.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtdvjcccix.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtmwbumlbt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtjgprtkuh.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gtsjgtiary.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.dashuyun.cn/gthndmboqp.html

[Q87] JSON 字段做条件
来源：http://hz.sweek.top/gthojyruji.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtahlikivw.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gtejbapbyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtbbjjoruw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuxming.cn/gtwwpaohmw.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtlfemnnbw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.havefunace.top/gtuwzuhrua.html

[Q90] 生成序号列
来源：http://hz.guannengcc.top/gttonnhoqx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtkmjsnnxh.html

================================================================================
来源：http://hz.yj202588.top/gtdbfaqnqo.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtzhmztjdh.html

================================================================================
来源：http://hz.cdnleiting.top/gtqirgefuq.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtkntdfude.html

#!/usr/bin/env bash
来源：http://hz.xuetiantiany.cn/gtsdzjlsbm.html

set -euo pipefail
来源：http://hz.guowangkeji.top/gtuschifxn.html

[R02] 变量赋值与使用
来源：http://hz.zhaomingkeji.xyz/gtiqbjvapb.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtxqlosccv.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtirvxtjxd.html

readonly PI=3.14
来源：http://hz.tanke756.top/gtsbajnzko.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtlwyvufun.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgfzy.top/gtqwimtnab.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gtzcmuavrk.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtaziwkdgp.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gthqxrvjjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtnmabzigs.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtvvusbufr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtktxlgdsl.html

[R08] 数值比较
来源：http://hz.yuanzhike.top/gtlfxnvzpz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.aizwys.cn/gtivcyqlwc.html

[R09] 字符串比较
来源：http://hz.chenlongwang.top/gtttktndzc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtmiierotu.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtkwaujzvl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtjaezwxce.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtnxoplqil.html

case "$1" in
来源：http://hz.sweek.top/gtdmntyjiq.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtewbbyzmb.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtcnrmgsaw.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtypsfdchx.html

esac
来源：http://hz.haohaochexian.top/gttxhiortt.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gtmaqdkqfi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtapkyjvyq.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtdudukxhb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtqjpwwwso.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtumwtkanw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtcqpsrjyg.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gtcjfvfpqx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtbdsrninc.html

[R16] until 等待条件
来源：http://hz.gogol.net.cn/gtxbzxhvzo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gtdtfgauwn.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtkfkxluie.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtdisubbhn.html

[R18] 遍历数组
来源：http://hz.bjfxy.top/gtraxorzkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtbfqjzbuu.html

[R19] 数组长度
来源：http://hz.smart0.xyz/gtyhidgfvj.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtdaozfxmx.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtyailwomn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258888.top/gtfobuknwz.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtiiornszu.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtvxanoomh.html

[R22] 截取子串
来源：http://hz.jyoumei.cn/gtcsfaqhfb.html

echo "${s:0:5}"
来源：http://hz.yvedp.cn/gtqtwlqqpg.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtukgbbfxj.html


<!-- 参考信息 -->