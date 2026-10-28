代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtzjukekpz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tian-w.cn/gtogrndawa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhengqikj.top/gtmkffgrko.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gthzgysoym.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gtymwoshoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.0kj1m.cn/gthvctyzav.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gtsoqtxznc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtldezoyjq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtmxuxbbwy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtljlxtugo.html

[P03] 生成短随机字符串
来源：http://hz.redwolf501.top/gtyoqvypys.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtradrheob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gtanocvmad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtmlkngbno.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtidtbocoq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gtdbjrqiug.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtomgkohvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtooqiqmai.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtcdgyijqp.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtsnottgsk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxinkj.top/gtuhlokdud.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtwuuamyzw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtvtvkilmx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hongshengwenyu.top/gtranixsdo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.chenjidiqi.icu/gtqvoelmib.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gttcrjjjik.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gtkdolyybz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtgomcrqpt.html

[P05] 判断两个对象内容是否相等
来源：http://hz.smart0.xyz/gtmysilnov.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gtjbtfkbul.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtxnezvjis.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shangyingyoupin.top/gtawnuvtnh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gtqqdihajl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pengpengdd.cyou/gtgwjwjvex.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.0kj1m.cn/gtlezrlrpr.html

Ruby: a == b
来源：http://hz.ydzc1.top/gtabwamreq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gzhubu.top/gtspiomltc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtkkrusoch.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shzxlz.cn/gtfhfulong.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtlbtirxvm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtcefqsiiu.html

TS:   if (x == null) {}
来源：http://hz.daria6918.cn/gthnqjadvw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sufxvd.cn/gtixrfpizg.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gtmnspyoit.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtapnxlvvi.html

C#:   if (x is null) {}
来源：http://hz.yongpay.top/gtmvqpbhtm.html

[P07] 防抖与节流
来源：http://hz.yuxming.cn/gtxayfnhgd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtxhcbtqfz.html

PHP:  // 手写时间戳比较
来源：http://hz.xylfe.cn/gtmdxdtirs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtitcplafl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtkfwvganz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gturnhpazi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtdwgdcojh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinqigfzy.top/gtxfdqtpai.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtgxtpppid.html

[P08] 处理浮点精度问题
来源：http://hz.feifeiyinyue.top/gtojknixbs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtseyzhaby.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtzdwgavqh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shanyushiyangkeji.top/gtwrnmffwp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtscxksorv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jianghu66.top/gtadwakeqm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydzc1.top/gtzsbmdwxy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dashuyun.cn/gtrgmkkmrx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hywenlv.cn/gtusgxfpaj.html

================================================================================
来源：http://hz.hnqzz.top/gtnxdgtowj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtjjakuiyr.html

================================================================================
来源：http://hz.hysaishi.cn/gtgyvffipi.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtsvbqrwzf.html

CREATE TABLE users (
来源：http://hz.dashuyun.cn/gtmotrctmj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtcifswuao.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtxlvghiug.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sysykeji.top/gtgehfxgqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yongpay.top/gtnsjczhwr.html

);
来源：http://hz.yanxiufei.cn/gtfddrhzzz.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtyvqkofgy.html

CREATE TABLE orders (
来源：http://hz.gogol.net.cn/gtdtopwexy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtcnpfbnxo.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gthlvuzevl.html

amount DECIMAL(10, 2),
来源：http://hz.snrcjt.cn/gtynowinnx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtynzcexcw.html

);
来源：http://hz.yongpay.top/gtlrgujlgt.html

[Q03] 增加列
来源：http://hz.zhaomingkeji.xyz/gtejvsluks.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cqqwz.cn/gtjxoujaxe.html

[Q04] 修改列类型
来源：http://hz.ivvv.top/gtppquqgvi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtkgsvnpaq.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtkxropytl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.haohaochexian.top/gtzuqzhhbh.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtkralwmon.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jyoumei.cn/gtoifyvsdv.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtnhrrczwh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtpjzzpokm.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtdysxmpha.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtgghmacla.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtditxklts.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangdashe.top/gtcvchowhl.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtowyatnpw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gaohongyu789.top/gtkdvkqijo.html

[Q11] 一次插入多行
来源：http://hz.yanxiufei.cn/gtqvzdnnnt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangkeji.top/gtocrdzesr.html

[Q12] 插入后取自增 ID
来源：http://hz.gogol.net.cn/gtwtgdhcko.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtqtaqtjkj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtmfclenfh.html

[Q13] 忽略重复插入
来源：http://hz.jqgufenzy.top/gtvmdaifdq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nwbrower.top/gtctrevflj.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtbylsujvx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtvgpxfilu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtljkotwgi.html

