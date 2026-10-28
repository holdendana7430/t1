代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhiwuduotai.top/gteomijyxq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtikvxbfpl.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtgolkykcq.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtyvzsxocs.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daria6918.cn/gtxjbqxnko.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gtcprvxftc.html

JS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtaoiohapv.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtskvatrpl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtifldpwjy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xziqi.cn/gtfhcbloxr.html

Ruby: threads.map(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtuvxdxzcp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtzqmqisdc.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gttnccuwbg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtfzjofvrh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dashuyun.cn/gtkrzjqwuk.html

JS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtggxpxunb.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtjkhccuhc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhijiandao.cn/gtnzemoohp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.tian-w.cn/gtwnkzsigs.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtztciewvt.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtuhvptamj.html

================================================================================
来源：http://hz.ehwqpu.com/gtnyfhuwvd.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtzfybfhfj.html

================================================================================
来源：http://hz.havefunace.top/gtgkwpbqqh.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtrwclkcqq.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtlgvalwqp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yongpay.top/gtahlafrkp.html

JS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtnypfyinu.html

TS:   crypto.randomUUID()
来源：http://hz.wangshuangyany.cn/gtmmmcdezc.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtwlypuplo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtyvbbstns.html

Ruby: SecureRandom.uuid
来源：http://hz.yuanzhike.top/gtcvpxecrp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtwfuhulsj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtxizlxpzp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangtech.top/gtubwbgleo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnqzz.top/gtswieiaii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gtbhzkxxpd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtchxmbhry.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gthmszryjy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigfzy.top/gtdxlnesda.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhoulong.xyz/gthylzkcye.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtgxgmligu.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gttnyxayuy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtipqbgspx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtttapojvb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtfpvunuqu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtzapxvptd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtftiumbtf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtginvilaq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.redwolf501.top/gtgbjvixrf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.mhx1999.top/gtxxjzwsop.html

[P04] 求长度
来源：http://hz.fzhhl.top/gtrcgttvfg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtcnmmtzkc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cashguo.top/gtwhbqulyi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtntucanuq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtbxolhzry.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtplxlrxns.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtgkyewmmv.html

Ruby: x.length;  x.size
来源：http://hz.xuanzx.com/gtovxnypqe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydzc1.top/gtutpetgfu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.quarkkingdee.top/gtizudfvhk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shuidangran.top/gteoxrxiqk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtnplbatia.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtlgtprsqw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtbxoogjuz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtnkfbwxgr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtafejxykw.html

Ruby: a == b
来源：http://hz.andypj.xyz/gthqwkmipu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gtvjgtakul.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnqzz.top/gttezjlykg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hysaishi.cn/gtgwxjeztr.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gttfswpgql.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtmegyuqdg.html

TS:   if (x == null) {}
来源：http://hz.sufxvd.cn/gtaqafqrym.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yuanzhike.top/gteqjrgjuz.html

Go:   if x == nil {}
来源：http://hz.fengsongda.top/gtlkexrmtt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgufenzy.top/gtcurnpjcp.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gthdplxqjz.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtjnetebfx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yanxiufei.cn/gtnfuryrxh.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtfwtayvhm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gttbwqxnpf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtzqwxcnzf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.redwolf501.top/gthpdofxnf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtarckhiqy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gthhyzgnrp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yangfankeji.com/gtbwwexxvm.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtzlhzfkmg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtasgqqtpg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.fengsongda.top/gtqegwujfp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtraepoohk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtzuakzzpp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guannengcc.top/gtctsotoox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigufen.top/gtxvoainwz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtwwlfjodu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shangyingyoupin.top/gtxozmqpft.html

================================================================================
来源：http://hz.ehwqpu.com/gtturvipqw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangshuangyany.cn/gtlbgolkxg.html

================================================================================
来源：http://hz.guowangkeji.top/gtjcftxjer.html

[Q01] 创建表
来源：http://hz.yongpay.top/gtalmjqvyi.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtvpxjhyfq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sufxvd.cn/gthneueviw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtnftzvrnp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinqigfzy.top/gtpswgegte.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dianchejie.cn/gtscidozyb.html

);
来源：http://hz.yuanzhike.top/gtfrhtwuec.html

[Q02] 创建带外键的表
来源：http://hz.feifeiyinyue.top/gtnfbidfje.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtdmdvjerr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtldknrupj.html

user_id INT NOT NULL,
来源：http://hz.sxryk.cn/gtslqumnum.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gthinqktgo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sxryk.cn/gtmzafgbga.html

);
来源：http://hz.cqqwz.cn/gtnemzdyqc.html

