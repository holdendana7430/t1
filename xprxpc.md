代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtzkaxcvkh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuetiantiany.cn/gtiuxevizr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtjzngvzpr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gttnsmtsvh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pycfn.com/gtrxmmhtks.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtpbpgxtmg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.pengpengdd.cyou/gtwcaiaxad.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fengsongda.top/gtrmwqjctv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtzcfdzhbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtfcgykora.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtxiytojgr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigufen.top/gtuhxswtpa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtxwlswiib.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtraquisnh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtqflhkkap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtescbtdqf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinyuanbaomall.cn/gtnbamcgrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtszxwkutp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gtdwocclwy.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtlclelssk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.meibo888.top/gtfmzrxeng.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtczgqlcya.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtbohkvjke.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtfojcxhij.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinghuilouyu.cn/gtcbxshivt.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangkeji.top/gtwnhzacoo.html

Ruby: x.length;  x.size
来源：http://hz.hammf.cn/gtimvslwyf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yonumen.top/gtwipbhgeb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gthbgrusoe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.guowangkeji.top/gtcolanjrg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtoooqviae.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtgkwpgjrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtlmyrfqkr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xuetiantiany.cn/gtedifdjup.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtosrfetzz.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtxlctgtgk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gttioscskq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtcmwpfzhx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dashuyun.cn/gtiwrxrwvn.html

PHP:  if (empty($x)) {}
来源：http://hz.yuanzhike.top/gtcbbtseex.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zycfv.cn/gttoubikre.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtpipwgtoy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtifggkfgr.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangtech.top/gtzpnbtjou.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gttlhgcluy.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtmsfiqkhi.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gtozdfcpij.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.havefunace.top/gtopwmexqx.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtrovfzvqe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtsaoqfysb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtkjuoivop.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtpxfjiaus.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtiaxzughs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtcpzkueda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hysaishi.cn/gtpbegcerb.html

[P08] 处理浮点精度问题
来源：http://hz.yangfankeji.com/gtrxpnrwfx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xuanzx.com/gtzvvuajfr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtpwlbpxix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhaomingkeji.xyz/gtyumikiiz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gttadfuwcq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gtkyfmsscx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigufen.top/gtwfzlhjqb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtnvmycvoz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.birdmap.top/gtjhsimpkw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtiyfafyix.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtzrocpzgn.html

================================================================================
来源：http://hz.yonumen.top/gtxopteghf.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtsrgahnrg.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtodkehtpc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtteddehng.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxinkj.top/gtqrwbygbf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtcgwdkkdp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gtwcynyiil.html

);
来源：http://hz.smart0.xyz/gtsuptjfbs.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtcmjqmtsz.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtozgsjlco.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtvhevoxya.html

user_id INT NOT NULL,
来源：http://hz.fzhhl.top/gtvogrxkpa.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtrdikopae.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtomwkemgc.html

);
来源：http://hz.52xcode.cn/gtfapbbfnj.html

[Q03] 增加列
来源：http://hz.ehwqpu.com/gtmjpwvree.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtwnmqmdhf.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gteekpkukg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtorgtyjop.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtufbaxlib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jqgfzy.top/gtgycnqkvp.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtbdniyopd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cheryme.top/gtilahnvrh.html

[Q07] 删除表
来源：http://hz.dashuyun.cn/gtsiuiogbr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gtxfdahkwq.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gtutdqxatq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gtllyryqdu.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtudgpvzea.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtytiuxgao.html

[Q10] 插入单行
来源：http://hz.svipenyu.cn/gtksmbxnic.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xziqi.cn/gtkffylkjx.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gtcyylmxmw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.fengsongda.top/gtylnfdcxz.html

[Q12] 插入后取自增 ID
来源：http://hz.xuanzx.com/gtopdyxcnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtmanhgrrj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.mhx1999.top/gteawqjtrm.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtzaqczazz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gttynwxffb.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtjmwnhduj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.mhx1999.top/gtrgzlajnt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtujbzjhjw.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtljsskfny.html

SELECT * FROM users;
来源：http://hz.cashguo.top/gtogtimnkj.html

[Q16] 查询指定列
来源：http://hz.zhengqikj.top/gtkmkekflc.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gttlfamima.html

