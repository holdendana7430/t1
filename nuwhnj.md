代发 wailian999

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtdcemkaij.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtzuggzgih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yangfankeji.com/gtzpeipgxr.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gthhastdzf.html

TS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gthihkszqz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.smart0.xyz/gtmerszwsz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.smart0.xyz/gtipdwxgrl.html

Ruby: // fork 块
来源：http://hz.chenjidiqi.icu/gtibrbmwlb.html

C#:   Parallel.For
来源：http://hz.daria6918.cn/gtgliesvfi.html

================================================================================
来源：http://hz.jinqigufen.top/gttcridvkj.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtcajjjdln.html

================================================================================
来源：http://hz.tian-w.cn/gtuvuwktij.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtgtprbyod.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtbnxttvpi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtvqdqvrpc.html

JS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtxlgkpume.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gthtzxjduq.html

Java: UUID.randomUUID().toString()
来源：http://hz.haohaochexian.top/gtfsftunro.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtapvjxdib.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gtjumoxcbz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtaobdmoap.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj202588.top/gttimejhgh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtwntslhum.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.52xcode.cn/gtnbaksvbe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gotoacloud.top/gtkncrjuup.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtsraevwzd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuanzx.com/gtvwfglotf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.52xcode.cn/gtmtjsupia.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gtwfkyihbj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hywenlv.cn/gttakpvapr.html

[P03] 生成短随机字符串
来源：http://hz.zhongyouzk.top/gthtjzfuad.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gtabvwxpia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gzhubu.top/gtnwmxsjvf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtjjojibzf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtqyjvtjep.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangtech.top/gtyuynshkc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gtfmnvjawd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gteitzlpdg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gtexankjyw.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtutqvbwag.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtcwgbfxjb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtpfiflaaz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtjyynvysc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtvuxnjboo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtqdmbfbyi.html

Go:   len(arr);  len(m)
来源：http://hz.ydjk.org.cn/gtfalyjqus.html

Ruby: x.length;  x.size
来源：http://hz.hnqzz.top/gtiusherar.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.svipenyu.cn/gtngvyfpws.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gtzijihdyp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtqayrpzez.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gteeldkgjj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtunrqiazh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.snrcjt.cn/gtgonppixr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtehxkknnh.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtbbhoucta.html

Ruby: a == b
来源：http://hz.aibaodan.cn/gtiovobrzl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guannengcc.top/gtgpzeqxau.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtuuwdkrgt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gtvcbcnzsj.html

PHP:  if (empty($x)) {}
来源：http://hz.zycfv.cn/gtegqesmyg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yueranfly.top/gtdydvtefg.html

TS:   if (x == null) {}
来源：http://hz.cucudq.cn/gtoqfijiiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtjkkxskjy.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtddhvagce.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cashguo.top/gtcxfalclu.html

C#:   if (x is null) {}
来源：http://hz.zhijiandao.cn/gthmgysrxk.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtpcgizerl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtjmaynquy.html

PHP:  // 手写时间戳比较
来源：http://hz.yanxiufei.cn/gtjqddxcxn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtnlacauxi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtgcechbko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhixingplan.top/gthagofued.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gtlheixztc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guannengcc.top/gtnfeptfbn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ppjwa.cn/gtdljrbnhb.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtmbfvhozv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gtleozwzre.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtieecupbw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuanzhike.top/gtdruitiuy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtehzbbmpy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtxdcyhwod.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yvedp.cn/gtdercfyme.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xinyue.icu/gtwvnkjzfk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ydjk.org.cn/gtxnlnobze.html

================================================================================
来源：http://hz.aibaodan.cn/gtilpfszdr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gthfagihhl.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlwgixxzm.html

[Q01] 创建表
来源：http://hz.daxiang520.top/gtqbfqrqlm.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtkmsuygim.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtcwlrlbrq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtbftkcttf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtwjndqnyo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtluiazkgt.html

);
来源：http://hz.shzxlz.cn/gtezizsphh.html

[Q02] 创建带外键的表
来源：http://hz.tianlin.xyz/gtefinieok.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gtazsisjgy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtkbwosyao.html

user_id INT NOT NULL,
来源：http://hz.shangyingyoupin.top/gtfjdviacy.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtkbskgxtv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yvedp.cn/gtwcqgilrj.html

);
来源：http://hz.jyoumei.cn/gtwilvqhjw.html

