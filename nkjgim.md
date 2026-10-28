代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhiwuduotai.top/gtsmxezvrg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gtngcizjbu.html

[P03] 生成短随机字符串
来源：http://hz.jlsjyb.cn/gtoyotwoqk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenzaomai.com/gtyydlcnus.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ywan-chungtsiang.top/gtcjyejben.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtbzldrhbt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtpqcqzbjb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.52xcode.cn/gtuwfylmao.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtslxwcevs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cqqwz.cn/gtvgqaxnik.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cheryme.top/gtukgilebt.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtzbjvvxmp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cdnleiting.top/gtgiaitovw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gttopulpxe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtbhykmzna.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gttjezjhkd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtrksocvho.html

Go:   len(arr);  len(m)
来源：http://hz.hysaishi.cn/gtnxyormdd.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtvrwgmvts.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hammf.cn/gtmycrwbyb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hammf.cn/gtwmaynyxg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtzbgbchpg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtvvteqpdx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtbisnoydg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258.top/gtftmivsdl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hfpthk.cn/gtustbycko.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtzsaddyaa.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtjnxfqkle.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yvedp.cn/gtkutvnrnh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.daria6918.cn/gtmpfjxpoi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xingfuxueyuan.xyz/gtlcoimcyo.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtpbcvkflb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.mhx1999.top/gtpcytbprv.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gtdcwkyvbs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtphaynapy.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtdtayocqp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tianlin.xyz/gtwyeugbkf.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gthlzmgext.html

[P07] 防抖与节流
来源：http://hz.zdqjudy.top/gtvqojelan.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258888.top/gtujrdckjx.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtqxupodio.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtmkszutnl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtkrhqocsp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gttkbucelk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtsdtrgwim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhoulong.xyz/gtaiagsehc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gthibrysgy.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gtkjaasgei.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtxtzetgga.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtqobywtcr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtsemsewdh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sysykeji.top/gtpxakzkrp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangdashe.top/gtukutetln.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtujxkjtat.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtwmapdhby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ywan-chungtsiang.top/gtqmxfonxp.html

================================================================================
来源：http://hz.fengsongda.top/gtzgubfrxo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtfhdyvkos.html

================================================================================
来源：http://hz.xinyue.icu/gtgacuenjd.html

[Q01] 创建表
来源：http://hz.yvedp.cn/gtuvkvyrzr.html

CREATE TABLE users (
来源：http://hz.yongpay.top/gtfogybnni.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtalunvuck.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jyoumei.cn/gtfcmwuldf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nanxinkj.top/gtkbyitaig.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daria6918.cn/gtncqbnulz.html

);
来源：http://hz.chenjidiqi.icu/gtpmncvjol.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gtrydlpnwz.html

CREATE TABLE orders (
来源：http://hz.aizwys.cn/gtznmfldcz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtmxfvcybk.html

user_id INT NOT NULL,
来源：http://hz.shanyushiyangkeji.top/gtqwxekkox.html

amount DECIMAL(10, 2),
来源：http://hz.0kj1m.cn/gtzkqbhcwl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yanxiufei.cn/gtpdxyztbi.html

);
来源：http://hz.tanke756.top/gtxzgdsgxz.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtmztpauks.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtvqijucfd.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtbbaotufy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jiagoushi.top/gtnurknjik.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtwsepkrul.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jianghu66.top/gtjwbdvlzu.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtaefdpuie.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.guannengcc.top/gtnitwzipx.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtxiknawvh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhiwuduotai.top/gtjgsxhrxf.html

[Q08] 创建普通索引
来源：http://hz.aibaodan.cn/gtmrudjhrd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtrhhebtnz.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtxzedzwhz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtzwgxxbzv.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtzaismedf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gtfnvayryl.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtkgeqefda.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtupipzcdy.html

[Q12] 插入后取自增 ID
来源：http://hz.jyoumei.cn/gtkrzfshtv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtvwslzxnf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gtlxnhktbc.html

[Q13] 忽略重复插入
来源：http://hz.gzhubu.top/gtksorjtui.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.tian-w.cn/gtccktmklw.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtouczpvmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuetiantiany.cn/gtkglcrimt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fzhhl.top/gtnvczrbis.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gtztmpffub.html

SELECT * FROM users;
来源：http://hz.jqgfzy.top/gtbgpuenfs.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtjgwnvugd.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtmmyhfegn.html