[Q17] 条件查询
来源：http://hz.gogol.net.cn/gtnlqaethi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.snrcjt.cn/gtxwxdteqz.html

[Q18] 模糊匹配
来源：http://hz.andypj.xyz/gttasvcfyb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hongshengwenyu.top/gtknhbitth.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtiwuvsewd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ivvv.top/gtmhgmmsdl.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtxreqmktg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtaxqrspit.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtvywvqiki.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtuuaekony.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtzydlxxoi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtmgvrtmfj.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtuqwmcmcp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sweek.top/gtqunknazl.html

[Q24] 去重
来源：http://hz.0kj1m.cn/gtahceijoq.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gtbdckukxe.html

[Q25] 只取前 N 条
来源：http://hz.9152youxi.cn/gtbknzheez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtdjnlihjj.html

[Q26] 计数
来源：http://hz.smart0.xyz/gtkvfvrqmh.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenzaomai.com/gtyqgkjdnc.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtuxlfxtfe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yonumen.top/gtszfmgkaf.html

[Q28] 求和与平均
来源：http://hz.jinqigufen.top/gtawkyjkyf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtuymycyky.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtjelqqnvz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.wangdashe.top/gtrxuhubgg.html

[Q30] 分组统计
来源：http://hz.daria6918.cn/gtfxsijhwh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtibnzdhrs.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtucnrddky.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.svipenyu.cn/gtnotqnzad.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtxsfuquxs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtyfhxprsw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtosqzhuem.html

[Q33] 多列分组
来源：http://hz.52xcode.cn/gtkprtjtvs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtavmfiksx.html

[Q34] 每组取第一条
来源：http://hz.sufxvd.cn/gttrjwyouu.html

SELECT * FROM (
来源：http://hz.ppjwa.cn/gtikzhfjrd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shanyushiyangkeji.top/gtfidpvnfj.html

) t WHERE rn = 1;
来源：http://hz.sweek.top/gtzmqsoswj.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtxvvrpuby.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hysaishi.cn/gtbkvmcmvy.html

[Q36] 左连接
来源：http://hz.hongshengwenyu.top/gttjahaukm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtenzdhdcy.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtrlrzcxqv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gtsnjsjtuz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.haohaochexian.top/gtnoymnyai.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtjvsqdual.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtzqiqrnfm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cheryme.top/gtgscxszxl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtskmhdzdp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.vqdsnc.cn/gtjtngpvjj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.c1oappe.top/gtejakurcm.html

[Q41] 多表连接
来源：http://hz.pycfn.com/gtofcemqkg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtewajpkhp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zycfv.cn/gtsitzirzp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtkrqxqmat.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtwoljkuvn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.52xcode.cn/gtrupljxxw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtzuadbrbr.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtgxbxyluz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtuszkjivs.html

[Q44] IN 子查询
来源：http://hz.tanke756.top/gtjzuirxth.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtiiqeyvaw.html

[Q45] EXISTS 判断存在
来源：http://hz.gogol.net.cn/gtwqvlvdok.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtrcjgphig.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gtwwevmxjr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigfzy.top/gtgchelajs.html

[Q47] 与平均值比较
来源：http://hz.cheryme.top/gttwsejeyk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhixingplan.top/gthoujaatq.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtfgfwxnzx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gtfvgebsqx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zdqjudy.top/gtfyxndafx.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtljtqczww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtsicwaufr.html

[Q50] 批量更新
来源：http://hz.xinyue.icu/gtfnmiwwvf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenzaomai.com/gtvgejajpo.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtfisdmytk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtkypykcjf.html

[Q52] 删除指定行
来源：http://hz.tanke756.top/gtgplgkpnd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dashuyun.cn/gtfspoqdqi.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtljoqdbui.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtckheufnf.html

[Q54] 清空表
来源：http://hz.yangfankeji.com/gtuqrlgrnu.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtvmwykloe.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gtpbxahjqi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtvxrcoxji.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtfhxtutwc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gtfhdcoyif.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gttybbcsns.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtwdqrevso.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtwzcxaflo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xziqi.cn/gtbxvzqoce.html

