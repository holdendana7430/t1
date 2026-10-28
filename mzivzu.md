代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gzhubu.top/gtgxhehbuu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtwiacqdqh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gtckkrzecf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtzfnxjnyi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ehwqpu.com/gtpdxpiozb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.redwolf501.top/gtonuyhocf.html

[P03] 生成短随机字符串
来源：http://hz.gaohongyu789.top/gtjjalflwb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtnkheuuxe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxuanxn.top/gtrzwxytbq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtavbczvnu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtnlermfoc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gtinmgebpg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gthnrvbitt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtyrlcicsy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtkqjbjhhv.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtdrlydudk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yuxming.cn/gtvtedifjc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtfjfpijxe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtmvtrpaef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtwandxsty.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxinkj.top/gtmlfjrowx.html

Go:   len(arr);  len(m)
来源：http://hz.cucudq.cn/gtqtgfezrw.html

Ruby: x.length;  x.size
来源：http://hz.wangshuangyany.cn/gtdktwqwwo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yonumen.top/gtbcufztbx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.9152youxi.cn/gtdkketqkh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnqzz.top/gtivjbbarf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gtyruiriug.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gthnhkfjzy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guowangkeji.top/gthjhnjuff.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtmzrjvgyr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtbvcsmsey.html

Ruby: a == b
来源：http://hz.cucudq.cn/gtxtwgadhq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtacmxjewc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtjwnvcpxs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aibaodan.cn/gtjlpzbpbb.html

PHP:  if (empty($x)) {}
来源：http://hz.nwbrower.top/gtajinxtnl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nanxuanxn.top/gtvjipizyt.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtopgwhqlq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtyypjovof.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtkliclflk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtdepkwxam.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtrwncozgq.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtsfsuzkrp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtbqftpehz.html

PHP:  // 手写时间戳比较
来源：http://hz.daxiang520.top/gttbfxzjpm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtlolbvoqj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtklrlotsy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gttqspauvf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dashuyun.cn/gtotkcqbbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhiwuduotai.top/gtndsykanz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zdqjudy.top/gtghjeoyff.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtevdriyao.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gthprsgmyo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.c1oappe.top/gthujqygqc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gtiojgpuzd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fzhhl.top/gtprjigtsi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daxiang520.top/gtpljnniqe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.smart0.xyz/gtbooisibe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtfpbslcjb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtksibttjp.html

================================================================================
来源：http://hz.fengsongda.top/gttizttkvd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtcemdtaey.html

================================================================================
来源：http://hz.hywenlv.cn/gtgcrgjklq.html

[Q01] 创建表
来源：http://hz.guowangkeji.top/gtumnmwcci.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gtsgtsygiz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tanke756.top/gtcjbxxqkr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhiwuduotai.top/gtzcufgxgk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnqzz.top/gtgwmtyody.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gogol.net.cn/gtediddvfk.html

);
来源：http://hz.nwbrower.top/gtpakpispd.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtayvrgfll.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gtsgjuxdka.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtibcnctiv.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gttunpdlfq.html

amount DECIMAL(10, 2),
来源：http://hz.zhaomingkeji.xyz/gtuufdxdfe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yangfankeji.com/gtxdnewlxl.html

);
来源：http://hz.hywenlv.cn/gtswupocov.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtsaehlcbm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tianlin.xyz/gtzqzuteqp.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtyhqhexgf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gtmhpzfmnh.html

[Q05] 重命名列
来源：http://hz.xziqi.cn/gtepteerxe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.snrcjt.cn/gtbhyarduf.html

[Q06] 删除列
来源：http://hz.zycfv.cn/gtdjrsnxbl.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtbmgkqusi.html

[Q07] 删除表
来源：http://hz.wangshuangyany.cn/gtcyqtgwaq.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cashguo.top/gtddipaibh.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtdcjsgotb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtpewzsujb.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtqnozkryr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtlwvraiip.html

[Q10] 插入单行
来源：http://hz.sweek.top/gtxyjwxxun.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhaomingkeji.xyz/gtwfomeztv.html

[Q11] 一次插入多行
来源：http://hz.chenlongwang.top/gttvhmxiva.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtenfdkudy.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtktgfxndh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenlongwang.top/gtawidtihk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtvcnkwvto.html

[Q13] 忽略重复插入
来源：http://hz.dianchejie.cn/gtyejqbnlt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jlsjyb.cn/gtwrqifpwr.html