[Q17] 条件查询
来源：http://hz.iojbl.cn/gtbavrmalm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.snrcjt.cn/gtphsxsdgu.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtnjlhgkfe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daxiang520.top/gtpmiksgit.html

[Q19] 范围查询
来源：http://hz.yangfankeji.com/gtusqervci.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxinkj.top/gtzotfwkxb.html

[Q20] IN 列表
来源：http://hz.yangfankeji.com/gtxjadcbfn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtslvwtegj.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gtpguldkrq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gteyikjqdy.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtscrwytls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.0kj1m.cn/gtzowocryo.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtcjdgsvpm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinyuanbaomall.cn/gtasjqwvfm.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtxzqgboma.html

SELECT DISTINCT city FROM users;
来源：http://hz.cheryme.top/gtgogxrjni.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtzjadtlxq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gteskazgnh.html

[Q26] 计数
来源：http://hz.ydzc1.top/gtihhlujny.html

SELECT COUNT(*) FROM users;
来源：http://hz.meibo888.top/gtcmuklyry.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtxnvqpema.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtfccxocqj.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gtoftofaxi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.c1oappe.top/gtngmnjfil.html

[Q29] 最大最小值
来源：http://hz.yvedp.cn/gtvtoaaxcw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtbuiwpphf.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtmbwqslag.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtmmqnsdkr.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtpyzaoiuk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gttegnvlox.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gthqnegwtg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtiyhjsnur.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtwxndtpfg.html

[Q33] 多列分组
来源：http://hz.guowangkeji.top/gtbbvktjwx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtgcmmclwc.html

[Q34] 每组取第一条
来源：http://hz.aibaodan.cn/gtcpisloni.html

