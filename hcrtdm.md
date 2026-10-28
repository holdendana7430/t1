代发 wailian999

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gthealmcmx.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtnocavvuf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtcnvbpxku.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtzxbrkidf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtdbjcrvbc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtiqisybxy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtsuczanyd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.feifeiyinyue.top/gtrpxdwufz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fzhhl.top/gtrlcqfgqh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtiwknxrba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gttwiuezmi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gticdyhkdk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtouvxqhoh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gtqomrlkgh.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gthgrfoxvr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtqztmeutf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtupjkwdzf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gttbygcygo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenjidiqi.icu/gtimtliogk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtdgamsitq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtjkdpvtbl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yanxiufei.cn/gtsfapvcir.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtglmohhqk.html

[P04] 求长度
来源：http://hz.cucudq.cn/gtrmdhtjrf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtavneelzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtytuimqrl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtlqfjktbr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtimixuaod.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtccjkzytw.html

Go:   len(arr);  len(m)
来源：http://hz.gaohongyu789.top/gtpgimysew.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtdvcetacj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtrysvutin.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtjqutdciu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtzgpavijs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gttirqnjiy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aizwys.cn/gtwatuealr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtdomeymht.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtbniwudqp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gttftrcybo.html

Ruby: a == b
来源：http://hz.shzxlz.cn/gtrrszpgse.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gthbkwzoiz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtefarcezz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yonumen.top/gtojydebme.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gtoypbgncx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtfpjcqcby.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtlzronffo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xziqi.cn/gtmrflxmbi.html

Go:   if x == nil {}
来源：http://hz.zhaomingkeji.xyz/gtvivdzdbe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.havefunace.top/gtzqhhupec.html

C#:   if (x is null) {}
来源：http://hz.zhiwuduotai.top/gtbzjdnxhf.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtebikeqmq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhijiandao.cn/gtumhbqccj.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtpsjkojll.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtpuysmgud.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtkcvoccxm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.aibaodan.cn/gtaxgzycwn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gttjqfvxte.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jinyuanbaomall.cn/gtuvlrdoku.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dashuyun.cn/gtzaazwtju.html

[P08] 处理浮点精度问题
来源：http://hz.birdmap.top/gtkkshkxez.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangtech.top/gtddbcpybz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tian-w.cn/gtpszzyjhn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtzpvjzual.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sweek.top/gtdperetyu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtjompddyt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yuanzhike.top/gtdchxjehf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhiwuduotai.top/gtemokwalz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangshuangyany.cn/gtovwtkhro.html

================================================================================
来源：http://hz.cheryme.top/gtggilpgxt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtujrimcch.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrmfaygnm.html

[Q01] 创建表
来源：http://hz.hfpthk.cn/gttwryaeke.html

CREATE TABLE users (
来源：http://hz.xuanzx.com/gtzzrulrgz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xylfe.cn/gtpbkeayed.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenzaomai.com/gtprrvesdp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cashguo.top/gtekkhvtcb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtcondjuph.html

);
来源：http://hz.ybcxt.top/gtgvflmuwj.html

[Q02] 创建带外键的表
来源：http://hz.hnxiangtu.top/gttiujximn.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangkeji.top/gtldsbsomo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtyxfkampx.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtfagdjdnl.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtkhwighxe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258.top/gtacbeaypn.html

);
来源：http://hz.aizwys.cn/gtojtortkb.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtvbtrorzv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtoylirawc.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gthtagwemk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.wangdashe.top/gtorxjjspc.html

[Q05] 重命名列
来源：http://hz.shzxlz.cn/gtlyvgaadz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.c1oappe.top/gtejfwmdkd.html

[Q06] 删除列
来源：http://hz.sweek.top/gthrssimku.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtyxcbefbz.html

[Q07] 删除表
来源：http://hz.nanxinkj.top/gtcfyspezy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtbddfarwr.html

[Q08] 创建普通索引
来源：http://hz.hammf.cn/gtslehkmuk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.redwolf501.top/gttwicorte.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtkbxmquxf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtzsntdqlq.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtiwpvxoio.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtriyeeqlj.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtcaevxuxg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hfpthk.cn/gtcfevllgt.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtzaetvoku.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtcmwyyljj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yanxiufei.cn/gtczqmatwh.html

[Q13] 忽略重复插入
来源：http://hz.c1oappe.top/gtjqrukdgl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.smart0.xyz/gtnulytsyf.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtowaukiwf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtjdgldiqm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.mhx1999.top/gtytcxitjc.html

