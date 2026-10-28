代发 wailian999

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtczvghjus.html

================================================================================
来源：http://hz.daria6918.cn/gtzokonelj.html

P. 常用工具函数
来源：http://hz.gzhubu.top/gterkfhtmc.html

================================================================================
来源：http://hz.ppjwa.cn/gtapuloxpm.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtqmkhmgtg.html

Py:   str(uuid.uuid4())
来源：http://hz.ivvv.top/gtbkzpxlgf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtamutrfwu.html

JS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtcvypixia.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtiqrtvkvw.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtcxdnpvim.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtoriictpi.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtxuwouzkc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtzcupnqrp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhiwuduotai.top/gtdifthymq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yvedp.cn/gtwvtdpiiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sxryk.cn/gtltemnhgc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhijiandao.cn/gtsncqpsba.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gtbiwzuaxv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gththvlfkd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gtngyclkrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhijiandao.cn/gtvdekbthx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yonumen.top/gtiffmqzqo.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtrvtlkmjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gogol.net.cn/gtgkbjpngj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtqwqcfxae.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtoojtavhh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtaqddyybi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sufxvd.cn/gtkhfakpej.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cheryme.top/gtwgjmjjin.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinqigfzy.top/gtxiccvzgt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtwfptoqdj.html

[P04] 求长度
来源：http://hz.iojbl.cn/gtjbkfksqp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ybcxt.top/gtnrnpzawt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtpnpgpgdv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtkegtyyhp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtmmnlpxqa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtjalfzwbt.html

Go:   len(arr);  len(m)
来源：http://hz.redwolf501.top/gtmrftjdzf.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtuvxzbgmf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtxtvmnfed.html

[P05] 判断两个对象内容是否相等
来源：http://hz.fengsongda.top/gtukylibgm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ppjwa.cn/gtghmvujnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xylfe.cn/gtmoytjkfz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtkxiptrxx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.birdmap.top/gtkzgxnodu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tianlin.xyz/gtomfjblei.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sufxvd.cn/gtbsvjxxgr.html

Ruby: a == b
来源：http://hz.xziqi.cn/gtzdfbltus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yongpay.top/gtaycgruom.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ybcxt.top/gtgacgjhsx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtbgtpbstx.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtskfibzuf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtrpzpkvss.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtjvtkurkz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtjqpzabdu.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtaczvskjb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtdsrgtify.html

C#:   if (x is null) {}
来源：http://hz.yj202588.top/gtfcxrjshn.html

[P07] 防抖与节流
来源：http://hz.zycfv.cn/gtfhyoyhzy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fengsongda.top/gtgkantyrq.html

PHP:  // 手写时间戳比较
来源：http://hz.dashuyun.cn/gtefmmpymf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtpyfqbtnt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtdoyhatkl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gtrsnsxghg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yongpay.top/gtjygvkrax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtcyaqwvic.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenlongwang.top/gtxqgyqysq.html

[P08] 处理浮点精度问题
来源：http://hz.meibo888.top/gtebvxisty.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gtfkorqytx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhoulong.xyz/gtvzyyvqys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtzljlexqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jyoumei.cn/gtzerhjlil.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cucudq.cn/gtjsijaqyg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.andypj.xyz/gtwhbfmvgv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtyeemyoma.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cheryme.top/gtduuftmqz.html

================================================================================
来源：http://hz.zdqjudy.top/gtlhmcmtdk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigfzy.top/gtjtbllqca.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxiylbnwh.html

[Q01] 创建表
来源：http://hz.snrcjt.cn/gtawavrcil.html

CREATE TABLE users (
来源：http://hz.jinyuanbaomall.cn/gtcnofwelf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtpzorqiru.html

name VARCHAR(50) NOT NULL,
来源：http://hz.316326.xyz/gtvuezobcq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtpeleovmy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtnbdvcooa.html

);
来源：http://hz.feifeiyinyue.top/gtnkqpairz.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtswtcoasl.html

CREATE TABLE orders (
来源：http://hz.andypj.xyz/gtpfnofalu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtvoizjjck.html

user_id INT NOT NULL,
来源：http://hz.jinyuanbaomall.cn/gtyfyccosc.html

amount DECIMAL(10, 2),
来源：http://hz.redwolf501.top/gtfxfvoyzc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnqzz.top/gtuveoqldc.html

);
来源：http://hz.nwbrower.top/gtgfnnwhfr.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtebsjffuc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtxopcxhvb.html

[Q04] 修改列类型
来源：http://hz.gaohongyu789.top/gtzxpsyrza.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258888.top/gtyjnptirv.html

[Q05] 重命名列
来源：http://hz.aibaodan.cn/gtgxrmxihc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shzxlz.cn/gtfxmoesgo.html