SELECT * FROM (
来源：http://hz.sufxvd.cn/gtlkyacjih.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtfkelkqtl.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtrmkjqzgm.html

[Q35] 内连接
来源：http://hz.yj202588.top/gtlbhybawo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtcsnckfti.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtnyfyfjui.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtliceelbd.html

[Q37] 右连接
来源：http://hz.xziqi.cn/gtgyooltfu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtkyevzeuq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shzxlz.cn/gtjnmxmuzo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gthzbjmkwm.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtousttqni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tianlin.xyz/gtmvtwyber.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hysaishi.cn/gtwaccdnga.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtucecygcx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgufenzy.top/gtatjakrwb.html

[Q41] 多表连接
来源：http://hz.xingfuxueyuan.xyz/gtpmxpftva.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cqqwz.cn/gtnedowqvi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sysykeji.top/gtrnvvxzra.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtwblvmgrs.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtinznbmne.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shangyingyoupin.top/gtqvzwitsr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtfkaxhpex.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtwklmvvqh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgufenzy.top/gtravcaqis.html

[Q44] IN 子查询
来源：http://hz.birdmap.top/gtzjrkfjvm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtixmsxmww.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtedeekajy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtszthwyoe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hysaishi.cn/gthnphlwtx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtxcfkzext.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtlqgoyfjn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtkxjxhrzy.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigfzy.top/gtglkbbkcn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tian-w.cn/gtalsibczx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shzxlz.cn/gtseathale.html

[Q49] 更新单行
来源：http://hz.ppjwa.cn/gtazqummbz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtrvrnpozk.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtzxflqhus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gtxwfrvtdp.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gteihclthc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.andypj.xyz/gtkzqfmhhj.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtpqjgbizq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cqqwz.cn/gtnzcsfvxy.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gteixryixk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtlxfxgouc.html

[Q54] 清空表
来源：http://hz.shanyushiyangtech.top/gtbdspdkcp.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gtggplbpwn.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigfzy.top/gtmtauizvr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtmqebkcyn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tanke756.top/gtgzhpwogn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gaohongyu789.top/gteajkpwap.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtvelertzk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtknsiunmx.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtpgrpepjb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtzgkywtas.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtmfyqreje.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shuidangran.top/gtgxfiyvql.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtzqylcomo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtmwdhdgxo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtfzostoqe.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtdiaqlaef.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtsimihnng.html

[Q62] 分组占比
来源：http://hz.cucudq.cn/gtkyvtkqum.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtdcsdvtie.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtsblzqqml.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtkwoxsgil.html

[Q64] 提交事务
来源：http://hz.yj202588.top/gtxixeddhi.html

COMMIT;
来源：http://hz.yj202588.top/gtexzllrmd.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtxjavzpqh.html

ROLLBACK;
来源：http://hz.zycfv.cn/gtlcuvgzgc.html

[Q66] 行锁查询
来源：http://hz.fengsongda.top/gtniztywdo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuanzx.com/gtzudljkmm.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtdyrydizs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtbjwzkitk.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtmhthafrw.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtekcrrwoi.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gtwxahidnr.html

[Q69] 查看执行计划
来源：http://hz.tianlin.xyz/gttfjctkqk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtbolmscxx.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gttfmsqzop.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtwxkriiqd.html

[Q71] 查看建表语句
来源：http://hz.yongpay.top/gtckmwegqy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtvsvhaeje.html

[Q72] 查看索引
来源：http://hz.kuanghao11.cn/gtqaabavwe.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtbdjnejfk.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtezhxarnv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shzxlz.cn/gttrzmqoaf.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtfvnlrtiz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtwndzgxyf.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gtcipoiheq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xziqi.cn/gtwzaixaaw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gtevnxnbuk.html

[Q76] 按天统计
来源：http://hz.xingfuxueyuan.xyz/gtystgyfqb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtjrlcwipr.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtfujvaegp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtcjstnnoi.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtsprgygwv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ehwqpu.com/gtnqhknipg.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtientrpff.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.iojbl.cn/gtfnhunonu.html

[Q80] 字符串截取
来源：http://hz.jqgfzy.top/gttviyipbb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xziqi.cn/gtqgomkpbn.html

[Q81] 字符串替换
来源：http://hz.jianghu66.top/gthvxzuzom.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtjuunoche.html

[Q82] 字符长度与字节长度
来源：http://hz.xuetiantiany.cn/gtnbdgybyv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtgmokujva.html

[Q83] 大小写转换
来源：http://hz.cheryme.top/gtqhnkkunh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtvqromhsh.html

[Q84] 去除首尾空格
来源：http://hz.cucudq.cn/gtqanduzle.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtbxwkhmje.html

[Q85] 数值取整
来源：http://hz.zhijiandao.cn/gtyciqbaua.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtdgxvyiry.html

[Q86] 读取 JSON 字段
来源：http://hz.yvedp.cn/gtijdnlpzv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtxmmkwizt.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtftqjmvqx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.c1oappe.top/gtjmpgaepd.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtshzgmibz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gthamrzlay.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtgegaiefi.html

[Q89] 判断表是否存在
来源：http://hz.jinghuilouyu.cn/gtjmvcovna.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtptxkyuqf.html

[Q90] 生成序号列
来源：http://hz.cdnleiting.top/gtlhhgtwfn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangdashe.top/gtpoxmgboz.html

================================================================================
来源：http://hz.fengsongda.top/gtzsbgrktm.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtgprxcodh.html

================================================================================
来源：http://hz.xylfe.cn/gtppntwhgo.html

[R01] shebang 与严格模式
来源：http://hz.sxryk.cn/gtluxzgvre.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtcxmotmor.html

set -euo pipefail
来源：http://hz.cqqwz.cn/gtdtdtxrtz.html

[R02] 变量赋值与使用
来源：http://hz.yanxiufei.cn/gthxktbkol.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gthepkomqg.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtriacmavw.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gttndcwvhh.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtnlnkorgo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtragwgsmc.html

[R05] 参数默认值
来源：http://hz.jinqigfzy.top/gtumwchfsa.html

name="${1:-default}"
来源：http://hz.xziqi.cn/gtsflabedn.html

[R06] 判断命令是否存在
来源：http://hz.xziqi.cn/gttahiywqj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtezzrfiyr.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gtfidhqryj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gtpcnltmip.html

[R08] 数值比较
来源：http://hz.yangfankeji.com/gtpsidxivz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gthvuovtna.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtbdrafpdm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtdwhrwnlt.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtmodfkhgg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtsusklzth.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtguoiiwxk.html

case "$1" in
来源：http://hz.chenlongwang.top/gtxccsften.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtqdzuncnb.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtstlhdksp.html

*)     echo "未知命令" ;;
来源：http://hz.vqdsnc.cn/gtttydblmh.html

esac
来源：http://hz.jlsjyb.cn/gtuvjoougy.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtmxxuvqhw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gtzsnoyowb.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtvqbldmpu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gtxqjootft.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtfwoajfmo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gteybladxc.html

[R15] while 逐行读文件
来源：http://hz.gotoacloud.top/gtejqlaykz.html


<!-- 参考信息 -->