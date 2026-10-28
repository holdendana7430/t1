代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gtzpducbaa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aibaodan.cn/gthjobcnxr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtkbpxoflz.html

[P04] 求长度
来源：http://hz.ivvv.top/gtztjbdade.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtnqorjvgj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtwkerrvrh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gthsrxzymq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtqmwnvykf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ivvv.top/gtpqfrzkol.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtvatpurek.html

Ruby: x.length;  x.size
来源：http://hz.gzhubu.top/gtxcczdjmy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtfdhdtnno.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtyddzhtjk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gzhubu.top/gtikbpjxde.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuxming.cn/gtnfnwopzi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.iojbl.cn/gtnyqwbpdt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtwcsiozny.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gtemzrqfle.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtyeshvaua.html

Ruby: a == b
来源：http://hz.xuanzx.com/gtxrqgffhh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtlmbgbmni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.snrcjt.cn/gteshfcmdd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtjtxtihrl.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtxclddlev.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtkdpliozv.html

TS:   if (x == null) {}
来源：http://hz.yuxming.cn/gtrcsblyaj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtdubbwemc.html

Go:   if x == nil {}
来源：http://hz.yanxiufei.cn/gtdxcayurq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtmxnwmknf.html

C#:   if (x is null) {}
来源：http://hz.xingfuxueyuan.xyz/gtatyqvkej.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtzklrracd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtkzvxcsop.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtxhmnbvst.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtrsbemxgf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtwkqisudf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtjhxcejxj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxuanxn.top/gtsaqracmc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gthgehqnwn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gogol.net.cn/gtfpemujyh.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtzsgwxqtb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sxryk.cn/gtvbbhyshy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtetmsnmpq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtdpyloxzu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtmruymgmf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtmcgwxdtb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tanke756.top/gtmxiwmwvb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.9152youxi.cn/gtpclxiajt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtvktalvoz.html

================================================================================
来源：http://hz.yj20258888.top/gtksxtozdn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.chenlongwang.top/gtksudskxm.html

================================================================================
来源：http://hz.bjfxy.top/gtdyeycpkl.html

[Q01] 创建表
来源：http://hz.havefunace.top/gtjwtoarxq.html

CREATE TABLE users (
来源：http://hz.shuidangran.top/gtvupkzkrb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangkeji.top/gtpvbkowip.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenzaomai.com/gtrhtzmadz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ivvv.top/gtxqwuxefy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.birdmap.top/gtlujlaowp.html

);
来源：http://hz.tian-w.cn/gttrwvqpje.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gtcbbpjyvh.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtsdphqmyz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtkgidkklk.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtpbgzzlay.html

amount DECIMAL(10, 2),
来源：http://hz.ydjk.org.cn/gtnhzhljrk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtjisbpxxf.html

);
来源：http://hz.gotoacloud.top/gtlaujnofw.html

[Q03] 增加列
来源：http://hz.snrcjt.cn/gtiqreirsq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtajhwxdus.html

[Q04] 修改列类型
来源：http://hz.xylfe.cn/gtgyrjbkdu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhoulong.xyz/gtjpdcspkt.html

[Q05] 重命名列
来源：http://hz.jinghuilouyu.cn/gtmpzvmbzr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nwbrower.top/gtthzapoye.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtcuxwmfah.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtnwnfcyuc.html

[Q07] 删除表
来源：http://hz.ppjwa.cn/gthqxdjnni.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtdwbgrumb.html

[Q08] 创建普通索引
来源：http://hz.hywenlv.cn/gtdudvjbmz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jiagoushi.top/gtskdplnov.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtlwqxbkez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtydzyxgtv.html

[Q10] 插入单行
来源：http://hz.hnxiangtu.top/gtkuogxqix.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gttgtezvws.html

[Q11] 一次插入多行
来源：http://hz.zdqjudy.top/gthbnqbbce.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cqqwz.cn/gtolftbgtw.html

[Q12] 插入后取自增 ID
来源：http://hz.yuxming.cn/gtgjyphhpd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuanzx.com/gtosmnpedi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtmdlemacw.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtzehmtmqr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtynjibayy.html

[Q14] 存在则更新（upsert）
来源：http://hz.yvedp.cn/gtwsnhqcfq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gtzhutljfv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtfiomuqym.html

[Q15] 查询全部
来源：http://hz.zhengqikj.top/gthzvyjack.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtopdcvuoz.html

