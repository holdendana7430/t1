代发 wailian999

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtnntopjfn.html

Py:   str(uuid.uuid4())
来源：http://hz.guannengcc.top/gtpynjuvyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pengpengdd.cyou/gthrmvzdjs.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtvrvbffhs.html

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtkuyfqfwq.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtzlddpeuw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fengsongda.top/gtmdqdbdev.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtscgoqzrn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtiqmmtiyw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhiwuduotai.top/gtxaaialjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtwumwqlxb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haohaochexian.top/gtsmsbqino.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtokbjugsk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.dianchejie.cn/gtfbmhcbgf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtlqqqdxjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtjexvmsgx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangtech.top/gtefkdkrfh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtqgsrfiob.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtfcuqbpki.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtmltianyo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hammf.cn/gtrgfgztai.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtimblginf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtywymwcxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.birdmap.top/gtbxssurjp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pengpengdd.cyou/gtjukaapyn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guowangkeji.top/gtfzehrsyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtcxqlrnmf.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtmqclpdck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cucudq.cn/gtopywsavd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtmlpreyip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtsealbcty.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtysebxnti.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258.top/gtklunhzsh.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gtffbswxzr.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtzpenjbjo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuanzhike.top/gtypoyoxrj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgfzy.top/gtnpxzdvwj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenzaomai.com/gtztyjeriw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtugnronir.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtwpxvekip.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtkbsutmwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnxiangtu.top/gtsjuzjwih.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.9152youxi.cn/gtvyggzhow.html

Ruby: a == b
来源：http://hz.jqgufenzy.top/gtzzbkpcgz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gtayiheqvp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gttlegjtjt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.meibo888.top/gtxghrzjlp.html

PHP:  if (empty($x)) {}
来源：http://hz.jinghuilouyu.cn/gtpngjezuo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gtmfmunkuc.html

TS:   if (x == null) {}
来源：http://hz.jinqigfzy.top/gtcugejitl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hfpthk.cn/gtswdcmdrn.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtntifwiti.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.daria6918.cn/gtxpykensz.html

C#:   if (x is null) {}
来源：http://hz.chenzaomai.com/gtopqhisie.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gttmkroanv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtgpnxtlip.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtskcbspyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hysaishi.cn/gtpfshriiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtbgpwfmkn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtndhldlhu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhiwuduotai.top/gtbhzijaze.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtrwjhomzp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtuzmlukov.html

[P08] 处理浮点精度问题
来源：http://hz.pycfn.com/gtedoplgtb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cashguo.top/gtfoujtqom.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtcwwyjoly.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuanzhike.top/gtpiinrfmm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.vqdsnc.cn/gtvuoksiku.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gtrkmtwapv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtrishxmhx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yuanzhike.top/gtyhoqncrx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xziqi.cn/gtglrpqeox.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtsxeimnrv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtxlhckyfv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtikexqdoj.html

[Q01] 创建表
来源：http://hz.xingfuxueyuan.xyz/gtftmuqucz.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gttashehrm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtmtdqtmea.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtehiyukja.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtphcvyjfa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtmftaytas.html

);
来源：http://hz.jqgfzy.top/gtvjwahncq.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gttsjiwkcq.html

CREATE TABLE orders (
来源：http://hz.hnxiangtu.top/gtyhptxzze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtduxivbes.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtcpzjljgb.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtzyyrelum.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtdjnfarth.html

);
来源：http://hz.meibo888.top/gtvleyfmwc.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtgqesqxom.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtzvocgboc.html

[Q04] 修改列类型
来源：http://hz.bjfxy.top/gtojpiotiy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gtakudrynv.html

[Q05] 重命名列
来源：http://hz.kuanghao11.cn/gtrwipwelb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhiwuduotai.top/gtxbnrpxkq.html

[Q06] 删除列
来源：http://hz.zhiwuduotai.top/gtybgrxrpt.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtiqiuwbwq.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtwvabtebk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtmrpnbhgx.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gtzvqursui.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gttmftpzny.html

[Q09] 创建唯一索引
来源：http://hz.jiagoushi.top/gtooayiafz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtfiebidhl.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gtabqgwuwz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtpzqjugok.html

[Q11] 一次插入多行
来源：http://hz.andypj.xyz/gtmbqqqqry.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.316326.xyz/gtxszpcxit.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gtjjwdxcdg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gogol.net.cn/gtuevimvzl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtbdkdgjhg.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtoqdwlqoh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gtrbbtjafo.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtmdisvxud.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.haohaochexian.top/gtgiuxtnat.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daria6918.cn/gtgpqgikvt.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtprlmdhxi.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtqruyixtg.html