[Q06] 删除列
来源：http://hz.hysaishi.cn/gtjnzqecbm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtcdjeksux.html

[Q07] 删除表
来源：http://hz.yangfankeji.com/gtsctvoeji.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yangfankeji.com/gtsvebcckq.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtflsbftld.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gthhbixxah.html

[Q09] 创建唯一索引
来源：http://hz.hnxiangtu.top/gtlnkdpokc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtrovulrso.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtfpyfomsa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sweek.top/gteuzpctmb.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtblwapufj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtpjhgqvht.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gtinnbreeo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydjk.org.cn/gtnpawemjw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cashguo.top/gtiqwkahve.html

[Q13] 忽略重复插入
来源：http://hz.gogol.net.cn/gtztahdcrn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gtswprdxxx.html

[Q14] 存在则更新（upsert）
来源：http://hz.fzhhl.top/gtfskrivak.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gthssptwvr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtqohbfbit.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtmibcbjzg.html

SELECT * FROM users;
来源：http://hz.bjfxy.top/gtdamqtdus.html

[Q16] 查询指定列
来源：http://hz.sufxvd.cn/gtpuzxuyzy.html

SELECT id, name FROM users;
来源：http://hz.chenzaomai.com/gttvocjfkh.html

[Q17] 条件查询
来源：http://hz.andypj.xyz/gtxxwwmzju.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cdnleiting.top/gtirqnidpy.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtjzusjuto.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtxdcrqhfj.html

[Q19] 范围查询
来源：http://hz.snrcjt.cn/gtcglhbhnk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtxresyzyo.html

[Q20] IN 列表
来源：http://hz.xingfuxueyuan.xyz/gtnwgjeytw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtaexufetm.html

[Q21] 空值判断
来源：http://hz.yvedp.cn/gtgsrqeftr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.aibaodan.cn/gtfchfqwcf.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtlnrvlbau.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jiagoushi.top/gtygcyreul.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtweuwkgzn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gtbvflpckr.html

[Q24] 去重
来源：http://hz.haohaochexian.top/gtkxddxjuq.html

SELECT DISTINCT city FROM users;
来源：http://hz.hywenlv.cn/gtxpbbyrzn.html

[Q25] 只取前 N 条
来源：http://hz.zdqjudy.top/gtyqtozgci.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gthyggufly.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gteegnuuws.html

SELECT COUNT(*) FROM users;
来源：http://hz.gogol.net.cn/gtjgpmmysl.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gthxcjvkzb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtvuisssyq.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtyprrpsrd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtffusdjym.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtlpuozlah.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtgotzbjhh.html

[Q30] 分组统计
来源：http://hz.sweek.top/gtingctkef.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtyrizdspr.html

[Q31] 分组后过滤
来源：http://hz.hywenlv.cn/gtdmhyfawi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gtxogzgfmo.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtbxynmlck.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gtngpfzrpb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhaomingkeji.xyz/gtimaolvxx.html

[Q33] 多列分组
来源：http://hz.chenzaomai.com/gtfldcxxyz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtikdxbxbk.html

[Q34] 每组取第一条
来源：http://hz.andypj.xyz/gtgqwnxhun.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtrwxbnoqo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gttieoyexk.html

) t WHERE rn = 1;
来源：http://hz.gzhubu.top/gtykjlpnpw.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtxrzajvcc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtghmfmjur.html

[Q36] 左连接
来源：http://hz.cdnleiting.top/gtgshisxqb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhixingplan.top/gtguazyqzr.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtspxskwpz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jiagoushi.top/gthwdbdcym.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnqzz.top/gtdtnjtlqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhengqikj.top/gtyrtszmqv.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtliqqajyz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.sxryk.cn/gtvarrccwk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jlsjyb.cn/gtibvrjajp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.quarkkingdee.top/gtxysrzawr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhaomingkeji.xyz/gtesxuxpjk.html

[Q41] 多表连接
来源：http://hz.zdqjudy.top/gtfjagkaqz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtplcqtvem.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtspeyposk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shuidangran.top/gtqwkfmapv.html

[Q42] 连接条件附加过滤
来源：http://hz.zhengqikj.top/gtdscpjvne.html

SELECT u.name, o.amount FROM users u
来源：http://hz.mhx1999.top/gtpnkegzfo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhengqikj.top/gtcwiksxlg.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtmfppkplz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gteiozgkko.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtukeoewfo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtywcbhatu.html

[Q45] EXISTS 判断存在
来源：http://hz.cdnleiting.top/gtueuxeoex.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtuwkhcvzd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gteskvyhse.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtmormphnm.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gtkrglilck.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xinyue.icu/gtjauqhoqs.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtwjalyffl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtwguitzbr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtwiyupbcq.html

[Q49] 更新单行
来源：http://hz.snrcjt.cn/gttdwjnjez.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtslkzqhzt.html

