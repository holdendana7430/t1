代发 wailian999

[O06] 使用进程池
来源：http://hz.sysykeji.top/gtomkxkpvf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dianchejie.cn/gtgbnynlkp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.316326.xyz/gthkjsgrug.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtxpkquhqu.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtlvcxtflj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gogol.net.cn/gtanqiwghb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtqirrabun.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtztcbxdif.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gtqldwaqpf.html

================================================================================
来源：http://hz.hammf.cn/gtjzxrdfgq.html

P. 常用工具函数
来源：http://hz.xylfe.cn/gtqfzbaebn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpqrkmykd.html

[P01] 生成 UUID
来源：http://hz.meibo888.top/gtpphjmfhy.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtagyemqme.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhijiandao.cn/gtnnfkcfxz.html

JS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gthdyyrxsh.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtlbltmtfs.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtouqtcbxe.html

Go:   // 用 github.com/google/uuid
来源：http://hz.meibo888.top/gtidaipkiq.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtxymqewlo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtiahvstki.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtjlpcfwhc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuetiantiany.cn/gtmbcmlbsn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.smart0.xyz/gtkravqgws.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtjzplxdcl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinghuilouyu.cn/gtggawloih.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtrkmpaszy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigfzy.top/gtysjvxizu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cheryme.top/gtwbfmtneb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cheryme.top/gtcoqqsrkj.html

[P03] 生成短随机字符串
来源：http://hz.andypj.xyz/gtjwcncezp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tianlin.xyz/gtkixygcfb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtxzwndulr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtvrydsnzc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtuwzhzoug.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtoxyocufv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258888.top/gtdxdhcfke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtpxqzriok.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ivvv.top/gtbbebdstd.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtdoxiwezo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jqgufenzy.top/gttmaqrlui.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtvxhszjvy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtavyncagd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtomaggijn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhengqikj.top/gtcfoemqql.html

Go:   len(arr);  len(m)
来源：http://hz.hnqzz.top/gtesgjlmzr.html

Ruby: x.length;  x.size
来源：http://hz.ivvv.top/gtnndaexxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jiagoushi.top/gtlcgoemcr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxinkj.top/gtxqaivzhw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hfpthk.cn/gtedbgqagh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yanxiufei.cn/gtlzjckpco.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cashguo.top/gtajqreynj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtmdrsjosz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shuidangran.top/gtsfeunsts.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gzhubu.top/gtprbzqvgt.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtavtpwjbe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinghuilouyu.cn/gtodxaqrzz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtfljlrnib.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnqzz.top/gtildfmcyf.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gteyallvbq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sysykeji.top/gtsylhryxu.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtplfhmgyr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtdbpyeper.html

Go:   if x == nil {}
来源：http://hz.gogol.net.cn/gtyywzezfi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tanke756.top/gtaxxvswsf.html

C#:   if (x is null) {}
来源：http://hz.jinghuilouyu.cn/gtktmvrgma.html

[P07] 防抖与节流
来源：http://hz.birdmap.top/gtliondhyo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtoqtnfgrm.html

PHP:  // 手写时间戳比较
来源：http://hz.daxiang520.top/gtajjtwwep.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtvynjfvsw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtkmkbsdzy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtwssgsvwb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtbmzrqpyk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtzrbmandj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shangyingyoupin.top/gtxctqvoek.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtwljxivjw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangkeji.top/gtxrdgkxze.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hysaishi.cn/gtiikjtdvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.svipenyu.cn/gtnxvbbsvk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtavqjiwmw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hfpthk.cn/gtajzkxunj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gthlholuhr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sxryk.cn/gtxbnqicyx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ehwqpu.com/gtkwrjqbdm.html

================================================================================
来源：http://hz.jlsjyb.cn/gthlkuyhhx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtpcscepte.html

================================================================================
来源：http://hz.yangfankeji.com/gtiqsitpnv.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtqkswfpjk.html

CREATE TABLE users (
来源：http://hz.daxiang520.top/gtjhyeybib.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtyvwybulb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cucudq.cn/gtvmwmjsly.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtmlrimizc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhijiandao.cn/gtvrbmsqje.html

);
来源：http://hz.yanxiufei.cn/gtjsvbcojf.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtbrksnqur.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtruqpchjs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gtivdguell.html

user_id INT NOT NULL,
来源：http://hz.hfpthk.cn/gtdkpmrtle.html