[Q16] 查询指定列
来源：http://hz.0kj1m.cn/gtfhedwcfl.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtifpiweoa.html

[Q17] 条件查询
来源：http://hz.hfpthk.cn/gtzoahgwkx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.aizwys.cn/gtxodpetox.html

[Q18] 模糊匹配
来源：http://hz.cqqwz.cn/gtdnyoymkb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtnvzsalet.html

[Q19] 范围查询
来源：http://hz.birdmap.top/gtyjebfomt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtnszwevkw.html

[Q20] IN 列表
来源：http://hz.fzhhl.top/gthmyufmbi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnqzz.top/gtanzyftzs.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtfctxwfkx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtmzecmxao.html

[Q22] 排序
来源：http://hz.havefunace.top/gtofzvdndk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hywenlv.cn/gtoeksanvh.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtykkxenih.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zycfv.cn/gteoybbzaw.html

[Q24] 去重
来源：http://hz.tianlin.xyz/gtwwilnepn.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtxxemkrfn.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gttfdtldrl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinyuanbaomall.cn/gtscqwfgmg.html

[Q26] 计数
来源：http://hz.gzhubu.top/gtupmkcfru.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtoqdptenz.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gtogqvcisu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtfsmfhdvr.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtlaitncqp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gturzkjknb.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtszcbhrie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtzttefthc.html

[Q30] 分组统计
来源：http://hz.yuanzhike.top/gtshpzlqnt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtioxmfgdn.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtilgvgdza.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.havefunace.top/gtshyyzntu.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtjsgyqhpy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtmjaerazm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtbynlrmky.html

[Q33] 多列分组
来源：http://hz.smart0.xyz/gtrgnxqvlf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.meibo888.top/gtykkdmome.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtiarxyfku.html

