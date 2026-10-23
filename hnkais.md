代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nvbavhhk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xdehkwaw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ctgndhfl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qgibsfqh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3axfoshnn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ieaaiehi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vdcvhied.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3xqtlfjfs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3valczjqg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ltadajlh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hlhdhaco.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wmnhooxb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3llxqzooe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qwfwrwaf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gufkaceh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lssrpriz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mziomkct.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lxtbexzu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jughurqn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sswtxrho.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kabbgiyd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwnjibxn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abpmrova.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wlaqljnf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vdppegmx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ajciczyp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhczgyag.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vjmoajeg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rdowbjtj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yosmttqd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kjridqgw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pwtprhtj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cfextrza.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hgprxeby.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qlotjvmt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xoxvdbna.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zlkutdbv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nynvbgld.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kiwrymrb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3emhkxnld.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pimlrhjj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bewtdqhf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rinokhrb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xmjciwnt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3sbxjslwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cusxhfit.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dhkbibuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlgtzzho.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3juhtmfkw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dkmshmnp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ioqiosmw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ohvwymxa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rbyctlcs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mqpnozfs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zansdyrd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tbczdkal.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tyaslwlc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gyyrdbwq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zrwehdhr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3giwribzk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3braqkeef.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hwbdxijq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mbmbpozn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zrmxoitu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbwukhz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xquvzkor.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isnlgjrm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3owddrdbh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ygumvqag.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jzzjureh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gqfvuqtx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcjqrad.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zyizrehi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kwollncc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xrnahjbm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bgqofjbj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zmurqjax.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obhkkblv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rfjxtahi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tqqinoai.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eyfzeorg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3evhvcidy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3nfhbnlyn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lgnuzybw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sgacbcxb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3nkcyjsfp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mkxifquf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uroimrji.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mnglrvee.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jgqnuqvc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpkbvci.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3csrvyzuf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3obozuiar.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ifixybxj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fdlxfmwx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pydkelkz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zprbtama.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mavbajpi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtvmchla.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbdxuzcf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkafhsb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbkepkud.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lqayaaag.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3neyeffwd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nslmjuii.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ubuguolu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vmbtvwxm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xrhtqcoq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pdrbxbxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nkamande.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fuqxvwxs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ambdgcyz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqkfwzh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ajhnsvez.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jjmfyrgg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wicsnimp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3klaepwtq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iapdgjgk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3knskhbrr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eprvvctw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zszwdqob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wbknlgzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvfkodcq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3imatvqjc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3byejuulv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xsrltcid.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qyhpmueb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gkfxmhfa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3waqpyosj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pwfskuvx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3sstwuhap.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3oiiqytdf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pycarbcn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3usmnmqcc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dhoqvupw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zdyvkwed.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kdujuevg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zudsnbaa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3agffvmsg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3rwjfgvnp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3guoveise.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mzvbcxqv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rkyuasbf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3oeffvaok.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3btrheliy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3yqdhzoay.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3awdxrjzj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ngorkmed.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ljfskbqv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yixejxhy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hriezdnx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ujnviqjm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ydwlbtwc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kazlhyru.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rgwxblkh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xagvxqqg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dncfpuaq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xsbtdshd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3llwxnrxp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bcbzkzky.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yvollbxh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ppwzraky.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kekivlmp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qtvjwdbk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjhqxnja.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3patflamo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgamscgu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kjdudsqi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fxrbpseb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zrjnxzyo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wdqxewmg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mbmopwxa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oxhjlmey.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dciyszjy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ylattmle.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vkhaeflq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jpelstjf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rlyflwrp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bwkaxwsy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mgyfwwzo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3eaaciicv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ajphmuyk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scynuyxc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rxpokskz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cbnjwfbn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tumroxfy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcxjdbit.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yqqwdgne.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvefozxo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kyblawel.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ablvtwyj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jvqetejt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vshkqjey.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3btudvvss.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zhncghhw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxzcojfe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3solmnmvo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3udidllbb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ksdbqjtr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3muqabnze.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qcaptldh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3eldqcxss.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qdvkefce.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ilohhlbr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3imhpigib.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3posozynd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gjgngpup.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iesdinur.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3riktopyk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uenahgvx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vszwxyhw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ncoyemfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bkzbnexc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3muacshag.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xonnozxo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rvhvomnv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3aasoeajo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pupulndl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3imntnapb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3oeqqqlkt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3obuhrkxx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fmdsckcp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wibvlras.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nszotrjb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fwythfew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3phrbesua.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sthugcwj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nrqgmuaw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tdurtpwv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cmqrvbry.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wskmhsby.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iejsohik.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jiuihytr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jnmwhjhf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rsmcmzul.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dcndlvcg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lrxxoqdj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3yefzdhyy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3dltqbktm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zcgocpql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zvoyoobe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kzblfdnu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vfylpuld.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nmfrxsnk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3crhdaemq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3opycqegc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tojhakpy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3quuibtbp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3swaugjrh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cxaggtsw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rvqtuxsd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kzbaigyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zbpjzbkl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ekgigzxx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rsekgyzp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3htfajcxu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yectjapj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ktstuotf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wjvvkzbe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uazztrme.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tmqlvsgy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qbmookwu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qwkkeeoq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wsyiykza.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kwzutare.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fdwpdmpo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fzwgenle.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kpudpioh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xgvnojne.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fcsuojja.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ijtbtdca.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kgblecym.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lsslzjcn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ajxkxpwl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3stfynthm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hkqikbza.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vjabaahw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dztncxqa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3auzyxcvj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bhrjgxli.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vehjylwy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dcpugoyv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3noibzcph.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pliovree.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tfseptjy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yfztuxdp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tlawgcej.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pezrkqag.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkszwzsg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3eyeoumvo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mbwfwpil.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sbulkcuf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xuotnogl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zndjskue.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cwmxdtgs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3omuhuqtq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3tfcbbhpz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rzqytcbg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ralioygv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vgselorr.html


<!-- 参考信息 -->