[Q14] 存在则更新（upsert）
来源：http://hz.xingfuxueyuan.xyz/gtzpbipzty.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.c1oappe.top/gtxchwheej.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtiipuegcn.html

[Q15] 查询全部
来源：http://hz.sweek.top/gtcixolzxh.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gthiusptqm.html

[Q16] 查询指定列
来源：http://hz.svipenyu.cn/gtrtbcerfh.html

SELECT id, name FROM users;
来源：http://hz.mhx1999.top/gtnfisuvif.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtcaxsrmhw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtwtxcpshw.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtoegmxvsi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.smart0.xyz/gttszticbs.html

[Q19] 范围查询
来源：http://hz.xuanzx.com/gthetdwxrd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtzlzwyetm.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtxgwtwzdr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.svipenyu.cn/gtpjrrcamp.html

[Q21] 空值判断
来源：http://hz.jqgfzy.top/gtskkrbyau.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.snrcjt.cn/gtswdjahbk.html

[Q22] 排序
来源：http://hz.zhengqikj.top/gtuakyncfv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.mhx1999.top/gtdmebgmfw.html

[Q23] 分页
来源：http://hz.nanxinkj.top/gtfcdfkqrb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtxddiarkz.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtnbwgafdc.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtsqibvgjz.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtnvkauabl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.bjfxy.top/gtbtwbjjfw.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtfuikjixh.html

SELECT COUNT(*) FROM users;
来源：http://hz.yongpay.top/gtuzhrlthd.html

[Q27] 条件计数
来源：http://hz.cucudq.cn/gtmolyblos.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtffcufpxr.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtxiilklij.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtgynkotfq.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtfxsxskoj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtpulwfhdd.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtpazvzday.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtvrohthft.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gtldseavvo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cheryme.top/gtnhjfjtyw.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtjhlrbwhq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtmvtzebug.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtfaqmxkur.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtddtqkqjp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtruhcgdbj.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtgsopobzn.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtszhlkkds.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.snrcjt.cn/gtownkqspw.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtxrasqcqk.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtkimkmrep.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtirmwdjry.html

[Q36] 左连接
来源：http://hz.gotoacloud.top/gtwmebtvjw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtnpxibbtw.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtdadesyei.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtjrjqoqnu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guowangkeji.top/gtdibwzyav.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yangfankeji.com/gtvxyvcule.html

[Q39] 自连接（查上下级）
来源：http://hz.yongpay.top/gtpvhwnodt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtubwxsijx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guowangkeji.top/gttpodibxg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgfzy.top/gtxjihelea.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtulhypwzt.html

[Q41] 多表连接
来源：http://hz.jinghuilouyu.cn/gtjkyvnvpg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.vqdsnc.cn/gttzwfgfsf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtdkimjyjr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtsaatladg.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtyncamndc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtrdjasdct.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtahtqgede.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtftqhrvra.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtkuodlfnb.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtkjblfebw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtfddkdbeh.html

[Q45] EXISTS 判断存在
来源：http://hz.tian-w.cn/gtvecukawc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtgneuywkk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.birdmap.top/gtjkumpjky.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtvcemidsp.html

[Q47] 与平均值比较
来源：http://hz.nanxuanxn.top/gtpgxfhgui.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtvjbnxkcv.html

[Q48] CTE 公用表表达式
来源：http://hz.cheryme.top/gtifznikpw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cdnleiting.top/gtkthwlvpy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtvjmcndkh.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtyawxqclh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtfasfahkp.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtxxbparod.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jianghu66.top/gtqjrdyjxg.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtnohdxreb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuetiantiany.cn/gteyflnrbb.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtalzuzref.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gogol.net.cn/gtocujwtzw.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtyhblsvod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtewoybjng.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtvruuqdqw.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtqdzkradn.html

[Q55] 排名（并列占位）
来源：http://hz.dianchejie.cn/gtsovnxezw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258888.top/gtbmfuaqyn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xylfe.cn/gtktyfpfkn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.316326.xyz/gtmzlvjzfx.html

[Q57] 行号
来源：http://hz.chenzaomai.com/gtuoqqgbwz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtwqalmsek.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtqpqbkrac.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtcwcbjdkm.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gtjheehdqe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.vqdsnc.cn/gtmipnyqpt.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtlhzucelb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.0kj1m.cn/gtccsnlcbn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zycfv.cn/gtzjeymles.html

[Q61] 移动平均
来源：http://hz.aibaodan.cn/gtyoaqxhvr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtmzraclgz.html

