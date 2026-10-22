代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jdoiernc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kyfratpx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hqkcadzf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2khtozrml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fkveqqxi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ozxjxokl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swygpssn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yfhocppg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2emlbygjs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oyzxlbct.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tbyrnusn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpjgkvu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cyaephxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fncorrlw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ctqbzgsx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yqklddut.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2llslcspu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dhptaeeg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nruieecp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ydahsxgp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sjfmtwfq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xjjxpwme.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uomzemjz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xwnsvaqb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2npunxisk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtrlpgjz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2neadzluj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ituldkdk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ovdcywfu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rxzstpqt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vbjkrdfq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xlbvfdmp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tvunykks.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpkgavvn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zvymvgjp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2juvonpsi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mbemjymd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zjhrybga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cwxkjrgd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivhbyeln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mqamuuso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kgzjfazr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2joynuwye.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ucphnkqy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtrouob.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vatwyjel.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iotvnwlu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ymhnpqtg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bxwlhwji.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zrcravia.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhyizitk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uveuacdc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uxyozygh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvatzwk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fjxsuppd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpdojpkv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gxfvkaim.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bjlrbcnq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lisokeba.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cachpqhu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2idvlzxgn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkblhey.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2shnjskot.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2osdzdtoa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2teucmtau.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2cwfgqbsp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zznqwroq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qybmozrm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcllihxn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2glykshyk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2spyjbcck.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2swmshaoh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2filottwy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ihmatrgx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nqtqwvxj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltlddogt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2etschthi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjihmwio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgmzlhon.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fnaqvawh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wuyctdzl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2diasbrht.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uxibfnsx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qertbkuw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ykfosjep.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xaexsjep.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yqsduxdv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2snmkgxnv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eoklfecm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2shbenivu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2dvfsvrbb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2uaijhtnk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ydxleocp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xeodbclx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bmxcwoak.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqwnfuvl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yvelyoko.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rafvvldi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ksdttnzz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rsobxfak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfvpqrzy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2adsleobs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbdmekle.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2elakcfxu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vupbrzhy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kxncnihd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hptytmuy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iegzymgb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2brnagfbr.html

);
来源：http://www.52xcode.cn/Article/details/gt2mdmkbprl.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bihmnbsa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zsnajykc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bxovvjvv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kuodcicu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2sqyudvoy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxgsfxi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iixefhus.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zbbpskeu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wnaftxwp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ichbwlxy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zsvminuv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nnniwzwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2sbiootnn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dqzrnsbb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zsdhsjod.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2onzxkljc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2execesiy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rbeyhzde.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cxhripko.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wfohldvo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dlzqpzyh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2lulihnfr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2efyxojsw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2huzlyugb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bixgnprm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kpihfwtl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lshfmccs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fkcautfc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uoihvxon.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ktibnlfm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hnnblvgf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vlsfrbjr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ynwtikft.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kpckkaav.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvkzpokh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zchzvudq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxjwiuzy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vgqjhisq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdcavv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2taifhuha.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ehrlcret.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tpqdsask.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2nihhkqtf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2njbapolu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2acpillga.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bbmeyiwj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ubfqtmam.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zqlaeszm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2engstwzc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gdxxlujn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mheopskf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xyysyfsm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvaupnej.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qrddtzvf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mqieuhvl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bgfroqez.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avbytalb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rwrleiro.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iytoxico.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2odequwrp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qpnthyzt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oyykyuzt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lkfjmjou.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rvepndfk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vxxdqlfr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xisgbeoi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wonxsros.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eseiugxp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cmmobnoj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mrgdgwxq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ckwxvsbt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2adadeqkk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jptzqayi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2quczhjgc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vnkslmoo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evdxxdth.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eeyicoaw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ofyjhznf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zpgvuxsk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hhihrvuv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2sgwpwdli.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bmzpbrep.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2takbhvnk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dndmjhox.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2iwmvpyny.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2biwksqma.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jisqpddp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dlxciofd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2chglyufx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2djdvpmrw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zfjcgiuy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ntbqozfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2okyjovht.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2grcjimgg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jyvmcyjt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2udoljfvp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jhrhhnbk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nslxdcms.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fjoaeril.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2aymnzcnr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wtmydcfw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2twfasjpz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2iicwimks.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mtiiqllu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vkviahjg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcssadp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vpvkbfmb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2tcztvybh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lxpsbpjy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mlktemci.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wqxfzjzw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ukbuicmo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jtdlmcpe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qjiqzmuw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqwlzhx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2oanoyhzl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xkoegocr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2eyswjzgo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fquvzzfv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dmcarinu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2svltpupu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wbjxtitj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aqjrukqk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fgzuktmh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jvezduai.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jaucjtmu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klaxvoij.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uavqmgso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lkttgjzm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uzrbjmpp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2myxsgxfd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kksybivo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pzhbgibr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxdinzme.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wyohdkxo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gjwopivw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qdxkebox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hsckcpmw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fbkokveh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2oxoautlx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2eciixrxd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2splndfdj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2coatwhhz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dcyldbxb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vbwfpage.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jzligfxx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cjyjgzjj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ptyeqfnl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mjkwyrgg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mnusmwyt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2afgeghrp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hodbagmp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2iuhdflwq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2quepaskl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2yewdyvdd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wfgltrdw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dcpgytyp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dksusqpi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfznmrxs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ctwmjrqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fmwrlopy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dnpkkjgg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rnwsofui.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wipcqkdi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ftppezyy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vrmzgorv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2veprmftd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rpgybtrt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kmlvyrky.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2anfhbogx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gsyzzvkz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pvfojkjd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvuuzc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fveuexqn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bdnekqcn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axjqshfb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sprjnogn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coahnrei.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gicsyqyr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zlcgwuer.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jznsrdvt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dkytnnau.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdsyom.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ejrkjfxa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ycfhqpft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hwkmchff.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nfiaueot.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jpthttlk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bgihkegh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fjomgzpf.html


<!-- 参考信息 -->