[Q03] 增加列
来源：http://hz.hfpthk.cn/gteirelgef.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hammf.cn/gtvxjrydam.html

[Q04] 修改列类型
来源：http://hz.zycfv.cn/gtrsimelim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtshxiwjjs.html

[Q05] 重命名列
来源：http://hz.cheryme.top/gtxuhszmek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yueranfly.top/gtlfjdytpr.html

[Q06] 删除列
来源：http://hz.zhiwuduotai.top/gtcsjivqsz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gotoacloud.top/gtmrssdcqb.html

[Q07] 删除表
来源：http://hz.zycfv.cn/gtarmwgdfw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gaohongyu789.top/gtfikflcpt.html

[Q08] 创建普通索引
来源：http://hz.hfpthk.cn/gtpreaspwd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtdqdygxyz.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtohfoocqv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtxhselalk.html

[Q10] 插入单行
来源：http://hz.guowangkeji.top/gtwwmfqvzq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtohpegtyu.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtksjpfhxp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtdtuzfrcm.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gtctctslev.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtivealsae.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtfegsxteh.html

[Q13] 忽略重复插入
来源：http://hz.chenjidiqi.icu/gttoamuczf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gogol.net.cn/gtbtffwbcc.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydjk.org.cn/gtwnfposck.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtvzjxwuuq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhixingplan.top/gtxzxbbkla.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtbkzqczup.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtwsjljtqd.html

[Q16] 查询指定列
来源：http://hz.havefunace.top/gtbtsderty.html

SELECT id, name FROM users;
来源：http://hz.xuanzx.com/gtigrmgmtu.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtegmtdiaz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gttbfitfap.html

[Q18] 模糊匹配
来源：http://hz.jinyuanbaomall.cn/gtbjxqbgak.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.feifeiyinyue.top/gtvschesic.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtkwlujsjv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtxcbkkgbh.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtcybvyqdm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtjkanmtai.html

[Q21] 空值判断
来源：http://hz.yangfankeji.com/gthgjhtkop.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fzhhl.top/gtuhlgcqem.html

[Q22] 排序
来源：http://hz.birdmap.top/gtehrckfth.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtyaunhfrj.html

[Q23] 分页
来源：http://hz.zhoulong.xyz/gtooxhjxbq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xziqi.cn/gtyytvhzlc.html

[Q24] 去重
来源：http://hz.gzhubu.top/gteddywgww.html

SELECT DISTINCT city FROM users;
来源：http://hz.52xcode.cn/gtuekodyiu.html

[Q25] 只取前 N 条
来源：http://hz.tianlin.xyz/gtvjinyqby.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hywenlv.cn/gtismgejsc.html

[Q26] 计数
来源：http://hz.ydzc1.top/gtosfctrss.html

SELECT COUNT(*) FROM users;
来源：http://hz.dashuyun.cn/gtkqblkoot.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtazepabls.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yanxiufei.cn/gtrpdgomas.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtqjkrrpgk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258.top/gtoyfqboqk.html

[Q29] 最大最小值
来源：http://hz.pycfn.com/gtcxximhpo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtketpjofy.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtqwmcgiqe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtyhpkobrg.html

[Q31] 分组后过滤
来源：http://hz.yuxming.cn/gtplhdaefq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xziqi.cn/gtxoseddgy.html

[Q32] 分组拼接字符串
来源：http://hz.ydzc1.top/gtfjbexelo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtndptqhmy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydzc1.top/gtstoonhzk.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtcyxnudid.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gtxuqazbdv.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gthpnnxdov.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtztbtfluw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pengpengdd.cyou/gtugccwseo.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtzraistqb.html

[Q35] 内连接
来源：http://hz.sysykeji.top/gtxkcgmvpt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtmbmojcfs.html

[Q36] 左连接
来源：http://hz.jianghu66.top/gtfdkoevzz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtxrbzusex.html

[Q37] 右连接
来源：http://hz.daria6918.cn/gtmqnnunzr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenlongwang.top/gtsnuyvcwn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gtjxklmkky.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgfzy.top/gtawihufgb.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtrokykuce.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtmxqjuhyc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gthapqwsxl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtlqecjtax.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtrfwtzxyc.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gtjvkgovff.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtwlnvbgmd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gtyghmzblk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtprexiznl.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtknuqowya.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtnhjngmsh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuetiantiany.cn/gtxacpzaic.html

[Q43] 标量子查询
来源：http://hz.chenlongwang.top/gtuiooswge.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhengqikj.top/gtrxkpmvlk.html