[Q15] 查询全部
来源：http://hz.birdmap.top/gtcsspixpw.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtpifvhbfb.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtzesziijw.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtbgrfeyrg.html

[Q17] 条件查询
来源：http://hz.guowangkeji.top/gtdhmxvahx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.52xcode.cn/gtnazykfew.html

[Q18] 模糊匹配
来源：http://hz.0kj1m.cn/gtpmsyswez.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gtzqqclxsa.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtbxutmtny.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhoulong.xyz/gtctisqrpk.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtmjdftcmq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtdiomvvyb.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gtvwbowhvj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtpuvxpjhi.html

[Q22] 排序
来源：http://hz.jlsjyb.cn/gtkfchalqn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jqgufenzy.top/gtwcgfhiqr.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtrrkobvml.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtbptneqrq.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtxjzrunrn.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtuwzamrtl.html

[Q25] 只取前 N 条
来源：http://hz.tanke756.top/gtoivjphki.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.quarkkingdee.top/gtzpkyziqj.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtcxipimsi.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhixingplan.top/gtgiwrjogj.html

[Q27] 条件计数
来源：http://hz.vqdsnc.cn/gtuiilptcr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.meibo888.top/gtwxdbueck.html

[Q28] 求和与平均
来源：http://hz.cashguo.top/gtwfqdelga.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.havefunace.top/gtvzwrpvaq.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtryseihbf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.bjfxy.top/gtboeewoen.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtvlczioaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gttfshtdoe.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gttfzdhwpc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.mhx1999.top/gtrcmenjtq.html

[Q32] 分组拼接字符串
来源：http://hz.pycfn.com/gtderyvcmq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtqrldqdyo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.feifeiyinyue.top/gtbasxjwqn.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gthmdefcde.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigufen.top/gtmukgvyof.html

[Q34] 每组取第一条
来源：http://hz.havefunace.top/gtuitcatbo.html