[Q16] 查询指定列
来源：http://hz.jinghuilouyu.cn/gthcskjniu.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtnggcwhxo.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtzzomoyxp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pengpengdd.cyou/gtxdsvydls.html

[Q18] 模糊匹配
来源：http://hz.tianlin.xyz/gtnjhjqnoe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sysykeji.top/gtyktibxit.html

[Q19] 范围查询
来源：http://hz.tian-w.cn/gtdifzxjim.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cheryme.top/gtsjhrljot.html

[Q20] IN 列表
来源：http://hz.xingfuxueyuan.xyz/gtqnshwkxh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtbgunzjki.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtrtsjjtwi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigfzy.top/gtxbhbsdku.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtoupnlius.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gtwrmciifs.html

[Q23] 分页
来源：http://hz.zhengqikj.top/gtuaimqfnc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gtlfadpqko.html

[Q24] 去重
来源：http://hz.ivvv.top/gtrcknisrj.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtsqpcztbm.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtevwhqnjn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gttbxgdyma.html

[Q26] 计数
来源：http://hz.iojbl.cn/gtbkqvldom.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuetiantiany.cn/gtgezglnve.html

[Q27] 条件计数
来源：http://hz.hysaishi.cn/gtnolcqacr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cqqwz.cn/gtaodltnvn.html

[Q28] 求和与平均
来源：http://hz.iojbl.cn/gtibmgjlwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtksrzlupa.html

[Q29] 最大最小值
来源：http://hz.yj202588.top/gtdoxuqrab.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtsujlmimy.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gttfrymala.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtsxvqhmqz.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtyolahrcf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtkegwmhls.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtijncxoow.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtpgkglyey.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gtftemsrrt.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gtkryzlrey.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtoxnbvkgm.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtsuavxdrt.html

SELECT * FROM (
来源：http://hz.fzhhl.top/gtztdaipvu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtfgpyktks.html

) t WHERE rn = 1;
来源：http://hz.hysaishi.cn/gtaivvvrgi.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtjjixocjm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtbuinwxjh.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtvrijxatq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtixczdpbk.html

[Q37] 右连接
来源：http://hz.jianghu66.top/gtjyskebqs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtoxeondks.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtdxmovvbl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj202588.top/gtcaudmdyp.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtbgfhrjyf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtizdsvpug.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtrgjqvawp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnxiangtu.top/gtftdpmghb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtwucbtmli.html

[Q41] 多表连接
来源：http://hz.yuanzhike.top/gtpidssrff.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gthektrzjq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cucudq.cn/gtbbfjuhrm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtlyvaeits.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtzxtodwsx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtwpirvxbd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gttpnbbfsd.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtciiyzscg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guannengcc.top/gtwmmjvcyc.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtliidmnfj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtxqioxogl.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtutebxbuk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtlrcwcdax.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtmxztbhyt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtzuzslfhw.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtzudzvjrf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gtwnfmefuq.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgufenzy.top/gthsmimrhv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtoczozlhs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtzdusytyl.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtyxdzzusn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuanzhike.top/gtetnrgcvc.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtxipiyzsg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtplbqmped.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtkjfknodd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigfzy.top/gtxxyhsnle.html

[Q52] 删除指定行
来源：http://hz.jiagoushi.top/gtphtetgxk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.bjfxy.top/gtnrzvbvtj.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtxxlkiwvo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtnmwfiqta.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gtoelljywv.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtryyfqcxb.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gtiiaxshbx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtodrecefb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.birdmap.top/gtdcvwdjwp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtkvlvcpum.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtlpyemezj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxuanxn.top/gtqodvkjgz.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtpozokogb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtbcjungto.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gthtiflydd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtcqhepzbr.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangtech.top/gtfkpkrchd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtzfgnvbzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangtech.top/gtfhbvupdh.html

[Q61] 移动平均
来源：http://hz.ybcxt.top/gtkpjyhspa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gtufctzxjv.html

[Q62] 分组占比
来源：http://hz.shanyushiyangkeji.top/gtpjsezwuu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtpseflsog.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gttjodhrpr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtxtfxtvtp.html

[Q64] 提交事务
来源：http://hz.tanke756.top/gtazvpohbd.html

COMMIT;
来源：http://hz.jyoumei.cn/gtzahhtvnd.html

[Q65] 回滚事务
来源：http://hz.redwolf501.top/gtwwordsab.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtskwgfiqn.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtaahaowax.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtwfbhkfbu.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtlggadver.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtipyzibwu.html

