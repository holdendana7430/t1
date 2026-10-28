代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.yvedp.cn/gtzdlubemg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ivvv.top/gtcjyfuxed.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtbbmsggua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj202588.top/gtvydmzzjr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258888.top/gtujpxdbsg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtjpkmekki.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtaizvzrqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.52xcode.cn/gtqmmfnrwr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtmwtbiaze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtpctazrbk.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtrzqrlyye.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sxryk.cn/gtkcschmhv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigfzy.top/gtcohjdlxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtcdlbeknz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtoaccxsvy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zycfv.cn/gtfkheqtma.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenjidiqi.icu/gtofauqczg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtgkzwbqkd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtwsurhlnb.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtoaiseewo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtisbvtrkh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtrxmkwtew.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtlhnphiod.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtihzhdgli.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hammf.cn/gtjtxnpdez.html

Go:   len(arr);  len(m)
来源：http://hz.birdmap.top/gtnrrgqaqt.html

Ruby: x.length;  x.size
来源：http://hz.chenjidiqi.icu/gturjwqusw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sysykeji.top/gtwtdilhdk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gtpinuikbh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cashguo.top/gtmllhhycn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhiwuduotai.top/gtdrzkaiiv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtjegdccpw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtnqzeqeuy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtlcjljsya.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtxdgjhhia.html

Ruby: a == b
来源：http://hz.sysykeji.top/gteetkswuu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tanke756.top/gtfzuzmfyi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtqajeowtw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtioqkcexc.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtfpwcijjt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtjzinbczn.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtencnyqgo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gzhubu.top/gtqnbpiuov.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtbaxxdxnm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtrladaqbn.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtytbwikbt.html

[P07] 防抖与节流
来源：http://hz.zhiwuduotai.top/gtfiksrbic.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtsastxzqm.html

PHP:  // 手写时间戳比较
来源：http://hz.haohaochexian.top/gtxwjgrrpj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtmqleofhl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtzhidocdc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtgrmbswqk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtnlgsdhse.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtygysynhl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtpmeuukcj.html

[P08] 处理浮点精度问题
来源：http://hz.cdnleiting.top/gtqenruski.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtcvkeewfx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.316326.xyz/gthxaoqhrm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gttfzxpklh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sufxvd.cn/gtngfzumaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yvedp.cn/gtlzakhppq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtjpxfoiyz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtfddfbvnt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtblbnpjhk.html

================================================================================
来源：http://hz.jianghu66.top/gtjuzdrgls.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.andypj.xyz/gtkiamscdb.html

================================================================================
来源：http://hz.wangdashe.top/gtosnjzqem.html

[Q01] 创建表
来源：http://hz.zhengqikj.top/gtrkwmvimb.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtxknxuqwf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtkxmonslq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sxryk.cn/gtxpggaoxs.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gtqnoinada.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.52xcode.cn/gtlknvcwni.html

);
来源：http://hz.chenzaomai.com/gtoczizjuc.html

[Q02] 创建带外键的表
来源：http://hz.yj202588.top/gtceiqkoxt.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gtzgpkcsvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuxming.cn/gttzlxivmq.html

user_id INT NOT NULL,
来源：http://hz.gotoacloud.top/gtfzlmunak.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtvkjrnxgw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtzrublaos.html

);
来源：http://hz.vqdsnc.cn/gtqwkwobhm.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtnrfyccim.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtntbvuouy.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtcokersfq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.andypj.xyz/gtdxjphlev.html

[Q05] 重命名列
来源：http://hz.jinqigfzy.top/gtkbnaucpj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtudzrjatv.html

[Q06] 删除列
来源：http://hz.ywan-chungtsiang.top/gtydifagda.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhongyouzk.top/gtvvochxxs.html

[Q07] 删除表
来源：http://hz.shangyingyoupin.top/gtgtnthxlb.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sxryk.cn/gtuspkmpba.html

[Q08] 创建普通索引
来源：http://hz.yj20258.top/gtxefvkktr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtwgnnckri.html

[Q09] 创建唯一索引
来源：http://hz.sxryk.cn/gtbmmonshb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cheryme.top/gtznncwdgp.html

[Q10] 插入单行
来源：http://hz.zhoulong.xyz/gtyiiitcel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xinyue.icu/gtjjxvayon.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtihuokccs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sufxvd.cn/gtwxuhjncj.html

[Q12] 插入后取自增 ID
来源：http://hz.jiagoushi.top/gtyozxvfku.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xingfuxueyuan.xyz/gtzptcgtpk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sxryk.cn/gtjbcagdrx.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtolpgukyp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.svipenyu.cn/gtryzggvif.html