[Q62] 分组占比
来源：http://hz.iojbl.cn/gtsmlkxndv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtbllwdulx.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtfevqlwim.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guowangkeji.top/gtyncafsxz.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gtanzgfcos.html

COMMIT;
来源：http://hz.nanxuanxn.top/gttjrqnajr.html

[Q65] 回滚事务
来源：http://hz.andypj.xyz/gtnblrcmck.html

ROLLBACK;
来源：http://hz.cdnleiting.top/gtiucobzmw.html

[Q66] 行锁查询
来源：http://hz.nwbrower.top/gthfbsirvs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shzxlz.cn/gtnvlikfgk.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtsqfhyuxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhixingplan.top/gtllopvkvi.html

[Q68] 保存点
来源：http://hz.fengsongda.top/gtsawzwcix.html

SAVEPOINT sp1;
来源：http://hz.vqdsnc.cn/gtzknbfzpb.html

ROLLBACK TO sp1;
来源：http://hz.aizwys.cn/gtvmnewoml.html

[Q69] 查看执行计划
来源：http://hz.redwolf501.top/gtftfbcwwi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.0kj1m.cn/gtgqklhzrr.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtgaguyxjk.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtppzxrxub.html

[Q71] 查看建表语句
来源：http://hz.guowangkeji.top/gtmpapdzlo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtaiccjhjz.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gtelrfcxao.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtkscizcvh.html

[Q73] 查看表状态
来源：http://hz.zhijiandao.cn/gtmpahtfhs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.52xcode.cn/gtpeevezmi.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtjmltqqut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gthekkjinl.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtrlnckutn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtnfmmpnfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtxugggshv.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtisufbpsq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnxiangtu.top/gtvpiolanb.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtimiuntot.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tian-w.cn/gtyueycwni.html

[Q78] 当前时间
来源：http://hz.iojbl.cn/gtodqkowkq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hammf.cn/gtlxflsxrz.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtkovpkkkc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtbybwpcxk.html

[Q80] 字符串截取
来源：http://hz.nwbrower.top/gtfvckdvei.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtgjftxbzv.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtcoewyomt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gttqqjizyd.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gthidnvuow.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtezhsfulg.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtjcgelyqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtrrfbhflc.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtqlfmsbjg.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gtptomegem.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtlsiztvya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gtonagwzdr.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtpwhuwmvm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtskalrtga.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtvbckpffc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yongpay.top/gtndozlbsp.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gttbeqakrf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.vqdsnc.cn/gthuqmeiag.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aizwys.cn/gtvaqvlrct.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtbvnkptmh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuanzhike.top/gtgvhffibp.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gttcjjwyla.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenzaomai.com/gtioychstt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtiuxwczkz.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtnxvpyots.html

================================================================================
来源：http://hz.dianchejie.cn/gtkkiptglm.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtplfcnlkm.html

#!/usr/bin/env bash
来源：http://hz.52xcode.cn/gtlcisfvdn.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtouwlemdq.html

[R02] 变量赋值与使用
来源：http://hz.fzhhl.top/gtneuwfktp.html

name="Tom"; echo "$name"
来源：http://hz.snrcjt.cn/gtjvorckbl.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtphufzxlm.html

readonly PI=3.14
来源：http://hz.jinyuanbaomall.cn/gtisgpvejj.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtehzmqgkl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenzaomai.com/gtparaijvm.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtcqzpbqwj.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtfbpnliag.html

[R06] 判断命令是否存在
来源：http://hz.zhijiandao.cn/gtldlsvhow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtmtqhcboe.html

[R07] if 判断文件
来源：http://hz.gogol.net.cn/gtadvnbodf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gthwatmutc.html

[R08] 数值比较
来源：http://hz.dianchejie.cn/gtnknbvbhu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guowangkeji.top/gtzqazvpai.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtsopuntvo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtmmcgubrg.html

[R10] 正则匹配
来源：http://hz.jqgufenzy.top/gtugtwujov.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.smart0.xyz/gtrcyfuiyh.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtareiqycf.html

case "$1" in
来源：http://hz.aibaodan.cn/gtzsncieoa.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtuaaticgv.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtkcehgkmq.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gtbuvmdvts.html

esac
来源：http://hz.pycfn.com/gtfnginvmh.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtdvaogdls.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtdcjwylio.html

[R13] for 计数循环
来源：http://hz.sufxvd.cn/gtoukvtcoq.html


<!-- 参考信息 -->