SELECT * FROM (
来源：http://hz.ivvv.top/gtkmpklwwe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtemcqwdfl.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gtmuurntcs.html

[Q35] 内连接
来源：http://hz.yuanzhike.top/gtelvaaqov.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtjonlbvae.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtlnfzkvkd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtqeejyifc.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtivtfvxct.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtvycndmmn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtlxwnbhbw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtalyhhdku.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gticvviebf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtapuxtaiy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gttvwzwyag.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtclhmjjhr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnxiangtu.top/gtneljnhfm.html

[Q41] 多表连接
来源：http://hz.xingfuxueyuan.xyz/gtlokbwlmb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhongyouzk.top/gtwxgmkolb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gtejsdxdxc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ehwqpu.com/gtrljvgrtu.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtumkibjap.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtomsgvtdl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangkeji.top/gtaadzarcx.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtlywyrnax.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtgoxqswen.html

[Q44] IN 子查询
来源：http://hz.zhengqikj.top/gtjhxokkcx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jyoumei.cn/gtdfxcnvci.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gttztqnbjb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sufxvd.cn/gtbkwezdri.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtknhdueum.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtybbfrlbh.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtzcicwrnx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ppjwa.cn/gthvcsqfkm.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gtscvrfynw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhaomingkeji.xyz/gtsjmmargx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dashuyun.cn/gtpsqgcxpa.html

[Q49] 更新单行
来源：http://hz.tianlin.xyz/gtuibnghnn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hywenlv.cn/gtbrvyhqop.html

[Q50] 批量更新
来源：http://hz.kuanghao11.cn/gtlvtkglcu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xinyue.icu/gtbolkbhgj.html

[Q51] 用子查询更新
来源：http://hz.hnxiangtu.top/gtiamcwxhx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtdilvbqlx.html

[Q52] 删除指定行
来源：http://hz.xinyue.icu/gtvpagfzhk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenzaomai.com/gtotpvdqin.html

[Q53] 按条件删除
来源：http://hz.meibo888.top/gtinfrtngv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtuqzbmmvq.html

[Q54] 清空表
来源：http://hz.jinqigufen.top/gtscguokfz.html

TRUNCATE TABLE logs;
来源：http://hz.pycfn.com/gtprahavrf.html

[Q55] 排名（并列占位）
来源：http://hz.xziqi.cn/gtthzksalf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sysykeji.top/gtyrrbysor.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtbnqlsdji.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.andypj.xyz/gtavefbhvh.html

[Q57] 行号
来源：http://hz.shzxlz.cn/gteouvdcki.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.meibo888.top/gtjifbeoww.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gthmipbywv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gtbgsvfykr.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gthxfuyads.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jyoumei.cn/gtcklrwgfg.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gtdsseuiqf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gttmwnnbyt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shangyingyoupin.top/gtpxklqcrw.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtphowlyyo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtilldqfop.html

[Q62] 分组占比
来源：http://hz.jqgfzy.top/gthhvypncl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtudmrqabm.html

[Q63] 开启事务
来源：http://hz.shanyushiyangkeji.top/gtxiyuxyfo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtukjqqaej.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtkeclssbo.html

COMMIT;
来源：http://hz.yuxming.cn/gtdfegyqrq.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtjwsfbpnc.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtpvomgtjl.html

[Q66] 行锁查询
来源：http://hz.52xcode.cn/gtlqevspjv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tianlin.xyz/gtzgjnuvpe.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtmmabpulm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtzrqwxlfm.html

[Q68] 保存点
来源：http://hz.daxiang520.top/gtaclhjqqn.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtrfbivupe.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtwxodaqmc.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtktcpstnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtgrtnvurk.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gtuzvgtjzy.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtqzlxxyje.html

[Q71] 查看建表语句
来源：http://hz.jqgufenzy.top/gtkamxggqf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gogol.net.cn/gtpffkzapj.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtpbhztqow.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvznrumyq.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gthequryau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtqlqxpqfl.html

[Q74] 强制使用索引
来源：http://hz.hfpthk.cn/gtdqhfqezq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtcpmbfulg.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtdqlokhoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtvbewmzxv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtfvdnsosq.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtgsxqdusp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtyqjggmnc.html

[Q77] 时间加减
来源：http://hz.smart0.xyz/gtnfkcybws.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtyldsusmf.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtbfkgeleq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tian-w.cn/gtxyvlmwvu.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtedhndnml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sysykeji.top/gtkswutwqn.html

[Q80] 字符串截取
来源：http://hz.nanxinkj.top/gtorrmapwx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.aizwys.cn/gtxxmtpqra.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtdpbtaaje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fzhhl.top/gtzjdjskui.html

[Q82] 字符长度与字节长度
来源：http://hz.zhoulong.xyz/gtfcjprsdy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtbppqovqn.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtzswjkjuu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gthwoshylv.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtxzocdwjg.html

SELECT TRIM(name) FROM users;
来源：http://hz.haohaochexian.top/gtebmmxrvr.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gthvbmfpox.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtyhqbfogm.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtkjehehyl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tianlin.xyz/gtiesemurm.html

[Q87] JSON 字段做条件
来源：http://hz.fzhhl.top/gtxaduxkjw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gthbzbvkvm.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gttzxrttwk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ywan-chungtsiang.top/gtnbyicpou.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtylfsxmtq.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtnchtqihx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jianghu66.top/gtxeuqkbey.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtgvgchkay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtnapiuegb.html

================================================================================
来源：http://hz.meibo888.top/gtwbxdptkf.html

R. Bash 专题
来源：http://hz.tanke756.top/gtoblczbuf.html

================================================================================
来源：http://hz.zdqjudy.top/gtdhrtjybr.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtzoyyxwvv.html

#!/usr/bin/env bash
来源：http://hz.jyoumei.cn/gtaxuhkoxb.html

set -euo pipefail
来源：http://hz.nwbrower.top/gthvrhmrxv.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtelsqwonw.html

name="Tom"; echo "$name"
来源：http://hz.jianghu66.top/gtynnifdua.html

[R03] 只读变量
来源：http://hz.meibo888.top/gtrppjndfw.html

readonly PI=3.14
来源：http://hz.kuanghao11.cn/gtbtwtihgr.html

[R04] 位置参数
来源：http://hz.jinqigfzy.top/gtdpefbijj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtcdemopcc.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gttynvwllh.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtrfobleyt.html

[R06] 判断命令是否存在
来源：http://hz.guannengcc.top/gtometsnsq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhengqikj.top/gteyernqcp.html

[R07] if 判断文件
来源：http://hz.yueranfly.top/gtyyzcwpnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.redwolf501.top/gtczqqjech.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtgxjgftvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hnqzz.top/gtepcaugup.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtyrcwqzzp.html


<!-- 参考信息 -->