[Q15] 查询全部
来源：http://hz.jianghu66.top/gtfwrsypoq.html

SELECT * FROM users;
来源：http://hz.zycfv.cn/gtsawtpusn.html

[Q16] 查询指定列
来源：http://hz.zhijiandao.cn/gtzlsdgwen.html

SELECT id, name FROM users;
来源：http://hz.shzxlz.cn/gtmxvkifza.html

[Q17] 条件查询
来源：http://hz.sweek.top/gtexxnylmt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.havefunace.top/gtqhsblmsz.html

[Q18] 模糊匹配
来源：http://hz.xinyue.icu/gtqoaxhkgr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtlfyiagvk.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtcwpqueje.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtxrsarvva.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtfuxatxsj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.52xcode.cn/gtitpgomqi.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtfnufgygx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gteexqmzxl.html

[Q22] 排序
来源：http://hz.shanyushiyangtech.top/gthofsyxqg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guowangkeji.top/gtpdafewnq.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtcjrnykcu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtccgoflyc.html

[Q24] 去重
来源：http://hz.bjfxy.top/gtyazjuuar.html

SELECT DISTINCT city FROM users;
来源：http://hz.guowangkeji.top/gtzwpcastq.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gtoxpcujnr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtjegfhqxn.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gtasnshgut.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtxrbhcjlm.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtemufierb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtuoadnorp.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtdahncouc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangshuangyany.cn/gtbtbzmlot.html

[Q29] 最大最小值
来源：http://hz.c1oappe.top/gtnwsevams.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gtxztdmwau.html

[Q30] 分组统计
来源：http://hz.jianghu66.top/gtiowljdhk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yonumen.top/gthyaspwkl.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtbdcvbbuq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ivvv.top/gtvyotwzmr.html

[Q32] 分组拼接字符串
来源：http://hz.aibaodan.cn/gtuylzqwri.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtjcodhblx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.9152youxi.cn/gtltpbnoqv.html

[Q33] 多列分组
来源：http://hz.yueranfly.top/gtnobavitc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gthawecufo.html

[Q34] 每组取第一条
来源：http://hz.jyoumei.cn/gthivljjmj.html

SELECT * FROM (
来源：http://hz.gotoacloud.top/gtpaijlvot.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtbgtznfvw.html

) t WHERE rn = 1;
来源：http://hz.feifeiyinyue.top/gttvkpngyq.html

[Q35] 内连接
来源：http://hz.jqgfzy.top/gtmwuzvmhm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtbrwmzvjk.html

[Q36] 左连接
来源：http://hz.shangyingyoupin.top/gtmlzrwgxe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtbwtsyyrz.html

[Q37] 右连接
来源：http://hz.chenzaomai.com/gtmbljxjoq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cashguo.top/gtkwgxvtwu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtoxkgcmbh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuanzx.com/gtmyqgnqro.html

[Q39] 自连接（查上下级）
来源：http://hz.yuxming.cn/gtmanifvlc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ehwqpu.com/gtpsmcdfwm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtiphpantb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtwuwdnlyp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtuddhzizc.html

[Q41] 多表连接
来源：http://hz.ivvv.top/gthyunwujg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtofdssnbb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtnalpwdsa.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.316326.xyz/gtygifcsez.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigfzy.top/gtejiferbg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtzwwnewlh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtpxwpedbu.html

[Q43] 标量子查询
来源：http://hz.bjfxy.top/gtbdbaoegl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zdqjudy.top/gtjlnmqibv.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gtzighhsys.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtiwjcdkzm.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtpxcspzny.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtexcazkdz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hywenlv.cn/gtmliistgk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtlvkhvpdu.html

[Q47] 与平均值比较
来源：http://hz.xinyue.icu/gtihtyigul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtxdavagct.html

[Q48] CTE 公用表表达式
来源：http://hz.guowangkeji.top/gtoirguzkv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtdijybjge.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtgqgkiuad.html

[Q49] 更新单行
来源：http://hz.yvedp.cn/gtyanqhdek.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtkuolydtx.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gtjkkknuqw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtdmbccvfi.html

[Q51] 用子查询更新
来源：http://hz.yj20258.top/gtpajncmfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gtuverfaym.html

[Q52] 删除指定行
来源：http://hz.hongshengwenyu.top/gtrjqwvkyj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtpcwfbirk.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtsxvmhobt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gtcclevtyr.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtemjrzhje.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtnabueirs.html

[Q55] 排名（并列占位）
来源：http://hz.vqdsnc.cn/gtrcxphhon.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtlfkccyey.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgfzy.top/gtgzdiqeub.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shuidangran.top/gtzthkeudr.html

