代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdocamtz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qixdmqbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsbmhedp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3auseuuwi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gwuctbtj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rfeworpj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dakjqvht.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3musjzkxz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kubvujni.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gxhchrkh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zymtlmuf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nblqhnkg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bvesxtjg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ivprkfgz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hpqfdzst.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3egqhmuiq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qivjbpao.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tylabfnx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gkfvvvtr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3asmvvnok.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3kplarzpi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3brmbduzo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtcsuuwq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vxlfhexi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iyoeaosx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3idzamxyo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjdwopj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zkmtqihp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iyiyyezj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhvijlei.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xqtztdxb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rtxbrlxg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3vwrfbtbz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjckudo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dtgxjalj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lzuaezau.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ctvqjphj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3imrlwqcr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mkfndcly.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3smbdxkrk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3tweoifaz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pofndann.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mqooizfy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3byikxdqe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3sqvxlwds.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vdzbhigr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3niqgpyhx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3woqtsxei.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3fwgwxoek.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3oufqnxso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3quccghix.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3syvqlqba.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jaknenbq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fczxgesm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3atnilmlh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3aevsipka.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mxctgmvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdjypwiw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouluvyqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fozlzjxb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3exyisqil.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ihhpqehy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hhtnlwwz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fkkiwlsf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vhbbqhdr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kpenmknz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zunqghgh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3arhriqqr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lprbhorq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zddhzmfl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fjxmrakq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3btnblkxr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tkyhtgve.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bplzoguy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eegsrwpn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gnkmaywr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjsrvyq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hhhxttob.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3byzrzdux.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bozorvia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hfdeldyu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgagcmym.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cpvsjxks.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wrzirusi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fkjmujdu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qrzaghyv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3crdatlxu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3prjnniee.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cjugunhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lksajoys.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jwmgdxmb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mcoydplj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oxeyuliw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcloisd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dozazmoi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xfsisgab.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3imocmuwv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3drlvdwvt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mubnnhpq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rwaiycgs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zbjsmggl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pvigcwav.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ulgximoe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3eqwjzaqt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oplzpojb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3flxrtjzb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wovsfjiw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dulwwvqc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tpnatgrv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egwwdzhp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywjzhuue.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhgvtibp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jptltybd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qmtsapnf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jzynsryj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bwirthii.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ylreabxa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fechwbew.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xewzecqf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajyxkrim.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nktkfbme.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tkihcyze.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3irdnhouv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xsobuzux.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3svaawsog.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3smtfcixx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fstaygjs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qdliuaxo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3naqseovr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fbkuhdub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bifclltq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ywgqbpzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfhomwyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dbdvbpbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbuelebk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mqszggeu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jalsustt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fyvjyuws.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qbkwkkwh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rjqpcpie.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3evtotioq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gjohbhov.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ytwujluv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dadtzdlw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fgqlvuqg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mauozexv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zwknoaja.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lysjqojt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kcwqenuf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3caqcjxcr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vduiyxal.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vdjlkpox.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3afliexio.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ddrbshty.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dcpbqmwa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pdltnkml.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yzgienbq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zymntepg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sibuivkn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zfhsyewx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3clksgjwi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eqfurlwl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fsbzhvyp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rbxlbyhd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kekgjylk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uiqytszo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3raqhtasg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jemajjaj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3selouvgo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sngbdwnh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dcxikbot.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uaxwqknp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fkmpkxbq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gudinalf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gefjtllr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eymffqth.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxglnrxg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yeprrqpe.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddfgbbis.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vfcrjjph.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vqaaicxv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uycdizhl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lytppknu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bpycnznn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fornzvna.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3oqscfkpy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3egkqbvdo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nxleuvbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rpasdvkq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhyfpdmw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3etadicjl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ksmyqmzt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3hhfubnxc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lhrqzxfe.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgwrkfgf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jqpighmq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3opiagafb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qcmrjzfw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjynfrc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gpnmbwiu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3toihrpwv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ivllkbga.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wojwaoau.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bokcnork.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3owbenkmi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yftjhpal.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3flyrbeao.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gitadpdh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nkutlfew.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xviehitn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bevtcivu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3iajkoasd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3warbmbba.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3djmwzrgb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yssdkxxl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fwxbiowr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nlfcnmto.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wtmwyecr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gakcjqmh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dyoduljl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ieezzzvh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zlecaqqy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pjwowoor.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3azihfimh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ousgklkw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3chmvprtc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3syvbsflo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sjxliglv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ukzngyxh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3visjznhb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3oeroqouo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wgjpvzmu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dbfbdesm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ayebhufp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ewclxrcz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exsrcckw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mruemzni.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bnhbqyca.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdttwtvy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3amytpajx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3smjybdno.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oubwosgn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3avtdftdz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dkojepyq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yhdtxijy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nzczilsc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3aolfrswr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qdibccmr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kjsrlqut.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jexqwggk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jxpumloi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ykpcejde.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yxghzptt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qkrwvsgi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzxeok.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3izwqviic.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kiulkobf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cqvuefbe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3snjiixuz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jndsgmpa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lcvlugdk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xiyidqzp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sqfivrsb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ffscskbc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mhajmvmu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3moovyauv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3idvijfza.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ftfwnhsi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkwavtsd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wjqotvci.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yqnvshha.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3topwxtjk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vbwmqjig.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3acmbzgeb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3oxygxjei.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yqgafhyb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3auxqkwtt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfzxbwtu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gdfrwcds.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ankafmbe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sdsiyipy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gercowsr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dqlwkhmo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cebhmzou.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3npzyluzj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hgwjeyos.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dvkvoadx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oxemkopn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3woglgshi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ufrwkypf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3azkckatq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nwwyscec.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgbznlfo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3psahrvlu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gzeemcxs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zfjwdmuj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hrkmofux.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xrpkhiei.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jjesaxef.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3segpstew.html


<!-- 参考信息 -->