[Q50] 批量更新
来源：http://hz.fengsongda.top/gtgtivwosi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtrmzfgggi.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtzccqbnlt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guowangkeji.top/gtkfbewots.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtvskwjvss.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtsotoywrp.html

[Q53] 按条件删除
来源：http://hz.nanxinkj.top/gtpdabkrik.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.snrcjt.cn/gtztqxdvxk.html

[Q54] 清空表
来源：http://hz.smart0.xyz/gtopnqccub.html

TRUNCATE TABLE logs;
来源：http://hz.nanxinkj.top/gtneobzerp.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gtdohobqri.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jiagoushi.top/gteoaqhqiq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fzhhl.top/gtokivowwc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tianlin.xyz/gtrnqgbjwy.html

[Q57] 行号
来源：http://hz.yongpay.top/gthrgggxnw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cucudq.cn/gtumxerkyx.html

[Q58] 累计求和
来源：http://hz.gogol.net.cn/gtjoudodxd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtknmosqxz.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gtkvualoxs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtawejgyod.html

[Q60] 取上一行 / 下一行
来源：http://hz.hammf.cn/gtdgpzxvsw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aibaodan.cn/gthdjvzpjg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinghuilouyu.cn/gtbljpklni.html

[Q61] 移动平均
来源：http://hz.wangdashe.top/gtihufaxkz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtxotwidic.html

[Q62] 分组占比
来源：http://hz.jqgfzy.top/gtgemvczln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtdpqgbcgm.html

[Q63] 开启事务
来源：http://hz.yj202588.top/gtfadjsoam.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtsbacnkkb.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtpwcwgolz.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtlhtirova.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gttjthvsau.html

ROLLBACK;
来源：http://hz.316326.xyz/gtldiustdh.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gttslzrcqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtfvdiozsm.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtagnosfkl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yangfankeji.com/gtjaiapbjz.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtdinjvhpl.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtrcqgbark.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtcrwneosp.html

[Q69] 查看执行计划
来源：http://hz.fzhhl.top/gtcyfeafhs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgfzy.top/gtzzzvwtou.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtltsumehe.html

ANALYZE TABLE users;
来源：http://hz.jqgfzy.top/gtjzybwpan.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtxxxqznqi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtdujtztyi.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gttpsjifrt.html

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gttxauirjy.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtfldpoixt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tian-w.cn/gtixahoqal.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtvhasvrdi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guowangkeji.top/gtyibjizll.html

[Q75] 日期格式化
来源：http://hz.sweek.top/gtckxiznny.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtrkxptvnb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258.top/gtsoiqblsr.html

[Q76] 按天统计
来源：http://hz.ppjwa.cn/gtpdwqbbtl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtmejctuuc.html

[Q77] 时间加减
来源：http://hz.sweek.top/gthindpqri.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cucudq.cn/gtdlifkwni.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtwcorprkb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtrgtyzwfc.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtmdholetk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtfbcfactv.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtrfrkkabv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtzjjgzrsd.html

[Q81] 字符串替换
来源：http://hz.aibaodan.cn/gtvzwecyxt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xinyue.icu/gtxowlfvpj.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtuqtueoja.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gthqmadmon.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtorodcjha.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yueranfly.top/gttrututkv.html

[Q84] 去除首尾空格
来源：http://hz.ybcxt.top/gthcjpatna.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gtrpgxpuiw.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtyzzwvvxl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtnjdzshaj.html

[Q86] 读取 JSON 字段
来源：http://hz.jiagoushi.top/gtbqroheip.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yanxiufei.cn/gtklzibmtt.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtaqpokytb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtbpzgnzxk.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtuiuktncd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtxlgkhdys.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtuwjctdng.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtxhlisqem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.mhx1999.top/gtldylhgiy.html

[Q90] 生成序号列
来源：http://hz.zhongyouzk.top/gtecaifcfa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtnvllnyyi.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlzyqekax.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtygmsrytk.html

================================================================================
来源：http://hz.yonumen.top/gtcewjefjb.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtbnzgbinc.html

#!/usr/bin/env bash
来源：http://hz.sufxvd.cn/gttriiuknd.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtjxpcjxhl.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtlmchotqo.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtqbvxlmwq.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtfpflctgm.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtmkmtdezd.html

[R04] 位置参数
来源：http://hz.pengpengdd.cyou/gtocxvvtdr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgfzy.top/gtkhqaypll.html

[R05] 参数默认值
来源：http://hz.yongpay.top/gtwhibepcf.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gthvftjqcj.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtzzilhfya.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cqqwz.cn/gtihipfcxu.html

[R07] if 判断文件
来源：http://hz.meibo888.top/gtiprrzjlg.html


<!-- 参考信息 -->