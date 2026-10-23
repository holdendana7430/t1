代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3aarcuizp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ipgfwbek.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pdmnjgyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3knesmkxy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxesmenn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tggxqenb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bchpiylv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bvxngnuk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xkujerby.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rdapqeal.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iuqcyxlf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dkvgmnqb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pnrewcyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3acbmyhhe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgmerr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jvkrywzl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3evtrlkmj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sxumbslh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lbtzoggu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dbfjnwpp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lxtccama.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fwzzfige.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wfxsydod.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvpbwqbj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qiyefzyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wktuimup.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mvehsyja.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wxeucdnn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jkwzdrpz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3feribiia.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ftfejhbr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lukpmpvp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wqnipgtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvomnxvf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jotzpwhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlbyvyll.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ywcufqey.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mmbfdrpe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oxhzasza.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vzleaqzb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xudbhiib.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iibogirt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qgyhjhlq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3glkninwu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mymaastf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oiypmufz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fbkptkza.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbxwvoth.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dwuxydos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3djjfcrol.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zpigtmnq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ykuindzr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyeqnxee.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dsaqqfhg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3myyuggxn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xriagyfu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qmvkofgi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mrmjnjqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jmxvcmbz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vzkwxqxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xjskusru.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mbjractt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qtzumljx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3paieydlx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bdiasgoh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nysdztsi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jaybdkrp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xobnoakg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gcandbrw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wmkzkipg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qdgwhawp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zthzlcrm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3znhhsbhz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zwsiopxp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3lujdaaxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3caxtvzzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3eeujnbxm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3oqvibkdo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbzetqr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fxvyeiou.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3haujddof.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mrwqhjoy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rfgwrujo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lretrjjb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3pohqukzh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ablqzrdi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fetamaxr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3iorpxmjn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dtoiszcu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcchqddx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3orauvzzw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wxeanmwt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3smubszwl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hwqbdmfg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jhksbtmh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3keetdnub.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pbumbhdy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pluhetvw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yxpywxgb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sjmsugea.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kqgsmbvn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lisdetdg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gwdikdvx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jtghnsvb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qpjpbpik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gfajpjvf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sgpbbuhl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3plhmihdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjgizfqq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3oqibatzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heztebgs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pdbyccmx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dcuaehdy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mbcmjiew.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mazmoxxp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fuwbtayy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ifjgwcwn.html

);
来源：http://www.52xcode.cn/Article/details/gt3wslnqofd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ptkbhcrl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3visefstg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rjucnyez.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3omesdecj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cuzpvwhc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3epuijpox.html

);
来源：http://www.52xcode.cn/Article/details/gt3ojprbnvv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tfufvllm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aclurtpr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxwgpeeo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bfezppjo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rkurxvml.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kojpqlcc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lvcnimqp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hpdnnvvw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3joplgmzc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3doreatbp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lzyowwua.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jricwkiu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qvsagahx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlcrlpx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mhmukurm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hsinibxz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3psvnqrbs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jbmdldsa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fbczvxxl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ojdpjrwb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3twfuvmqc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3pkvlfyhn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fsbxrlbi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ajmmzuwq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zzoazxix.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xfrqcvbm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bkzjrban.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmwrfaam.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gutacbqq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkofyrau.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hogztgyx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gdkijyot.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jbtkpwem.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fjsuoeer.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qkcayaaa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lbyfxqjg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tdlctlqc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xzolhbva.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ibxmyypg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cthflorx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3utpievuy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rnqneuos.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3asgycrlc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bdvxkzqs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xomoohfx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dumqlaul.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zywiqhdp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ahncdchf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zhconwor.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycxvceit.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3arhpatdu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tysbalvn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xjjleafh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rgexegli.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hxmstiau.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmbsuqzg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mmflcmae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wtqhwtks.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3peuairlr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3eciikuqc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xolkpjrg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fpbedydj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3upbujyjg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3niyfjppd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3sgjxbhth.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bclfuuhx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cjcersjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ekdodazf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkbgbchi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3iakdnkad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ghmxuntv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bwthzdzo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ienrjtbc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jyzvionm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfgpibk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bpmybhqk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3klsorwcz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xsdrvwuw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ggjlbtqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3farjuywj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bqcpmdye.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rjhfrjxo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dvkaatld.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ecvehauo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zumwbely.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kkmbzzxh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3urncagju.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zbaxcvpd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gxjxtzow.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zxvmatrk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3exkndlxj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fyahgssi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fzmynjcx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jnfbjetz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3izzqbfja.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3unywjsrf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qwhjizdd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3teydkqio.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3auikbnqq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zsasmvho.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3swjnrdmx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lxvhxclj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vmaamkhs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scoctaeu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3exzdxqxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3soyusngd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ugruxpax.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrddaigh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nmgeecjp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vwjvjstk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rkmydajp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nxnkqjyt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3quparpkp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ycvwakgc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tqwqlaob.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3olnuccnl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tfyuohyb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mcyfkxvc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ouvivqsp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dufuabco.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pgvhnugd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gklflisw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3zbisiyfw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yvfdmpkd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bsxkgalj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mzwfkrtp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nuxllxuk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ynctqhms.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jemoreuc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gjvkjdfn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nejmlhij.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nmvawsvq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3klbjqmpi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jxgewyrs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nmeksztr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cvaovmja.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cqggaljg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kcmomlat.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qulqoakw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jkmxwjkq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rxxkkuvk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xxohqnxl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjlsdll.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tqaveyrj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3stjlkbhu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hqpglzys.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cjhrssag.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wrrkqpxk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tasjrmgj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ddwxjeyj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lnltkshh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggrhqytq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ysbmrxoc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zwpqukoq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ldjprhdv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gyxdewdx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jpiisqlb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vzzfgymf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3adwkvveq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jvthquvj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cibksdnt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xezwqntk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qbkfvsea.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3htdbdhyx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pacusbor.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jxfgudsd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pwwqasfz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lyrqkokb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rownzeme.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jkugsjit.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idjvdtvc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ejdnxhuz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yuinpmsf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aiumpxyr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eefvtyai.html


<!-- 参考信息 -->