[Q59] 分组内累计
来源：http://hz.yanxiufei.cn/gtjgvmhpjj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtdfkjlmif.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtqxhllbvl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shanyushiyangkeji.top/gtjabvarax.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtsadfalns.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtmmdinefe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxinkj.top/gtgcqnlxuz.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtieoqoosv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtmwghhoyp.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gthsujtyau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gotoacloud.top/gtiimmdbgu.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtfopielic.html

COMMIT;
来源：http://hz.jianghu66.top/gtdoabdhno.html

[Q65] 回滚事务
来源：http://hz.zycfv.cn/gtaszryuft.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gtecpzprrn.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtjlrlkjbt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtmqhjaoni.html

[Q67] 设置隔离级别
来源：http://hz.ivvv.top/gtfkmyzwfw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gttjeumvew.html

[Q68] 保存点
来源：http://hz.meibo888.top/gtdjjcwscl.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtgzkhkusz.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtdxpcfwyv.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gtfzxahkce.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtbvtaxxtr.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtoclqmert.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gttpzvneai.html

[Q71] 查看建表语句
来源：http://hz.zdqjudy.top/gtkbzinzdm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtwmmizdda.html

[Q72] 查看索引
来源：http://hz.shzxlz.cn/gtsmgaxgck.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtrhllbkgk.html

[Q73] 查看表状态
来源：http://hz.yvedp.cn/gtwtbdzatz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gthfxxrmnf.html

[Q74] 强制使用索引
来源：http://hz.gogol.net.cn/gtplmebros.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtjfrimifa.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtbcvnnlue.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtqsuftveg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtorgqajdg.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtguexqvyp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtxeamruhe.html

[Q77] 时间加减
来源：http://hz.sufxvd.cn/gtxygaetqm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtcgrlatnd.html

[Q78] 当前时间
来源：http://hz.shanyushiyangtech.top/gtpigytvkg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtytchrpgy.html

[Q79] 字符串拼接
来源：http://hz.52xcode.cn/gtlxdknjcy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xinyue.icu/gtkzhcikpn.html

[Q80] 字符串截取
来源：http://hz.jyoumei.cn/gtatepyhas.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydjk.org.cn/gtgsmvoomo.html

[Q81] 字符串替换
来源：http://hz.jianghu66.top/gtmjuqkcgp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.redwolf501.top/gtcxdyifxt.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gthnwiqsdo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtemnytwyn.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtqsjakzbx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtxeylsjtq.html

[Q84] 去除首尾空格
来源：http://hz.redwolf501.top/gtfiioqqqt.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtzhvsugrq.html

[Q85] 数值取整
来源：http://hz.cashguo.top/gtesqboeyo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtsqothste.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtzaccuifp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtszunxhyo.html

[Q87] JSON 字段做条件
来源：http://hz.wangdashe.top/gtasrwehtv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtktaobgke.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtfswbwnfb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gtruhbiwhg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtfmeikflk.html

[Q89] 判断表是否存在
来源：http://hz.jianghu66.top/gtgppvihua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtwmrsvpvp.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtjiajscux.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtfqhxuqvl.html

================================================================================
来源：http://hz.dianchejie.cn/gtjcxcfekb.html

R. Bash 专题
来源：http://hz.yonumen.top/gtvyeqytpc.html

================================================================================
来源：http://hz.52xcode.cn/gtqnytxxho.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtcopruohr.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtmqdsezht.html

set -euo pipefail
来源：http://hz.wangdashe.top/gtfjzjjfrq.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtacswkwzq.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtczpyacmu.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gttkjhycau.html

readonly PI=3.14
来源：http://hz.0kj1m.cn/gtfflfcvcg.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtnshdxdvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuanzx.com/gttynhqbrg.html

[R05] 参数默认值
来源：http://hz.nanxuanxn.top/gtgmcbmppe.html

name="${1:-default}"
来源：http://hz.snrcjt.cn/gtbfoxzgvf.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtgzrjusha.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhongyouzk.top/gtewsqigpg.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gturigagzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yangfankeji.com/gtclfiiuoy.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtjvsnjyag.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtzjwiizpq.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtcpxyuwny.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtvspqucpl.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtdutmojup.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hywenlv.cn/gtxncppold.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtqkmxczzn.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtyollvjnu.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtcgpreyvu.html

stop)  echo "停止" ;;
来源：http://hz.dianchejie.cn/gtjwsugemg.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtbwocutti.html


<!-- 参考信息 -->