amount DECIMAL(10, 2),
来源：http://hz.nanxuanxn.top/gtxqhehuzl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jiagoushi.top/gtafagibuq.html

);
来源：http://hz.zhoulong.xyz/gtcimbpblw.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtrneafwav.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ppjwa.cn/gthjojtdsl.html

[Q04] 修改列类型
来源：http://hz.sxryk.cn/gtpnilqeze.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtqsvllsod.html

[Q05] 重命名列
来源：http://hz.jqgfzy.top/gthgnzsdee.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cucudq.cn/gtmkezskfw.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtfantedsn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gttmuhqfpr.html

[Q07] 删除表
来源：http://hz.xziqi.cn/gtbbhkbsdo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tanke756.top/gtstmjmxbd.html

[Q08] 创建普通索引
来源：http://hz.sufxvd.cn/gtioxqggoh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtqzvkrmms.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtdnzhxcho.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtawhdflyj.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtdqrewtjh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ivvv.top/gtcmbnnirn.html

[Q11] 一次插入多行
来源：http://hz.aibaodan.cn/gtrtqvncgm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtrhejqjfz.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtloovpzxn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtqoknqfsw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtqbethflh.html

[Q13] 忽略重复插入
来源：http://hz.smart0.xyz/gtpdvvqrhf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gttyqatosc.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigfzy.top/gtketuzbel.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgufenzy.top/gtxrqpkwkh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gtetroeadd.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gtxcwrubvv.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtvcdzkbaf.html

[Q16] 查询指定列
来源：http://hz.xinyue.icu/gtiswjzivw.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gteyvnwgrr.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtxpymjbft.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gthuqskymi.html

[Q18] 模糊匹配
来源：http://hz.fzhhl.top/gtltrdxcji.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gotoacloud.top/gtwibnvdtw.html

[Q19] 范围查询
来源：http://hz.xziqi.cn/gtkgnkqogn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gtdqqovoxn.html

[Q20] IN 列表
来源：http://hz.ywan-chungtsiang.top/gtsmbdcppn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gotoacloud.top/gtarltzalj.html

[Q21] 空值判断
来源：http://hz.yanxiufei.cn/gtnbdiwntj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtgbdlsuyy.html

[Q22] 排序
来源：http://hz.redwolf501.top/gtfepdmzde.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.meibo888.top/gtqgqrqbfx.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtodgqfwev.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shanyushiyangkeji.top/gtqrbuczfq.html

[Q24] 去重
来源：http://hz.cucudq.cn/gtziiamlic.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gtbgpegfjh.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtqkkqvqkz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.quarkkingdee.top/gtzgpkmbvf.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtskftlpdm.html

SELECT COUNT(*) FROM users;
来源：http://hz.cucudq.cn/gtgupbuiaa.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtushswamw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxinkj.top/gtkzvxxcer.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtazkjbwpx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtwzdwvcru.html

[Q29] 最大最小值
来源：http://hz.pycfn.com/gtyzifujnb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtuwjlrmxb.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtavcjukvv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtjqxwopun.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtpwkqezev.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtbjyvlbau.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gtccndvxqj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtfmabztqw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtindmpuft.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gtnbhprayx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sufxvd.cn/gtmpbhmgkw.html

[Q34] 每组取第一条
来源：http://hz.kuanghao11.cn/gtgtftofgw.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtlhrwitgt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtwxogzdus.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gttkvrwizp.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtacqmoduz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtedzdcwfy.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtphegwnvr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtwdasijcn.html

[Q37] 右连接
来源：http://hz.yuxming.cn/gtmupolqzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtaukhqtwy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.9152youxi.cn/gtrihdqwxt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtfljmmkby.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gtqeghgoyu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.smart0.xyz/gtcuhhvekm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtrvjmwzmw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gtwautsvjq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jqgfzy.top/gtjwelzoli.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtstkjbzux.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtyfmmgsrv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtjinqcohb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtkkimcebi.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtixhiiyhk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.bjfxy.top/gttjnzzdds.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinghuilouyu.cn/gtozabdlaq.html

[Q43] 标量子查询
来源：http://hz.316326.xyz/gtecnkwmeb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtslfrvuhg.html

[Q44] IN 子查询
来源：http://hz.zhiwuduotai.top/gtwlrkermk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.c1oappe.top/gtouabtlvv.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtdkufnroq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtdsxqibem.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtzisriren.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtpzbrkmnr.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtdiljvofr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtdbfaghfp.html

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gthocmccpj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtxypzhbwz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtntzsbqvo.html

[Q49] 更新单行
来源：http://hz.0kj1m.cn/gtxicvxiqt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nwbrower.top/gtkgpmowdj.html

