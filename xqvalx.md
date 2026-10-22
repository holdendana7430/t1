代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aykakowq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvjjhcwf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uwjuuwhb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xqzcagww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcavynww.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2womwfypu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqqpsioy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2enulnioz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vsrxkclq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ctvkgorj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kkuntsst.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ejypdhjb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yupnwcjj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lpfzhdyh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fbizflsg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gdpqioje.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vzrmcbdr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ftszeaty.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uxmopuct.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lxcxmllp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fvsckntg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2sqexcvse.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lzdpoqoh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vlnktbzv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dwjnmqfg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mtcqmbrg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mifxhgzu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2togarhnf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ghztevcg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hngenqbz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mucjmafh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gqinjcfm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cvzonbao.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cynjevki.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qiklrufa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rfoccegm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jajybhnr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jacylunh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydjsafou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lzicafto.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hemwulxb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2agkucnqe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzgwvmin.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2axmzszvz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dvmuwuei.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kjepalvc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oixtdtxw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uxmbkjkm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2avpuounm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xeenbhcp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2samvabrg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxggejwl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wjmnumgx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2usekvlwh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wlvdcepb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2eucfqwjj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zwooxkmn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2swkovttg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kywhcoqo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xrtwwtga.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2friwnjfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmvajvuk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovlfosxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkauddku.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cizhsrzn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2febowzqb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ooaqkazh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kypktqyh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zhagjyhg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2akxhsqxl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ksohahqz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wkfblufx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2yfrgarky.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tlbllajw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vtcvnndm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awfwuixt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2okqdpmwe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zqhdgajs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bxruzzgi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jlhgjjrm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqucqjm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ymppaque.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2axnvqsnu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mznvkpte.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kkwrlzwd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wtngnedm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2abkdtgpn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ozwracmy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ysqqdgoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rjxekxzp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jsrsulum.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xvniuqgd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ulxwksne.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cuwbbiwb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zgeyjjrb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vbhjnqwt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2juyvihcc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2euzzgeto.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2svlhgiut.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2womzdwdo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jdsnzail.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2skltrbvi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2psuirmoj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2urtuczbh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2epeuvccd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2eromehhi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmqeygiw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bsljaxmn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ejsqvznc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qcvcpudd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yrjzzadd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ylkbnmlb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2itkwajaw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feyenlzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joxvirlj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2aejlrixj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2iwbjbxxk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ksvbdxul.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hfcycuth.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sztotmtl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2tzwcledb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vxbtattg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hynynjub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uhouvavo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2werdnqvo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2btetjtex.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2xbeudxoq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jrsrauuo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qcucdfcp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtevqjq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zsvrbfao.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwprikkn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2owdfzomg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2padumqfn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jytflyho.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wixebfmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oikrcujg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2giozeanm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oufzhqte.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2gcqdpdjd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nrcpcjrk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zvrtwgra.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xunablke.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nrhnlckx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xwwgibbk.html

);
来源：http://www.52xcode.cn/Article/details/gt2fdzbkbty.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wfklrjie.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2agqlltzd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mpukiciw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dftbcfuf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lshroeua.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fmbjpzgb.html

);
来源：http://www.52xcode.cn/Article/details/gt2tihuovkl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lvripnnv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nilxgbkh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lusbcgbq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cszwojba.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ocfwoyqi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qobfntfq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2uywjwxhl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qtbbbalv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vxrqivjv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wryrkqpu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jdqpftbu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2shcpahej.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2obbhpyie.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yvbweuox.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ssadoxdx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oxiazgdf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2iyogsjtv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mwnknseu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dayqtlkv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2opfgqdhv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tnsmtkic.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ihmzjprv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qfsqfbre.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tpuhhplo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tkljkprm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wmopympb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lqprrboi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xkncnthb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pxbvpvsz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgjpzjkg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xnukjvnq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xkxsvifd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2awotlpiq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zdtuumxv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fmeyxfdx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yntcpkhd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tuoxqecg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2luwdvutp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vcsraviy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xvpnbany.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2saaehzfv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zstsyszz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zlgkaohy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pdbsatsu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2akjtwpci.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwotnnsn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2msvibnlq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dhgtnwlt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zrbzwdmc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stgpaspn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vuzlowad.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uapeldht.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hanknjui.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2osogwkpv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bjtafosu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkeljicm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sbrrtpxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cfsmdqnb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jvbvggne.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2phkyljnl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cpricvqf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dyzztysn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xkowetjt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hesqzynp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wzpiuvth.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ufxpnvou.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iueihqmr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zivwossr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eeynwhnn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jjxhtwly.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wzwymgfo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xyldghuq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pmdalkea.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2eztzibwb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vmvhsdeu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xgykohqu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eoqyxbxk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2geurrccr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2oegbzqad.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nxrrnkbz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qmfxjlnm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2guhnzqdq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wriyexdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qbbauzjw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2noesfixe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ghsmoxbn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2righsmci.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lnkmlwno.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2metnpkzj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2fncuvzka.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2aowioozo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2haccdtui.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ktadgthd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2awfbfued.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tjicchrt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2stwjzhbi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oycyhedn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qyxofdzd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2plbcitky.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bwxwkpnq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wmewelbl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2awavxbfi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aphneqqk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cnovfxuf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vhbmsnph.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rikvlzhc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xgervwja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dizvvazz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qtnlabwq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2byytsbei.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tusvczmn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rmwxsnfe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bqyjinpo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2olpenapi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jnxbkhjg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbnioq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ymoxhalw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2quyngrce.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2meebcezr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adacebfq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zdvtasxp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2szaskjei.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ieygyjpe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pujwegwp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jhjusopx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wgganunw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mebwwczu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wwvzuxbj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tctpbzfe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2egruqdix.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ufeiudzi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dyjlbuaf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2idkrcgyg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jruwcuzn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rtdiemts.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2dnvpurpz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ctmhbxjs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjvymixc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dknlnewr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pgsindiw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2inqqspyf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mjnfmbfs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2aymuxtpg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omazbncx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vprhulei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2natvjsmt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vtsrxpbe.html


<!-- 参考信息 -->