[Q14] 存在则更新（upsert）
来源：http://hz.fengsongda.top/gtciinphzb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hysaishi.cn/gtspssdplf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtuyyowqoy.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtbasnhixd.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gtrztmxsoy.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtcipcpodx.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gthtnkhsxt.html

[Q17] 条件查询
来源：http://hz.cucudq.cn/gthlnhuviu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtlpgtnbfk.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gthcdasvfz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtsjnqocuv.html

[Q19] 范围查询
来源：http://hz.zhoulong.xyz/gtmsvviijo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnqzz.top/gtkstnomjo.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gtddvfkxzl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shuidangran.top/gtluelbmky.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtehwpcqkk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtrxgpifek.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtwjefpgqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtcvpenwkk.html

[Q23] 分页
来源：http://hz.cheryme.top/gtvzsebash.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangtech.top/gtwsyqjlja.html

[Q24] 去重
来源：http://hz.fengsongda.top/gthtbtpdrl.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtniqmyuns.html

[Q25] 只取前 N 条
来源：http://hz.jqgfzy.top/gtrexiczej.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtptwydyma.html

[Q26] 计数
来源：http://hz.meibo888.top/gtyrvxvcrz.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenzaomai.com/gthuxwmuil.html

[Q27] 条件计数
来源：http://hz.ivvv.top/gtogbwgoai.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtjtzqiazk.html

[Q28] 求和与平均
来源：http://hz.mhx1999.top/gtjkdelwst.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yonumen.top/gtnlnemgjd.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtdcybxplg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.c1oappe.top/gtihhwmqpa.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtnghqizim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gttcehlcam.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gtjtajmjkw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtbekmomyb.html

[Q32] 分组拼接字符串
来源：http://hz.ydjk.org.cn/gtksorzpao.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtbqigjgsj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gthembgxle.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtxnzrmuav.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtbrvtquyg.html

[Q34] 每组取第一条
来源：http://hz.hywenlv.cn/gtfcboqmrt.html