[Q50] 批量更新
来源：http://hz.snrcjt.cn/gtmkcsdfzz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtmvgoroja.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtsbpttfgx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigfzy.top/gteyddqsaa.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtqyqlqasy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtkioubmnf.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtfdwnunqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtbvqfedgq.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtdcosmygd.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gtfdujyhcq.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtmmclxyam.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtckxjlolg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtzarfjudy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtodzodmrb.html

[Q57] 行号
来源：http://hz.shzxlz.cn/gtukmhmxic.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtvidpagbz.html

[Q58] 累计求和
来源：http://hz.jinghuilouyu.cn/gtrjxfidbg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jianghu66.top/gtlwvrnhjh.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtolpanirs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtloeyqema.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtypfpxxse.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtysqyqxth.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgufenzy.top/gtrjtqoyti.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtekcthgrs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gthsuveljd.html

[Q62] 分组占比
来源：http://hz.bjfxy.top/gtowiclrvy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtqsfpjmka.html

[Q63] 开启事务
来源：http://hz.iojbl.cn/gtkskhzrnu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gttjjcgnom.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtbwzpgptw.html

COMMIT;
来源：http://hz.yongpay.top/gteuwletsu.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtycdxflak.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtpqpmdqsk.html

[Q66] 行锁查询
来源：http://hz.nanxinkj.top/gtvrkjnykl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jianghu66.top/gtvxkgsfhd.html

[Q67] 设置隔离级别
来源：http://hz.bjfxy.top/gtklkegnuu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtovgudmnq.html

[Q68] 保存点
来源：http://hz.birdmap.top/gtgertclrr.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtmxmyjnlg.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtjhbywtbi.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtolnlfjta.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtsystofdd.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtllpivhkx.html

ANALYZE TABLE users;
来源：http://hz.hfpthk.cn/gtqepjrkxw.html

[Q71] 查看建表语句
来源：http://hz.0kj1m.cn/gtvsvspcie.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gttkcfilat.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtyyxvnhlc.html

SHOW INDEX FROM users;
来源：http://hz.hongshengwenyu.top/gtipnqacqu.html

[Q73] 查看表状态
来源：http://hz.wangdashe.top/gtlamjhrdf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtunorgmwh.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtskdjsqeb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cqqwz.cn/gtxbbdnpfn.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtpclhpoux.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtijslbctb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pycfn.com/gtwbgtdrld.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gtcgrxappr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jiagoushi.top/gtvbjsmyuh.html

[Q77] 时间加减
来源：http://hz.52xcode.cn/gtzpaihvsw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sweek.top/gtozwqjusi.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtwcahwqgx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtdcakqxqj.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtztaxchcs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtlyhvslxq.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gtjytmroop.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgufenzy.top/gtzlmwoodp.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtsjimruek.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.iojbl.cn/gtxdfinyti.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtittjnljv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gtglxjhien.html

[Q83] 大小写转换
来源：http://hz.nanxinkj.top/gtlwnwfohf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtgjyrkslz.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtdypvhwep.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gttttvgqpr.html

[Q85] 数值取整
来源：http://hz.ybcxt.top/gtibgsfdkm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtqtbdrrpm.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtdvaatvvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinqigfzy.top/gtsvlcylef.html

[Q87] JSON 字段做条件
来源：http://hz.haohaochexian.top/gtpnxgmnem.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.andypj.xyz/gtifxoirfl.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtdpjiidlg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtuokrzkhf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtmqbvfmue.html

[Q89] 判断表是否存在
来源：http://hz.jinqigufen.top/gtgfsgnllp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtjvdnituy.html

[Q90] 生成序号列
来源：http://hz.ybcxt.top/gtdhuttavs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtqqjekfhy.html

================================================================================
来源：http://hz.gotoacloud.top/gtfnvatymz.html

R. Bash 专题
来源：http://hz.gotoacloud.top/gtnvfkgage.html

================================================================================
来源：http://hz.jinqigufen.top/gtlkukdsbc.html

[R01] shebang 与严格模式
来源：http://hz.yuanzhike.top/gtdhonugnx.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gtpryxrfdc.html

set -euo pipefail
来源：http://hz.svipenyu.cn/gteilzcajv.html

[R02] 变量赋值与使用
来源：http://hz.sweek.top/gtkgzuwrtv.html

name="Tom"; echo "$name"
来源：http://hz.gaohongyu789.top/gtzetcgxkb.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtgmoivydb.html


<!-- 参考信息 -->