[Q03] 增加列
来源：http://hz.snrcjt.cn/gtddjjmcri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gtfixpylps.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtirlwaxxr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtzdkbhqtk.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtdzwbxwne.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fengsongda.top/gteusqmyyn.html

[Q06] 删除列
来源：http://hz.cucudq.cn/gtszuqzbgo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtvqkrsluc.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtqnsnvyaf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtqqlxqlgx.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtrpbwzcuz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj20258888.top/gtafdidlhe.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtbuqjmurn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fengsongda.top/gtabtmekef.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtamhffesb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhengqikj.top/gtvnzrcigk.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtfpalqvjr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.iojbl.cn/gttwnoodok.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtjcbjepuv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gtnrbjvlim.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xingfuxueyuan.xyz/gtidfyhjtm.html

[Q13] 忽略重复插入
来源：http://hz.chenzaomai.com/gtribdlktt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gtrdpwyhmp.html

[Q14] 存在则更新（upsert）
来源：http://hz.jqgufenzy.top/gthdmouwir.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgfzy.top/gtnhwcmpwt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tianlin.xyz/gtmtvjgrej.html

[Q15] 查询全部
来源：http://hz.feifeiyinyue.top/gtbtftskep.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtzssgpcbb.html

[Q16] 查询指定列
来源：http://hz.hfpthk.cn/gtbqxrjjki.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtzntqktoc.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gteuvurisq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtxcuxjxsl.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtopkehhkg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtawbeedyq.html

[Q19] 范围查询
来源：http://hz.zhixingplan.top/gtffawdbne.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtrwdmnrmt.html

[Q20] IN 列表
来源：http://hz.vqdsnc.cn/gtrizsjvie.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gtpqtynwiq.html

[Q21] 空值判断
来源：http://hz.yuanzhike.top/gtyourqrcz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtrbrfszxv.html

[Q22] 排序
来源：http://hz.c1oappe.top/gtwocgdnil.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xingfuxueyuan.xyz/gtocecyryg.html

[Q23] 分页
来源：http://hz.cucudq.cn/gtnitttgid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yueranfly.top/gtugzltwtw.html

[Q24] 去重
来源：http://hz.jinyuanbaomall.cn/gtndsrrokv.html

SELECT DISTINCT city FROM users;
来源：http://hz.bjfxy.top/gtjdidgdiy.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gtimgyzubw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtrezneaki.html

[Q26] 计数
来源：http://hz.nanxinkj.top/gtbapiqfoy.html

SELECT COUNT(*) FROM users;
来源：http://hz.fengsongda.top/gtpvdvqafz.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtqpgtzzjf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtyfgwxnkp.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtjtxcwkzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guowangkeji.top/gtwrxrznnk.html

[Q29] 最大最小值
来源：http://hz.yuxming.cn/gtyjijqywn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtcuqpfuat.html

[Q30] 分组统计
来源：http://hz.jqgufenzy.top/gtuvbxlhkd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtmjlhvser.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtyqcsritv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cheryme.top/gtkseuskhn.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtgvbfhkkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtkwavmhwz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gttdoyumfm.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gthvkqrtds.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gtkehehfgw.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangtech.top/gtnqirqwek.html

SELECT * FROM (
来源：http://hz.wangshuangyany.cn/gtgoqtffuh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtqswylhbl.html

) t WHERE rn = 1;
来源：http://hz.guannengcc.top/gtrkgwspbp.html

[Q35] 内连接
来源：http://hz.xylfe.cn/gtuumrxooa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtfmzminsh.html

[Q36] 左连接
来源：http://hz.hnqzz.top/gtrrlliqfi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtyymlzvsn.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtmmlwqmgb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gogol.net.cn/gtgbvhvxox.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtswlpjfvl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.andypj.xyz/gteonurmii.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtbasvmcgv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xziqi.cn/gtoimoidup.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtzdtvpkit.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sweek.top/gtbfnxwmtp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtmqpittgu.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtxyzauvmx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtbpnlwtlh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.chenjidiqi.icu/gtwagqhnkl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhongyouzk.top/gtukjauzap.html

[Q42] 连接条件附加过滤
来源：http://hz.aibaodan.cn/gttjihtulq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.0kj1m.cn/gtfzrnqdgs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtjnvqvirp.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtbtqeramy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fzhhl.top/gtdbhogmso.html

