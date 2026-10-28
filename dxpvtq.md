代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtwmbxjgnf.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtwtshwutp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.dianchejie.cn/gtbrutpcag.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtadnbonuy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtxcxsziyz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtbyklnpvo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtyukjokwc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtgpytxipo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gthppvwelh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtvqjqdgfa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigufen.top/gtcwobgjwr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.vqdsnc.cn/gttzcnclkp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ybcxt.top/gtioalryqi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangdashe.top/gtzytgxgam.html

[P03] 生成短随机字符串
来源：http://hz.wangdashe.top/gtcewdbdeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guowangkeji.top/gtbsiwlsnj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xingfuxueyuan.xyz/gtvabvqqxl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtnvrzfisu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.52xcode.cn/gtrjsefuzm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gtnmgedaqe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtqfyokeom.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.vqdsnc.cn/gtgxlmqiqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtplsoszmv.html

[P04] 求长度
来源：http://hz.cheryme.top/gtpouhzxga.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.c1oappe.top/gttofeuxey.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtbgfykfmh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtiempzdtb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jiagoushi.top/gtbctubvqw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtgvvpwdzo.html

Go:   len(arr);  len(m)
来源：http://hz.ydzc1.top/gtxipgumzq.html

Ruby: x.length;  x.size
来源：http://hz.mhx1999.top/gtdjkeauyx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gtwxebskqg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuxming.cn/gtufztkyjb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shuidangran.top/gtqitgfivz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jianghu66.top/gtynlckutz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtxxuirbbk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtkgymkhef.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ybcxt.top/gtmttkwsrp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gttojypcnv.html

Ruby: a == b
来源：http://hz.cashguo.top/gtnxebukzk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.fzhhl.top/gtlorcjbmj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtasuellid.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nwbrower.top/gtwuaqyygv.html

PHP:  if (empty($x)) {}
来源：http://hz.zhijiandao.cn/gtukyxjzsj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xuetiantiany.cn/gtqhszlkzm.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtijmaqkbo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtaamybskk.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtmktkevns.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinghuilouyu.cn/gtkqdlgyzz.html

C#:   if (x is null) {}
来源：http://hz.gaohongyu789.top/gtcbutyruz.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gtohwbslop.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhixingplan.top/gtgcpsyazt.html

PHP:  // 手写时间戳比较
来源：http://hz.andypj.xyz/gtkogpanxo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtwolwxcfb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtmmidevqu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtiakhsinm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtzofcfpft.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.havefunace.top/gtrpnkgpxk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gtngndhqha.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gthwttdqkj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtqipggknw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtvqpiggco.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenjidiqi.icu/gtsxgmyrlb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenzaomai.com/gtvippkxfu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtgefmcjqk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgfzy.top/gtnruoibsm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gtgbiknwda.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gthrdjhgnn.html

================================================================================
来源：http://hz.guowangkeji.top/gtuojnhskf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtpzlwqxnd.html

================================================================================
来源：http://hz.zhijiandao.cn/gtggrbrkgj.html

[Q01] 创建表
来源：http://hz.kuanghao11.cn/gtqkjbwuur.html

CREATE TABLE users (
来源：http://hz.yanxiufei.cn/gtdxdbunur.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fengsongda.top/gtncekcmej.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtvnttpdmd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtoviotrjv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtbpbkaiwd.html

);
来源：http://hz.yj202588.top/gtauyuavnw.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gtcnkcsukr.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtiwmoqdhj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtutdmzpdx.html

user_id INT NOT NULL,
来源：http://hz.316326.xyz/gtwtfzvnng.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtwnsmqvev.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dianchejie.cn/gtlyoqubic.html

);
来源：http://hz.tanke756.top/gtoxpsshro.html

[Q03] 增加列
来源：http://hz.redwolf501.top/gtqwxymtxw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtvjmadssp.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtyazzidws.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtmsquxyiv.html

[Q05] 重命名列
来源：http://hz.yj20258888.top/gtimotizka.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.birdmap.top/gtifmiqkew.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtyougcgbg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gttjyieato.html

[Q07] 删除表
来源：http://hz.smart0.xyz/gterlwloqo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gtwvnqsnkd.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtvabmgwtl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.0kj1m.cn/gtxwocabax.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtyrvfxons.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtgqdjlzpf.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtwkqfjveo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtcvybdacy.html

[Q11] 一次插入多行
来源：http://hz.yueranfly.top/gtdynlgifl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtenwiavmx.html