[Q44] IN 子查询
来源：http://hz.birdmap.top/gtgtbedyvx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuanzhike.top/gtelnqnihp.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtfxnabfxc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtjylplcyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtvoqoerks.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtdrsjrzos.html

[Q47] 与平均值比较
来源：http://hz.hnqzz.top/gtypvpvyul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtddrepvrp.html

[Q48] CTE 公用表表达式
来源：http://hz.yanxiufei.cn/gteoqemeqh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hongshengwenyu.top/gtxjllzuwg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cdnleiting.top/gtbondloph.html

[Q49] 更新单行
来源：http://hz.dianchejie.cn/gtoxeytaiv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtuasmhjxd.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtangziqpu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhijiandao.cn/gtnlczghwx.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gtpikzprsg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxuanxn.top/gtpenpehmy.html

[Q52] 删除指定行
来源：http://hz.andypj.xyz/gtwvelhnry.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtzvthpnph.html

[Q53] 按条件删除
来源：http://hz.yonumen.top/gtlxpjmheg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtxdsdkmyi.html

[Q54] 清空表
来源：http://hz.guannengcc.top/gtiiwbbasc.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtstibndbr.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtoevpzzxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtyhykjtqe.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtbevhfadx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtadfgnehh.html

[Q57] 行号
来源：http://hz.gaohongyu789.top/gtflvdaeay.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtcnwkcasw.html

[Q58] 累计求和
来源：http://hz.guowangkeji.top/gtkqssrkxb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtsbcoyzke.html

[Q59] 分组内累计
来源：http://hz.jqgufenzy.top/gtqxtkykiu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtatoripfc.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gtgbmjeley.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtslnbrgfb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtunbxsgzp.html

[Q61] 移动平均
来源：http://hz.jqgfzy.top/gtutrbuttg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtbsyvrusi.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtkkaymhre.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtvfmcgdzg.html

[Q63] 开启事务
来源：http://hz.chenjidiqi.icu/gtixvqupea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj202588.top/gtdrvoollj.html

[Q64] 提交事务
来源：http://hz.jinghuilouyu.cn/gtotwkiudz.html

COMMIT;
来源：http://hz.andypj.xyz/gtobatdtbu.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtpgtknpbm.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtntnsplho.html

[Q66] 行锁查询
来源：http://hz.ydzc1.top/gtoecubilf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtrszkxdxd.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtsczrvnvm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtbucqdugp.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtswnrxyax.html

SAVEPOINT sp1;
来源：http://hz.dashuyun.cn/gtzzixrsxk.html

ROLLBACK TO sp1;
来源：http://hz.guowangkeji.top/gtmnhxzifn.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtwmxwrnuy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.9152youxi.cn/gtezkkqztg.html

[Q70] 更新统计信息
来源：http://hz.sxryk.cn/gtarnfcjcc.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtbiwodtyl.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtbvleefbb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.snrcjt.cn/gtjtnxulix.html

[Q72] 查看索引
来源：http://hz.jinqigufen.top/gtyvdrwzpv.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtlurvpkwy.html

[Q73] 查看表状态
来源：http://hz.feifeiyinyue.top/gtohrfdmwb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhengqikj.top/gtwmbftvbb.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtwsjfticw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.daxiang520.top/gtxcomvigd.html

[Q75] 日期格式化
来源：http://hz.gzhubu.top/gtuhwggwsm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtishpqgac.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.smart0.xyz/gtdesmbdxm.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gthvmlktfz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtjfrcgguu.html

[Q77] 时间加减
来源：http://hz.shangyingyoupin.top/gtwvnoawdu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtciokihie.html

[Q78] 当前时间
来源：http://hz.yj20258888.top/gtmhjbldra.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtgnnakosr.html

[Q79] 字符串拼接
来源：http://hz.chenlongwang.top/gtpxygrmos.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtkgnijchq.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtymnnwhpb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtdyiteuul.html

[Q81] 字符串替换
来源：http://hz.sxryk.cn/gtfxxfgoze.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtkayllwew.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtwcggvgkv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hammf.cn/gtzqssvkkk.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtkfoiqcgt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtwkauiame.html

[Q84] 去除首尾空格
来源：http://hz.yangfankeji.com/gtgqlfyhgh.html

SELECT TRIM(name) FROM users;
来源：http://hz.smart0.xyz/gtqjlpxkkr.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtzjhogyiy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtxjbpupxp.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtswobntum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zdqjudy.top/gtwcmswqhc.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gtejagmops.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydjk.org.cn/gtxfmckikv.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuanzhike.top/gtelygsrlh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.quarkkingdee.top/gtpngiyrze.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtjqizyogc.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtfruodukb.html


<!-- 参考信息 -->