[Q57] 行号
来源：http://hz.haohaochexian.top/gtlgjleapf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtamhkyhwj.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtposlgloz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenlongwang.top/gtbqwjkecn.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtcsckwnxb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gtieufeyvc.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gtjpnejpfg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtsyechjwh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtkuvgbslm.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gtjbvrqdkc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tanke756.top/gtodczrvoo.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtqjbjqhsg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtmyftcrcd.html

[Q63] 开启事务
来源：http://hz.daria6918.cn/gthjphqjrb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cdnleiting.top/gtnlxnxfhq.html

[Q64] 提交事务
来源：http://hz.yj20258.top/gtyheeahyn.html

COMMIT;
来源：http://hz.yonumen.top/gtggniirtt.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtvojcjhrk.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtrfcihagi.html

[Q66] 行锁查询
来源：http://hz.zhaomingkeji.xyz/gtegzjtsot.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtbkdrzlvf.html

[Q67] 设置隔离级别
来源：http://hz.cucudq.cn/gtktqobdmj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.birdmap.top/gtxfjocfjr.html

[Q68] 保存点
来源：http://hz.snrcjt.cn/gtipiqomjn.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtaslhhhjv.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gtqnsabrht.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gtsxpiwzji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinghuilouyu.cn/gtalflnulf.html

[Q70] 更新统计信息
来源：http://hz.ppjwa.cn/gtbmhqtxqk.html

ANALYZE TABLE users;
来源：http://hz.meibo888.top/gtnastbtxh.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gtumvbgxjp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ywan-chungtsiang.top/gtmoovswff.html

[Q72] 查看索引
来源：http://hz.jiagoushi.top/gtodzcjgrl.html

SHOW INDEX FROM users;
来源：http://hz.sufxvd.cn/gttftwibok.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtznxfuxsp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtatlxvxqu.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtggmjnmho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aizwys.cn/gtmzozaunt.html

[Q75] 日期格式化
来源：http://hz.yanxiufei.cn/gtakqauqkq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtlxqncuyp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtstnavycc.html

[Q76] 按天统计
来源：http://hz.xingfuxueyuan.xyz/gtltzykkje.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtkmcyevrp.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtqanmlvdp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtxmvmwgvf.html

[Q78] 当前时间
来源：http://hz.52xcode.cn/gtwzeqpcvk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtofibgmaw.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtnozlzbde.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yongpay.top/gtlriekxmy.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtsmrdfuhj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtbtvrhyyd.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtrpqizsxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuetiantiany.cn/gtaaeiiwwd.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtnwgizsgo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.smart0.xyz/gtosuyisem.html

[Q83] 大小写转换
来源：http://hz.gaohongyu789.top/gtqdflunch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cheryme.top/gtccdxxmoi.html

[Q84] 去除首尾空格
来源：http://hz.zhijiandao.cn/gtfknawxbg.html

SELECT TRIM(name) FROM users;
来源：http://hz.vqdsnc.cn/gtsqnfwzup.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtysunbqvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangdashe.top/gtfendyxid.html

[Q86] 读取 JSON 字段
来源：http://hz.aizwys.cn/gtzbefalae.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtdcdysdrl.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gthuvnmsme.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gtbdicnjir.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtfjefhijx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtmvknnvzi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gtfxyutjjq.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtnqzwtsxv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtfszlvxey.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gtbgsnifaq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtrwmbghjx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrkzboixr.html

R. Bash 专题
来源：http://hz.hnxiangtu.top/gtkoxyfegz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpeaenhfc.html

[R01] shebang 与严格模式
来源：http://hz.svipenyu.cn/gtaevdyuyf.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtqrmnkszb.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtcilgyjfg.html

[R02] 变量赋值与使用
来源：http://hz.jyoumei.cn/gteaoixuti.html

name="Tom"; echo "$name"
来源：http://hz.yuanzhike.top/gtlybapwmv.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtaqdzkqse.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtwavsylpy.html

[R04] 位置参数
来源：http://hz.haohaochexian.top/gtykwoewdc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtxuotlawf.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtgguyrubf.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtuljpzzaf.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtuufxxstv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xinyue.icu/gtpogckufl.html

[R07] if 判断文件
来源：http://hz.zhengqikj.top/gtyzypxriv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtefcasakr.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtkvnnvejg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtdpyqvyub.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtxctorcxw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sxryk.cn/gtkxfncxad.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtdjponagm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtgppwgrpv.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtcfxyegyr.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtdjzfhztm.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gtbsymsuik.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtndttwsrk.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtrjhpuexa.html


<!-- 参考信息 -->