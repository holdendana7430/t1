代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2oyyczrbu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2egmtdauq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jzdoemvq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gtyydtwf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sgycydnk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2luyxphep.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aitsjyof.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yuothajl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eqwqzdmv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tlmxnpry.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yiylxunt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nnhwqdgj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uyxlrnke.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rafmlyko.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jlhwabqc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hvzonmdd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2plglllbx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bbmanmbl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qemtpooz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eyifvine.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gopcfsvy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnctqjpm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2muwgjgwf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zwoxydhl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tofseupx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylczgram.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hbqbyuxd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pehtnpco.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uffwbgqr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2essfwolz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ptvhmmhh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wcpufhwn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xzbjhszj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fywvdvmz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxzhpjer.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qyidznci.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2humeuzyp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mpnnarzw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcbjvgl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oofgrywx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aeuyzvkk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ukctabfa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xgftdkev.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ilipqkwj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lsolqkrl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzkdupw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tzhtjncq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wlooepkk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2inlslbrm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ingksnzu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fdhkuhfz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fwcrkliu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2skjqbqas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hggektgu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhggyubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwcnzamo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cuenpwlc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aftixfmy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vlhhlvdg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dyqymrvn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kbosmlai.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2djyhzjqd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bpooukrj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jucopcrz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2chiseuba.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2apuitacf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2inixqufn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bawqrvky.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2uaebijwy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kixcgohh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wxpxuiqb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xhejhzat.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ijvvnnlv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fobfbzut.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bifkunvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lmitojtx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vskxyger.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ksyslnsg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbnlkuf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jihetqgx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2teqoaigl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wmtqnkrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2xtshsxrh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ogspjjsz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2uqesvxjc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zmrghycr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jldpofcc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iehouopx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2egujcjez.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mfcdqurg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kzkquqqe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ineegzby.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zypvhjet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2drxuvtjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wsetfrqe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ionbhdvk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rksyeulh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ubbsjlue.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nbqxrife.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rfitpgfn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2zzazimco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2skttauil.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lomdbmha.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nhsryeiu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tlvrpioz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fwnemikp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ckypsuoz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjbomfew.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbldifu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewyndlmz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ipepdbjj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cmqtdesd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hxtyiogi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zaajiurt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vrnkhitv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2csxqdpxv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ktdqrlbn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iabmosct.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qfanxitt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2atxrncpz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dynmyhch.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iftkqpmx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wavolmzu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcuarr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2izsujxmr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pajilddh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lhpyause.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2nezyhwkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyxmkubz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bpjnrajb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccrsolub.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xtlsvxeb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qfhhuoyv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jejvrjxb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tcbsxscs.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2burkdagt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ttevzycu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vyzfhqot.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zfoydqee.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ucblhdmq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qryxfqob.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ucejnbsz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zmuhkixj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2grpgmfqs.html

);
来源：http://www.52xcode.cn/Article/details/gt2wbcwqjud.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2esxlzqwq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xutwemvt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2aikfmhru.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lchvocdq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gpakqrbp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2murbfdxx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bdjvjoyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnfccpd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qmonrmfy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kfguhtpj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2goerbhia.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iebabbso.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2caautgqi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ttfxajoi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ggsnoycw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2deuvasmd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xamzjgsy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wpgzijrp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2psribfbo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2skfrsfve.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ecmhxpjo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pxcrzoyx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2amouuvix.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uqbgvjln.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dtqodmah.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xqpzuabf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pffdhgur.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrlsuxrw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rauuhyfm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ucxqxlut.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2svtslill.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dqqxpibh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbvrezrq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sqwqsnvq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2atdiiwtq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mgsellek.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lhhexnri.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vuulpfgk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eijemwch.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wafscgud.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yhxgctoc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ueajtiak.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fkdxxhsr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tydhncyr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hdcxxdvp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnzuuql.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jlluszlb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wrrqozkp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tupnicat.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfadiipl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gxnnkeji.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgvhipuh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2keiarfsx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sxlguofw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pxsprtim.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dszwdfpw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dqyitfny.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzzujxl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zopbbsjq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vhxrurqq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cdyjfjsn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qtgoupry.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2byzrgdtc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nugqkejc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ezrnjmzl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qlxokyds.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dmesjloh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kqxakref.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkpdsnap.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yptgbwjs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dmcnscyb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kdvbrinz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2shjnbplh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrpastjw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2alyxxpua.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2sdrthlnq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hsoewfoy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dzxojvcx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2futwdxei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qritwwjw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2apwocutq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zqhgqtrq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kcwjfocg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fvmurtwn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hbxsaufq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vynyzjtm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2wwbxtqor.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zohwszca.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2emcyrlbg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vkndgvtl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2gzxkhxyn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rkpozxad.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2otzvujxi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ldrmgqfh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xcdexonm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mvbtgbsj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ufdktfoc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tcxnwaci.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zuabnbrj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lzhnhvrw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jlydmvdf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2abtebhlz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zlyesxbz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xgkvbmif.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tqwqceoa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ptuxjyta.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wxzzmjtm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mtzadqkl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2apukurjf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kkbchawk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2obpiriof.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ugonvukt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vpjokhzb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2shdhjkbb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pppyfpmc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sbyrgrzj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gmlmmlbl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xxyhvsoi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfcmsp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrxmooey.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xfkoiffa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgqecbxy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2diuvtfpt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxzsyvzg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rqkkjmnm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dindcdij.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uphldexl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xgnianvb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2optrsauw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2czkutdwu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ivsfzdwa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nlhycrmz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jmxyvpau.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2pdhmytrm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xezxssgv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jydmmyig.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fggasfvp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pcpmdnkw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2crrlolkf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vljfekwh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kjtbqobq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xicvvskt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eohxtdpe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ulepuayn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lkgciekl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qvbvkuts.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2zhpztgwc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibpfecbd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kgctqtzp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2arexjdtf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xbpjruhh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eabrjoko.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fgyqnkuy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ilegaytt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2suzgpeyl.html


<!-- 参考信息 -->