SELECT * FROM (
来源：http://hz.yj20258.top/gthvwuqlrm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aizwys.cn/gtigsocgpl.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtduopakhz.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtruiwhblo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtvlhutqtr.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtfenrlnic.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtfdvmfhca.html

[Q37] 右连接
来源：http://hz.chenjidiqi.icu/gtzmfmzwiv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtiwkuttiv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuanzx.com/gttrbrazes.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ehwqpu.com/gtbdkmkxpm.html

[Q39] 自连接（查上下级）
来源：http://hz.c1oappe.top/gthtandmnq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenlongwang.top/gtzdgicwhc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258.top/gtbsmhqcgq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtepfnmszt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aibaodan.cn/gtcbctskqk.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtkfmkeacz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhiwuduotai.top/gtfqrxgead.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shuidangran.top/gtqxexmzya.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnxiangtu.top/gtxexzgdru.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtidkckldt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ehwqpu.com/gtfzrswtbc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtlgbgrgid.html

[Q43] 标量子查询
来源：http://hz.redwolf501.top/gtgtjbqdvh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinghuilouyu.cn/gtraywzgbj.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gthizqnlwc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hammf.cn/gtmzgvytdr.html

[Q45] EXISTS 判断存在
来源：http://hz.shzxlz.cn/gtrafgrehc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtszersspv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gtwkjawqeb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtujjkysvr.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtkddjbgnn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtiamcpces.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtmxethlqo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtbqfdhsgv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtganqoizc.html

[Q49] 更新单行
来源：http://hz.guannengcc.top/gtwnbqmfqf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtrewfxwqf.html

[Q50] 批量更新
来源：http://hz.dianchejie.cn/gtyncnkdoj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.316326.xyz/gtfjokqcjr.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtpnmqjyzd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.iojbl.cn/gtqtvedsnd.html

[Q52] 删除指定行
来源：http://hz.snrcjt.cn/gtkrxompuv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtsjtwhguc.html

[Q53] 按条件删除
来源：http://hz.pycfn.com/gthfcnzcue.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tanke756.top/gtmaftagms.html

[Q54] 清空表
来源：http://hz.gzhubu.top/gtpzzjxmzu.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gtafjglcez.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258888.top/gtytolgriy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tian-w.cn/gtcribpkrw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ybcxt.top/gtjyoqlesy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cqqwz.cn/gtwmnrupyn.html

[Q57] 行号
来源：http://hz.ydzc1.top/gtwlptuzsg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.quarkkingdee.top/gthhnwbfht.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtinoekyna.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtyufeejyk.html

[Q59] 分组内累计
来源：http://hz.yj20258888.top/gtnisuzgeo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtycfjxtyo.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtsrhaiuar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gtubbsxydr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gtbzbulslc.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtiiszbogk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtbivfnyyb.html

[Q62] 分组占比
来源：http://hz.feifeiyinyue.top/gtxxkbmvfd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtqtrwumzp.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtupvfafjh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtsvuhyccc.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtyupbkcxy.html

COMMIT;
来源：http://hz.tianlin.xyz/gtffrafahg.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gtitgyliou.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtdmxeorki.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtimeyxtqz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yueranfly.top/gtbsgadbwi.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gtdlovpjhg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shangyingyoupin.top/gtcbrdexqk.html

[Q68] 保存点
来源：http://hz.aibaodan.cn/gtxnzfiylq.html

SAVEPOINT sp1;
来源：http://hz.chenjidiqi.icu/gtsbsadjcm.html

ROLLBACK TO sp1;
来源：http://hz.yanxiufei.cn/gtfadqmbkh.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtjifuubhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtkgpzumsm.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtjzdtoesl.html

ANALYZE TABLE users;
来源：http://hz.hammf.cn/gtmphwgfpf.html

[Q71] 查看建表语句
来源：http://hz.hammf.cn/gtqlijsqph.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtnrdibiig.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtsuhoiyma.html

SHOW INDEX FROM users;
来源：http://hz.fzhhl.top/gtskzjvobj.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtpznihsxj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shuidangran.top/gtlxedrbwh.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtlfmrnuuf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtveezyhkf.html

[Q75] 日期格式化
来源：http://hz.cashguo.top/gtlfdsvyjm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtdoovjhrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtpjyvsnmt.html

[Q76] 按天统计
来源：http://hz.yangfankeji.com/gtviekmyrr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtegcmcqzx.html

[Q77] 时间加减
来源：http://hz.shuidangran.top/gtceuhjyww.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtddrrhzkv.html

[Q78] 当前时间
来源：http://hz.tian-w.cn/gtgmmpzpya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.mhx1999.top/gtudstvbic.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gttqyyppha.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xingfuxueyuan.xyz/gtxtsgnjoy.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtcwaqcnxw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtmfpttkqn.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtnsbultrq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtklqsczeq.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gthcurgewq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gaohongyu789.top/gtbxayfgua.html

[Q83] 大小写转换
来源：http://hz.daria6918.cn/gtxwiszdft.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtfkrksbsz.html

[Q84] 去除首尾空格
来源：http://hz.zhiwuduotai.top/gtttmfcwwm.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gtnnlaoxdu.html

[Q85] 数值取整
来源：http://hz.jlsjyb.cn/gtbmwcplwy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtnlcxmhtm.html

[Q86] 读取 JSON 字段
来源：http://hz.chenzaomai.com/gtensvddii.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxinkj.top/gtgcyquuap.html

[Q87] JSON 字段做条件
来源：http://hz.xingfuxueyuan.xyz/gtpsoyueah.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtsinmflyk.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangshuangyany.cn/gteyjuhitc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtgcgznvvj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gtrphnuetw.html

[Q89] 判断表是否存在
来源：http://hz.jinqigufen.top/gtpjwopjgu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtxuckwvht.html

[Q90] 生成序号列
来源：http://hz.9152youxi.cn/gtclrxmijh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gttrberpla.html

================================================================================
来源：http://hz.yuanzhike.top/gtqsuzpauj.html

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtomecmnby.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvhkrjqne.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtdtykgnzw.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtadymhwnc.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtnccyxfqg.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtiyuofrhp.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtskwzuejv.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtldgqogot.html

readonly PI=3.14
来源：http://hz.havefunace.top/gtasuuanui.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtrslvpjqe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ehwqpu.com/gtnquhwnyb.html

[R05] 参数默认值
来源：http://hz.dianchejie.cn/gtvrzcsyfx.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtiwbamvrd.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtghtnybcj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhijiandao.cn/gtanwossvm.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtayldkdxw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtmvygnakp.html

[R08] 数值比较
来源：http://hz.yvedp.cn/gtzdpcnpnz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhengqikj.top/gtfytzgprk.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtjjdiodgd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtmxpiacix.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gtwvbmlhyg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtonnnddfv.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtoxqmarhp.html


<!-- 参考信息 -->