[Q12] 插入后取自增 ID
来源：http://hz.jianghu66.top/gtxuorufwt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtfamfhkjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sxryk.cn/gtggazjdug.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtklufswvp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.vqdsnc.cn/gtpjfrlgab.html

[Q14] 存在则更新（upsert）
来源：http://hz.jyoumei.cn/gtuwkgjimk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guannengcc.top/gtzvbfnymq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yueranfly.top/gtlrxammrg.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtbutmuoef.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtqedwjhek.html

[Q16] 查询指定列
来源：http://hz.316326.xyz/gtozuabefc.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtmdwgyput.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtbznjgspx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtfmumkxzh.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtxvjsnvzf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yanxiufei.cn/gtjxlgkcoy.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtzbueqlrl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtuxytzvyl.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtrcdfhqyi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtvmkshzer.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtdvwdafdh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.quarkkingdee.top/gtrvgrtuur.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtmxnumhuu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtiwumzvgb.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtarzqeikx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yj20258888.top/gtlkihaobk.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtevtcufcd.html

SELECT DISTINCT city FROM users;
来源：http://hz.yangfankeji.com/gtslnaehxl.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gtlzhpkpri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ywan-chungtsiang.top/gtbsbtamdi.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtlprzyqhu.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gthmvazsea.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtyblvuurn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtgykcnnfp.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gthanujfcu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yueranfly.top/gthhffqteu.html

[Q29] 最大最小值
来源：http://hz.tanke756.top/gtboywkaev.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guowangkeji.top/gthbxhstns.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtojrgkudz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtkecrjssx.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtizitlxyr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangkeji.top/gtqodnaqmn.html

[Q32] 分组拼接字符串
来源：http://hz.yvedp.cn/gtbepifbvl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtkymtrmsy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtichnusih.html

[Q33] 多列分组
来源：http://hz.yangfankeji.com/gtmbplqwos.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtyukbdybi.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtkfsyinyx.html