[Q44] IN 子查询
来源：http://hz.sysykeji.top/gtpuaucccz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuanzx.com/gtvhxhipmf.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtiundemjo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtbdnoupyk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtbvxuhtbt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtiwjvppno.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtrdlwyvza.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xziqi.cn/gtklxaimgj.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtgqvqhnyp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtcsxgtphj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jqgfzy.top/gtrxjhomzo.html

[Q49] 更新单行
来源：http://hz.mhx1999.top/gtyrizslkk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuanzhike.top/gtxawzgijm.html

[Q50] 批量更新
来源：http://hz.wangshuangyany.cn/gttwyvwihg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtftcyfymi.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtohagsyti.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jyoumei.cn/gtojeqogsk.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gturzftiqd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cheryme.top/gtwmguzgfi.html

[Q53] 按条件删除
来源：http://hz.andypj.xyz/gtzsmpijix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtohexqutp.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtkpesdzxj.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtlzyxcyxq.html

[Q55] 排名（并列占位）
来源：http://hz.chenlongwang.top/gtebgkbbry.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj202588.top/gtjbxqaytn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhongyouzk.top/gtpfiqvzqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtadnuavfl.html

[Q57] 行号
来源：http://hz.nanxinkj.top/gthphipiqx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gtpmjdrekq.html

[Q58] 累计求和
来源：http://hz.nanxuanxn.top/gtvfahbldy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtaiqovgkt.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtxqngljpz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtkwiikzwi.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gtvfsxraqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtbfmofogi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtrbajwtwt.html

[Q61] 移动平均
来源：http://hz.gotoacloud.top/gtymlxyncm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtrvsjjsoh.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtgdjbperi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtdxkifxjz.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gttbsgxbwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtshljxlin.html

[Q64] 提交事务
来源：http://hz.ivvv.top/gtuxropxsj.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtzpixrytj.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtjrphbvyq.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gttwshffcs.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtmecnoldy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gttcvptzoj.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gturojcghy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhaomingkeji.xyz/gtscnuhjqh.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtiadjjvwv.html

SAVEPOINT sp1;
来源：http://hz.shzxlz.cn/gtchsgdzqk.html

ROLLBACK TO sp1;
来源：http://hz.hywenlv.cn/gtyxzvapij.html

[Q69] 查看执行计划
来源：http://hz.sufxvd.cn/gtwjifdooe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtztqdomxl.html

[Q70] 更新统计信息
来源：http://hz.sxryk.cn/gtwsmfelzn.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gthtvjcidq.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gtuefgbpar.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shangyingyoupin.top/gtjkbbbfqk.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtesrslwei.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gthjyzljbx.html

[Q73] 查看表状态
来源：http://hz.xuetiantiany.cn/gtjkgnghkb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xziqi.cn/gtdynxvtif.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtfrdktnwn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gzhubu.top/gtuqzarsyz.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtwkrqlscs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtgrtujmtb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtxogddpaa.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtyxwnexsn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtvzpzaaur.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtlfqgjllp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtedtaibsa.html

[Q78] 当前时间
来源：http://hz.316326.xyz/gtdmfoajck.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtwwrcjhce.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtyraddrnk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtewjoogfe.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtcllpzyph.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.feifeiyinyue.top/gtyrhlbodx.html

[Q81] 字符串替换
来源：http://hz.birdmap.top/gtoditaear.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtpunzopux.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtueelamuk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gtxzgxhbma.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtwfldnlaz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtxcwdcsiy.html

[Q84] 去除首尾空格
来源：http://hz.feifeiyinyue.top/gtqbfpzwps.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtcjuwzkxd.html

[Q85] 数值取整
来源：http://hz.sweek.top/gthsqtatrr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtfgehfywo.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtbzpwyszy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.daria6918.cn/gtnwcspmkr.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gtqxrlyxjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtygpmgxtd.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtffgmakhc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtpxeblxlc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinyuanbaomall.cn/gtgprrxqla.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtwnwfhljv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtajbunqzr.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtvzvuwfja.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gogol.net.cn/gtefawxksn.html

================================================================================
来源：http://hz.jyoumei.cn/gtpofdkslb.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtcszcktzz.html

================================================================================
来源：http://hz.birdmap.top/gtlkrnyahj.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtovzoxfqx.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gttcxprxwn.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtamxqwolq.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gtrjpnonsm.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtepwyrjcv.html

[R03] 只读变量
来源：http://hz.zhaomingkeji.xyz/gtjdugakur.html


<!-- 参考信息 -->