[Q68] 保存点
来源：http://hz.ehwqpu.com/gtzfzdiufg.html

SAVEPOINT sp1;
来源：http://hz.zhongyouzk.top/gttpjpoifr.html

ROLLBACK TO sp1;
来源：http://hz.pengpengdd.cyou/gtxukkjbqf.html

[Q69] 查看执行计划
来源：http://hz.tian-w.cn/gtkbmngtst.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shzxlz.cn/gtxcmiqkgg.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtxvzxlore.html

ANALYZE TABLE users;
来源：http://hz.cqqwz.cn/gtlvheglha.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gtxlgpzwrs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cheryme.top/gtgskreflu.html

[Q72] 查看索引
来源：http://hz.hysaishi.cn/gtahlmppli.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtevwhapdb.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtdfttijdh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gthqarmrow.html

[Q74] 强制使用索引
来源：http://hz.snrcjt.cn/gtooeabbgg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dashuyun.cn/gtlvgdntpx.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gthizdpfzq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cucudq.cn/gtlxcavezk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yongpay.top/gttusrabmo.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtrfysjluo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gtpvzrkzyk.html

[Q77] 时间加减
来源：http://hz.mhx1999.top/gtsgixqroq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtpwmakkms.html

[Q78] 当前时间
来源：http://hz.52xcode.cn/gtmlgqzlsd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtnkcdeqsh.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtahtcevez.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gtsbmrkocl.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtiahdzdaa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtrpuvhmzm.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtwjflofda.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gtekvlighv.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtfatmvcdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtpuzwkpee.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtmsdgyygv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtpbsiscjt.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gteqdtidal.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gtaacxuiec.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtveayhxmr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtewglwvxu.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtkrkjbaed.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tianlin.xyz/gtzjcepaef.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gtirkceiwi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.52xcode.cn/gtgtdebkxt.html

[Q88] 行转列（条件聚合）
来源：http://hz.xuanzx.com/gtciqzxvic.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gthxnpidim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gthihskyqg.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtgpkbyufj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gtnwurxinq.html

[Q90] 生成序号列
来源：http://hz.birdmap.top/gthptabjbz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuanzx.com/gtkhonysds.html

================================================================================
来源：http://hz.c1oappe.top/gtsuwlhfyb.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtdrditcrb.html

================================================================================
来源：http://hz.shzxlz.cn/gtyvxzrxkx.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtdvrdwhpi.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtxzabbspi.html

set -euo pipefail
来源：http://hz.nanxuanxn.top/gtrtjtcych.html

[R02] 变量赋值与使用
来源：http://hz.dianchejie.cn/gtmvrcnlvi.html

name="Tom"; echo "$name"
来源：http://hz.316326.xyz/gtwpodscbh.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtirsxyasf.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtqiukxfmn.html

[R04] 位置参数
来源：http://hz.jinyuanbaomall.cn/gtfcyvcpsx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gtywlrypgk.html

[R05] 参数默认值
来源：http://hz.nwbrower.top/gtatdylqek.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtmthzzfoo.html

[R06] 判断命令是否存在
来源：http://hz.zhiwuduotai.top/gtzfgqijsv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gteguxqyob.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtqkrjmvbd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtyavantxu.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtttjbkpez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtofbeyufz.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtodtpxask.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenlongwang.top/gtisycoajj.html

[R10] 正则匹配
来源：http://hz.ywan-chungtsiang.top/gtitsxtkez.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtivqfngwx.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtxbccaefh.html

case "$1" in
来源：http://hz.jinyuanbaomall.cn/gtbcdxpffp.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gtqojpzqws.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtpsuwesqh.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtetacrnso.html

esac
来源：http://hz.zhijiandao.cn/gtdyxlbzul.html

[R12] for 遍历文件
来源：http://hz.zhijiandao.cn/gttckthnql.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xinyue.icu/gthklhtuby.html

[R13] for 计数循环
来源：http://hz.xuanzx.com/gtwgbtnjeg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtcqljtcza.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtnxyiplsn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jianghu66.top/gtcwhdgzok.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtzssskbzr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtwbcujkwd.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtsdpvlvjr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtvnsqwbsk.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtlgympkmi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtlrzfdjdl.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtkvfthqgu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtftkrkujv.html

[R19] 数组长度
来源：http://hz.sufxvd.cn/gttqadokhb.html


<!-- 参考信息 -->