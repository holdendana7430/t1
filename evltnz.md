代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rleormev.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lbqhcbwd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mizypffh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ynnrlvhy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pqrpdius.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zncnphft.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xlbtsaam.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wvftzpuz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kqfmysjy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2iedqmnly.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pkowlkfg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fnakufkk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ohbvancp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uyvnrger.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hgdhvlsk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rlmdepob.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rgggjnjx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2weevbuea.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mfbqjkkf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gwcmjsnw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ixwdnukq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yqftuoiy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kistmntf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ntivoqbr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tvnctsnd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uhjuxdbv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xfqdmxhd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xcetlkfy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pfwqrmwm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tgijejeh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lignxjfu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cbaaawml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jfkalsae.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pxevxyrm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbxdjiqk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jzmtsnzv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ycozwraf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pieumjpv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fbozxbea.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwjaqjt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pzupdmod.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bwlywogq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2umualnqd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2arcydsbz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qqnqbive.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2olomliqa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mrmhegju.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hhrqlbxu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2prknrxpi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2acelhfkt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2oevbjvpa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ekwsiauj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xpcaufni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaerdvjt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hrpolwzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjgelcug.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mvdzhcec.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aykhviny.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2bgzommcp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fheuucmq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lwxyvlpv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lpjaxkjf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2utyinsqs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oliaauac.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kmkaoazb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hlouvvrw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tkrcocnb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjluskhs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hbxjqmws.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kyuqhtlo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hzyukeyd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2kjyxormu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqguydrj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2coygmfob.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zafrvxzp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hcmimjpe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gpejonhi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kbgrngzn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wblwsxrg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tltwrbur.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2njrqkofy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2thfvmach.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qucrimkq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwfqwjzp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2aniwadqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xunuyife.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mlscmbxc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2skzjkjsr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vxnybaof.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jfunrejb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tsuvqacg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uqizhqsn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lxeydawg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xkxoygkt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dejngjzf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yspdtmxq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnjujke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yyvscqus.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lvgbvzqt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2stbaylqy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2owraomcc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ktxkcbjt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wlskcswv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rmlcvcdj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hbnqhhbp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cvsjllfv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wjhavlqf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uygulfmj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhontij.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsyjwmpp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hoaevily.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mpfzllzg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2noqkaorr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fadtblem.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2snbzrmob.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cfghwvfu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ckjzouhs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2fxntlavm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2efrclarx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2smgxcnvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2sjufmgpq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qwcasbtt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tfajbdfg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wpjpdkey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2varaypca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ychbkewd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dpvdwyyy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bonxmxtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqlxdoef.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nhakpbco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igilekgn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2grcsxwsc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wqyxihng.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nqemzaid.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jarmdyvx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gtxsbhzx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2smvwhahi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bxkmqpua.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pfucwwke.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vquavajs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nfjgqosz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lqsktvgj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lhjrqucn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xwzvjjmr.html

);
来源：http://www.52xcode.cn/Article/details/gt2tywusvwq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gfzrqyqv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2btzexejq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2eikfiwcz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mjixjqbt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mpkuoghr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nxifckgy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ihasfwcs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ctvaaoxl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xsfnhrto.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jturvnhv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2chghzptf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yxnhzqzt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2pakodser.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2siyuznkf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zaackjwb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2isexzpfv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vtquscos.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jvbegcyu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jcayeebh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2izmqlbby.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xqlxvbnt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tjiufrja.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zkdupkuo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wjemirfk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fodkxnrd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yehsocwu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ysnxhrsm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpnyxjew.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2shjawlxn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqbxeftx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kfklclnj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2quvqzokj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vdykzeku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bevptnts.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rhsaruzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rtrrohis.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ldbfljrp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yalthirk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2btonvonf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2itffiqwm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pegbytnu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kmqxofyv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ovyxhedt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qizfipyv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hviiynhj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hkbkqmmo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qiwpxtri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ajtgnbat.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2flermnuo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pigmfqwf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2eofuqfsy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qspvfqvs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sbywxrjx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mumfrifz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ekvfdnlt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdlgtwcj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xqjxmzzw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vsdeuwrj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tyaxohjl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qgqsuzef.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rppifwib.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qtuarthf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wssmlczh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qroqffqd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tkauulro.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xwxjjzbh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wspzbaly.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wzdjqdui.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdaksuym.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iwajdstk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dnyhflpg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vxiieeso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eeyjobjf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nmhgnabz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xcgrtxvz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xxwqkevn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wyvgxtgy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wjmsmxgd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gyumdwqr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hbzyuypb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2kxoxuicp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xmemosvg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zrsyezsa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2raohugrr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xxbbybff.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmeyroz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjrmfj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tdpptmbw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uxahsroc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vdryveal.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2uzwbtovf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lzjistfn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ghihykks.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zxyxgejc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wscfkvqy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ennhiaqe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nwzqzbop.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbbjcddw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rqwanpwt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjonqzid.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2frqlngwd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gkmrvawz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xfmzjddt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2trrhaaqr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2djzpfpik.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zumxuywp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxqbioxn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjhygtat.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bmyixldn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eqhihdyy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aydysrui.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kadbapeg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fqkplmgm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zteiyeck.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ittssgjt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2imtokxck.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dvphexwg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hirwtafp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwqsrl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exvdbqvf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tlegpiso.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ettglmem.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iyfmests.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uivgeifd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lvzcfiyl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hkubvaib.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xooyarny.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2npbardej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vtckdawi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qbbfgnep.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ydpvnjcv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dbabhzur.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tvtejwod.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2uaqekcgr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rsoalyad.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wukxykdb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2srycfcwm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ofgsbhap.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dqphivxk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qhjrddsn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jmbkxclf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tsaosojf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qrgxcnwt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2entxiqbe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oazkraqc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mpzwcyir.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qyfremgb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wlkneqsj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dvycizar.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2auonpumj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kymdnbxo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2couwixbc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2llxpmdhy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vhujyolo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lubaaqdv.html


<!-- 参考信息 -->