SELECT * FROM (
来源：http://hz.cheryme.top/gthqqkmikb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gttdticjfh.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtrusrgxic.html

[Q35] 内连接
来源：http://hz.nanxuanxn.top/gtzmcsfavp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtlpcojhzs.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtalbawglx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.guannengcc.top/gtqhspzzsy.html

[Q37] 右连接
来源：http://hz.yangfankeji.com/gtkdewooyg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtpsqeifqo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenjidiqi.icu/gtxmclcfjt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shuidangran.top/gtmfihgivl.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtzelvxbvc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.havefunace.top/gttxzncozu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenlongwang.top/gtacfjozsu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtyrzsdznx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gtdgsbfszh.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtlwoonaah.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtbbylyfsb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenzaomai.com/gtenujrevo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guowangkeji.top/gtpugshest.html

[Q42] 连接条件附加过滤
来源：http://hz.aizwys.cn/gtgqsadpon.html

SELECT u.name, o.amount FROM users u
来源：http://hz.havefunace.top/gtzayrmhme.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtqnqsdnhk.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gtnqjdrpqj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hysaishi.cn/gtfiejhcbs.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtmlhuhsgh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtfguiktsb.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtchtgpokh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtqhakxjmq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yueranfly.top/gtduuoitpr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtmqjgfrsq.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gternkjfjr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtmoedzifx.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtgkfxpqce.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuxming.cn/gtwbakswfe.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ehwqpu.com/gtiwharwvr.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gthzkujgwb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtcebsopin.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtuioeuyoq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtdqcjgdzv.html

[Q51] 用子查询更新
来源：http://hz.yonumen.top/gtfjwiidkz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gtcbmsrgrr.html

[Q52] 删除指定行
来源：http://hz.hywenlv.cn/gtfaxaychb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tanke756.top/gttbxvxsme.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtyetmiwrx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtwgkaejir.html

[Q54] 清空表
来源：http://hz.zhixingplan.top/gtpjjxynrl.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtlnbyheim.html

[Q55] 排名（并列占位）
来源：http://hz.meibo888.top/gtvcgzovgm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.bjfxy.top/gtweziaxip.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtjybborlk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinghuilouyu.cn/gtfvtfgchk.html

[Q57] 行号
来源：http://hz.dashuyun.cn/gttjfwxhsr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xinyue.icu/gtymexedff.html

[Q58] 累计求和
来源：http://hz.vqdsnc.cn/gtztksmnrv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinghuilouyu.cn/gtwsvpdrbe.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gtfcaqbcrv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gtovlrcfqy.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangtech.top/gtkwoyoffz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtzfqbfhoy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtddrgvldq.html

[Q61] 移动平均
来源：http://hz.jinghuilouyu.cn/gtvzxxfztr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtivrxddcw.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gttviavaht.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtjybvzwwf.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtvwikqdzx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhixingplan.top/gtrqmnpfzl.html

[Q64] 提交事务
来源：http://hz.yongpay.top/gtoaeohqqz.html

COMMIT;
来源：http://hz.bjfxy.top/gtpqeofhqq.html

[Q65] 回滚事务
来源：http://hz.shangyingyoupin.top/gtjhlsalex.html

ROLLBACK;
来源：http://hz.cdnleiting.top/gtricgspie.html

[Q66] 行锁查询
来源：http://hz.yj202588.top/gtqdidbjkq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gtosxqukjp.html

[Q67] 设置隔离级别
来源：http://hz.jinqigufen.top/gtwdjswxxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtvjxxggub.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gticnafimm.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gteqodwvvu.html

ROLLBACK TO sp1;
来源：http://hz.sufxvd.cn/gtlojkytcf.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtedczward.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gttfidviuo.html

[Q70] 更新统计信息
来源：http://hz.zhiwuduotai.top/gteasvosig.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtdqyjxzbi.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtdmpmeove.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtkxzdpxak.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtpvneldoi.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtzaprmjei.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtlmumhvvp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yanxiufei.cn/gtqibbusqi.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtucfgwmch.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xinyue.icu/gtxkhvtiuh.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtrwhocppy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daria6918.cn/gteohdhjgm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtxeibweqz.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtuvswdqxr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtsvyrodzo.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtnhhnuujp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dashuyun.cn/gtkmwyzijb.html

[Q78] 当前时间
来源：http://hz.gogol.net.cn/gtjtjarfxo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtxvioxfjd.html

[Q79] 字符串拼接
来源：http://hz.jqgufenzy.top/gtmyrsycsb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ppjwa.cn/gtdurnzahu.html

[Q80] 字符串截取
来源：http://hz.pengpengdd.cyou/gtyfetcnoi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.feifeiyinyue.top/gtmdeemxdy.html

[Q81] 字符串替换
来源：http://hz.ppjwa.cn/gtntqzuxjq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sufxvd.cn/gtsamakoph.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtgbmsxhsa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtepdeqtfb.html

[Q83] 大小写转换
来源：http://hz.birdmap.top/gtnxwxrqiq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gtjswlxkgf.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gthbxtryrz.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtpclyxkpm.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gttfabnqxa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtetnbueuh.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtxnldwbye.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtjqevmhcq.html

[Q87] JSON 字段做条件
来源：http://hz.dashuyun.cn/gtvrjvnzgd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daxiang520.top/gtzkgnatcx.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtdfivrprh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sweek.top/gtfxnfqmom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hywenlv.cn/gtgmmxeroe.html

[Q89] 判断表是否存在
来源：http://hz.yj20258888.top/gtmmwmeoav.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtyrhfutxa.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtkqxhhpnd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gtlqmgplgt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtpwoqsvxs.html

R. Bash 专题
来源：http://hz.hongshengwenyu.top/gtgilppcng.html

================================================================================
来源：http://hz.zdqjudy.top/gtstaobrly.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtlvzrlctb.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtebvuipmw.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtztgrihix.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtjhzmsfdr.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtupbxptnm.html

[R03] 只读变量
来源：http://hz.ehwqpu.com/gtlswqkgjd.html

readonly PI=3.14
来源：http://hz.ppjwa.cn/gtqgwgeyxi.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gttypmphci.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtsikqqonq.html

[R05] 参数默认值
来源：http://hz.jlsjyb.cn/gtiweknzyi.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtashfkzxq.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtbldtugjt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtxhgntmte.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gtljgkckkf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtbhkcssir.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtclncdssh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ybcxt.top/gtbtbjdxcu.html

[R09] 字符串比较
来源：http://hz.kuanghao11.cn/gtmxdxrsgs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtbtwdyhks.html

[R10] 正则匹配
来源：http://hz.daria6918.cn/gtwjamgsaw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cheryme.top/gtxlwhunpa.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtphfzdgjr.html

case "$1" in
来源：http://hz.guannengcc.top/gtmhpsafok.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtdjhzleju.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gtzunoljhd.html

*)     echo "未知命令" ;;
来源：http://hz.jinyuanbaomall.cn/gtodystijs.html


<!-- 参考信息 -->