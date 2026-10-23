代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxhsbsix.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qqynktrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iorloywh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fybptxac.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bvcormec.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvaqtaci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xkhbzjkb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gbvnygmg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3avdjtdyc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3eogcqklp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vsjaqmli.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xzlcdtnm.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3asvgcqfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cylchjxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tzkvoecj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aockuomi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jviuwgeh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zyclzfqa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3esrqiujw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qzawdowv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hwhhspmy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pqgsnhdf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcavvubz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vavczbcj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zthnjejo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jelzpjkp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3luwwfifx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wtuurwnc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wqukhbrg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swejorxs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qdohfwxi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hgrpqrih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lifuvvxy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bundvglq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3exqgvepi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bjvqbtpu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iwlanbrf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bzvnweef.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3svuilfon.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tntrnsab.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gnohzosa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jgwcaefs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yljvwgym.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3aweahvto.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3znwumvsv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3pdiocntt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3twsufcji.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3racwdlxa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zffcyalv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yoetjygw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lekfmkhu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qpxdiuei.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eupmrhtp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3spcyilyb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ekjnpfge.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xfzknxtn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nxqvirsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuyltony.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3foonwngw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqccjcca.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zehehasy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gglowcon.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pglmfvur.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nnfcbduz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ysrvncma.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rytsulkw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hczpjhhh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gkatvbuv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3voihncgv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bidonlzu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3unnyvgtr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhotwosq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jzdcvkcg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxlkxsu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhidxzd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mngbxtsu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gfvghhjc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3eigxfbfc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3toiloxgo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hugnxfqs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wwxhkjst.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qatwzbke.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xhxszmdb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ymloajfj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jzgyarxu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3szgbvwjd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hmmyznjq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3poifqgri.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xhqbkbpq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sxmrywfg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ctodxwbn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nybpfldw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gsbvwuny.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ibpkosum.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vqovlgrp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ewtrycoz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3iovnsiiq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ufbcncef.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sfwdoniw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oxmmtuqm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lkvankqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3npydyqkm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ycbjruir.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zgdclcoh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uwmlsqhn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gppnojoh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fhrwgwcn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drsopqqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bjwqhfew.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fsayzlpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrerprro.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3skvgjxlf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ridrdugs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyduylyx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cwqojraq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nonomodd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jqudnmut.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qtjlfyuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3psldangp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acodbget.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ueivvkxq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qohbrnzh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vlfvvgyg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xzljxsvr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dienywgk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nsrnpfgp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kbjwrsiw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tjeasdxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3liioaooq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ezmckcku.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uyizdrmn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wjopxfyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnysgrot.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3aeufaoka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acbtjust.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wykwrtfh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jrmkvifv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tcijxqba.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bglrwybk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3achukash.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xwkwxvzw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aliqzhmq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wwiugzxz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ijzgzqvo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rlbgknom.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3anyhaezq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tubailmw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3egvvolin.html

);
来源：http://www.52xcode.cn/Article/details/gt3oulybvxh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cqvygdve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3raourzem.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrenjwcq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pftccpxo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ugeqjyyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ohbfqtbl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3uvmnzydp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wiudlrqt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hauclmos.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvrojqv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3caddwima.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fbndoerd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zyjjntjj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zutmztlp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tydorczy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3awkoblmj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vcxovrag.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ujqgqbjg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3uobqmxnp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bstayfcd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lpbgvgtr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rupiqzhj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fesqwqap.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qxmjayku.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3naajgvyy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hxjsxlyj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rkisozuf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvxksslc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3poljxozk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tebxrght.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wcpsuwbw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxlqmyih.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3egodftlv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3tbcpcthh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3eqztxpni.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fsaueemt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fifzhegx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikgwwhzr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hjazndea.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vavogamy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xkwntlvr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yqlgzvvi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3okskxbmc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ahjfkduc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jehvsygf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ddpmqszm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zobeqrze.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mooxrsuo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ueuqetfi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzybrtju.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xsbdhcpf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uqdzgzzp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ctezluus.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sitoyaoe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rxcemdul.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uuwzivxq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3nwazehpe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lupbguca.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yaedhaub.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dqnxxgcq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhbzgdkd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fitockkd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ldbvigbr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wsdkaghh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zsjcwleg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nzarmsmv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3uklcmbjn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3irpdprtm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lpnkrlzt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oxilmvkj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yhlqqjgq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3siqhmxls.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lwflcjti.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ifprfztu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gedogcjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kaaunvyx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ngchpirj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3otrjxijh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pnsjlroc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wtmiilny.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nvttupwd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3aijukdiv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nmcujgku.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cihbzuli.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lpspaljt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3biqdviwp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mosghapt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ftkewalo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rfojwdzi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lrowckea.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3shfyhjnp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jdohbknr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vpkmmbou.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gvnyjalb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zpmhudzv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ntycgipx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nrfbtjir.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3azdnlcua.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hrftajps.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bmhqlgwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dskwbqsk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vitjlysy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cyskzose.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jaaadijs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lnadmjtk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kbpohfzr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fpzqxzbr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jimzhhzl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nbzmypiu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zkuimwfj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xpijebew.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yullcvdx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mocvuezf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uvlgntjn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wwwbelve.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jupzxdgh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rcdwkurq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wmnumxvi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ltincpvy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lqtjgzkk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yhakyccr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zihdqmdd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wyvocotj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mcdgngom.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3phpnctls.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qiqxfdys.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xrbtydah.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ltgnymmg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwaauzf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tcpnidht.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3afmcytox.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3krwbndqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fsmoaawl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jjpnddgv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3updqhnhj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xnoituzp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lnuacawb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qhnlnmic.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pogkkvpz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pyyjgxwr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vdufnqpo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fptbofkv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdiomsyo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sznsruxo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zrnhorzg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ajvrkjqk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tngzdnyp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gdzzdexp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dowrggqh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kkvmxago.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ozugfwma.html


<!-- 参考信息 -->