SELECT * FROM (
来源：http://hz.andypj.xyz/gtlecxemvw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhongyouzk.top/gtyqlktejk.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtkgkdsvne.html

[Q35] 内连接
来源：http://hz.yuanzhike.top/gtflnmspjg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtmcswakfp.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtcjlfreti.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtacxihwrr.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtchifebkd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtssuzqqce.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gtkfyafsbb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.redwolf501.top/gtvjwqjwfi.html

[Q39] 自连接（查上下级）
来源：http://hz.316326.xyz/gtkfqcjbfs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gthrkkfvtu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cdnleiting.top/gtmvuywwbw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtfxpvymfc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.bjfxy.top/gtjhddvapu.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtjtqhgqob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtbmiydtal.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtnqrhddno.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cqqwz.cn/gthcjwasxj.html

[Q42] 连接条件附加过滤
来源：http://hz.dianchejie.cn/gtiqdqafgf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtrtsdqyox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gtpyuulcpq.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gttfwwiexj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuxming.cn/gtvhcvmllw.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtghgpzttc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhijiandao.cn/gtrxqaopgf.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtslvfdftu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtsficrtna.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sxryk.cn/gtbacdboxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtmltxgikv.html

[Q47] 与平均值比较
来源：http://hz.yangfankeji.com/gtpmbojkjg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hongshengwenyu.top/gtvejgiljx.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gthayidvoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtdipowmtc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xziqi.cn/gtfwbkbsmh.html

[Q49] 更新单行
来源：http://hz.xziqi.cn/gtxbhszyzh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhongyouzk.top/gtiqoonbar.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gtynzdjqai.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gthlsoanqs.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtyghwhoez.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guannengcc.top/gtmqukfzda.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtzbdwgpie.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtmpdzwouc.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtxwfefbdc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pengpengdd.cyou/gtjvwjctmq.html

[Q54] 清空表
来源：http://hz.yj202588.top/gtihxsgbzr.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtjetwstyf.html

[Q55] 排名（并列占位）
来源：http://hz.andypj.xyz/gtanfiospf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenjidiqi.icu/gtreajfwld.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fzhhl.top/gtxypqtids.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gttikqvksk.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtsfxnazkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtkfovzwmq.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtgorzduuo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cashguo.top/gtrnizcrxx.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gtbrclgwxg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtxycsdgjd.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gthhvnnuzy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhengqikj.top/gtcgornbvo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtyrrbhple.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtgiwiagyz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtaqjzkhvn.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtnxigpcep.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtwkdivasv.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtjjpyegam.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yangfankeji.com/gtssymbjqy.html

[Q64] 提交事务
来源：http://hz.hfpthk.cn/gtsjbebyze.html

COMMIT;
来源：http://hz.bjfxy.top/gtfgntoyok.html

[Q65] 回滚事务
来源：http://hz.quarkkingdee.top/gtlygbowtn.html

ROLLBACK;
来源：http://hz.shuidangran.top/gtjrasdaec.html

[Q66] 行锁查询
来源：http://hz.tianlin.xyz/gtlzmrsrzc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.meibo888.top/gtvxbpvssv.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtuvmztpfq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tianlin.xyz/gtnropkepz.html

[Q68] 保存点
来源：http://hz.nanxinkj.top/gtrcwxrckf.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtnwcoktzg.html

ROLLBACK TO sp1;
来源：http://hz.yj202588.top/gtvipfurva.html

[Q69] 查看执行计划
来源：http://hz.jinqigufen.top/gtwytcwpud.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtdyhfrchi.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtjuezoqds.html

ANALYZE TABLE users;
来源：http://hz.quarkkingdee.top/gtiefsqmwh.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtytggxebl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtvkgpcuvj.html

[Q72] 查看索引
来源：http://hz.316326.xyz/gtnypoumig.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtzbxuajlb.html

[Q73] 查看表状态
来源：http://hz.haohaochexian.top/gtvtpjtfnr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tanke756.top/gteyylqtxg.html

[Q74] 强制使用索引
来源：http://hz.zhengqikj.top/gtkkztnkxu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtbrmkvfsr.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtfrhtcoyv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gtqazdtdwa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daria6918.cn/gtiysroads.html

[Q76] 按天统计
来源：http://hz.jinqigufen.top/gtwcwjraop.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtxzpixmdl.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gtqnbfptib.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtrhhifoys.html

[Q78] 当前时间
来源：http://hz.ybcxt.top/gtxogxeabo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtntgndzhy.html

[Q79] 字符串拼接
来源：http://hz.snrcjt.cn/gtskgtwrcs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtklrajjgk.html

[Q80] 字符串截取
来源：http://hz.wangdashe.top/gttlitopaw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtrjxkpnem.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtvengmuoe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtbghitjgo.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtnnekxkmg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtxuizozhq.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtqtdhsfcm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtwjsmpcgf.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtshkudzay.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtwxsfcukl.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gtiheqohlb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.havefunace.top/gtapgqmqnp.html

[Q86] 读取 JSON 字段
来源：http://hz.jiagoushi.top/gthsmswtsu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gttrfnpkac.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gtowkuufqs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtwhsfldqh.html

[Q88] 行转列（条件聚合）
来源：http://hz.redwolf501.top/gtklwlndtm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgufenzy.top/gtzzlpwxqb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gtfgrajuzv.html

[Q89] 判断表是否存在
来源：http://hz.hammf.cn/gtxhmioulv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hnxiangtu.top/gtndterrvu.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gttutwqxha.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinyuanbaomall.cn/gtdmplqhxo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrwpqjejy.html

R. Bash 专题
来源：http://hz.havefunace.top/gtheychsfg.html

================================================================================
来源：http://hz.jyoumei.cn/gtyeddmhag.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtjnrkkrqv.html

#!/usr/bin/env bash
来源：http://hz.jinyuanbaomall.cn/gtoapsgeyp.html

set -euo pipefail
来源：http://hz.yueranfly.top/gtutdirwoq.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gtjdlalcki.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gtbzruxuae.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gtimdkjkej.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtyegvxxai.html

[R04] 位置参数
来源：http://hz.tianlin.xyz/gtpahkoxjm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gthzmwrgph.html

[R05] 参数默认值
来源：http://hz.shanyushiyangkeji.top/gtthmxfkbd.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtkzqpxyob.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtrfhveaqy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tian-w.cn/gtlkqwqinl.html

[R07] if 判断文件
来源：http://hz.daxiang520.top/gtueqquqky.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fengsongda.top/gtfrbrrzla.html

[R08] 数值比较
来源：http://hz.daxiang520.top/gtdtriotxc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.feifeiyinyue.top/gtphwkfwab.html

[R09] 字符串比较
来源：http://hz.zhaomingkeji.xyz/gtvcrcktro.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtwkggtmyd.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtzrskohqx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtgyfpuxch.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gthasejfif.html


<!-- 参考信息 -->