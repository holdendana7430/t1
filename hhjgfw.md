代发 wailian999

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2glumignp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uwthrfml.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aqtkfouq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zpefwwwx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xnlkgzkv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fdslfeie.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vwrgiobg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ipyxnloe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yuamnuxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgnrolq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nzljswfl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fhatbxxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xowanbis.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pvetwwgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuanehah.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yrefnmve.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jsssckjv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yqjllrav.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jefjvtob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2stfasvds.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hggooqkj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cksuhgtw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gerovpyu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pszyofkf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sxxbdtxh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yyrgdmvh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iobkhsgi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2whmuiioh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zbpzhspw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyzhzbs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qsaiavgb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cvgmbhcy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tpnlfodl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2riwotbws.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mebggrvh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xonbrdyv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qpxhwmhw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xfitxqnt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tqbnredy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ulntxyux.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kdfhlddb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqfzuiv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rioxzewc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2axrgzwpo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2eenorwgm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2watpegtu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxtzcedf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yahakmvr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yqaybjzz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zsqvodbv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zwjmtpod.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wxzgjtym.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvxvdfc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hgshuxha.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgrkioa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2emlocxzq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2winmhudr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zpejijta.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eyawuljf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2twffybqj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bwrujlfo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zrafajmz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtkekxwi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rbgrunuc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pfcpnnhn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vtymoxgq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tjcgichr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xlojzpuy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fbsmjboi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbfntqqz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fybsrepj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsayegju.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dfoobvhr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2alwvpcqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hoaesnqq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dpzmythk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2alfkqcum.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2apkmatjo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2goxzepli.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2uazsxgfs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nfdoqxjo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2eonqcdzi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2sdyuxpis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmznlouv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zngfidfp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmhejjj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rznmsfds.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zeujshfs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2eafbcfft.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wbcronjw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ufbripqm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mpfwdgju.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2urodclel.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zastaqcb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cynopfxl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpxtblg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qehdqdbn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tlrzcaip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mxatzrhq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uuyoeiwh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zpcbmzoo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gnqjskqn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wiywfxql.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bvdxujts.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fubxkgll.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ncvytafl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vskdbhbo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nftsuxla.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mwfecfln.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yjudfbzj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wbsfeozy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2edhfrxhz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2plcczdkh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2qmnmslnz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pbpvuweu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uibfplig.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2azqzuott.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wvvwugcg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2eowlbchk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhoifwaf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mvlzbvsy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azaafabg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qscntktk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjbrklns.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xqbsqsvb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtwrciqq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mkmeszar.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2brzhawvx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2tumvtmtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hprhbcvt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zyvparvm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rcqfolox.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hyrmxckn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bxhykuho.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2amrzbrbe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tdwdwtcs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2spdwzgoi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tsmlndse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2erwpmlxc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2frrciusq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lkgvmwwm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zdvyxsju.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wargrvrr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2siglqyxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcrqhmhh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fuokdsnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfnrdvre.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2llecflje.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lrmajtzy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jnouyscz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tmoopkip.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jrfjdnkj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2xvsjglyc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xfusyeva.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2uayxxmvj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2oiowvkhq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pcpgggrl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jwjqtomf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2swulrsjt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2kwtltmic.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jshmwgzd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wnsepamz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2geqpqleb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2sdbimzog.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ueibqkbp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yxagvjdg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kzlohfzg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pwyctjyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mkdusxfy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2aiscbrsj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2megujtub.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jncioerb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hnbudygo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqkdxrvj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iaockqev.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2iiofxqck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yyyyvywz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mvblavdn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uatgiwrs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kgajdyds.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqrzpo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rpexcflb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kyyrylpq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2viinfdzf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vpukbnmg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xhknlmda.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2udsxkyoz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hbvkeqhs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzhmffnb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2izgoknhf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uyqynqei.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2icphtcqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2sqahantq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmvbnare.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nfmcimzx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ywigzirf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pywfesch.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2skuafnjn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cxymglkk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gnjqcuzy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bjvoiedc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rfkguujj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mlrnigeb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2siwaqxvd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wtfpwbae.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hnucatus.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2odzgmzew.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qgmlpjnl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2iqbvhljz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gnyfuhwb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvgqzpjh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qqmbxmzj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byuqxejt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ybshmxaj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mlvqhihe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zibbplwd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2leyapien.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2urdvdcpr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iyupebcp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2giyzyofa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ezeskjwd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zrmmyruk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tycevqtf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uhouiuxe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zfidkivt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ehudofrb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rtxenity.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ncvqcico.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wuarqsnp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2khiapbrz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ucictilv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ujmxrozi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tsckloce.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2higcmkfq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2lnjtnuvz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2khbsvifu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hdlrgtyb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pleravnu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rnrfsqbc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gsrhepqp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jlnugcpd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2unjhpqei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nksurcjt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dpvzxini.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ugicskyn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jjlaklst.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yzxxtdlx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2erzepudi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rgrxealx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ueoefmci.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jxsvrxnd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xnqjegrj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2frhwwcbo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eiiixarw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hqwcymyz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qhgxhmrl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2pbuydvsc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ispewvck.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkywytzp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tkopwldt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nhbbtjlo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yxciegnb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zflyahpb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hjmxgbul.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxedtn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wzxiyyhg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cchvtplr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wqeguqik.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2corrfjfe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2molmpgws.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kqduxlbd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jvumecfn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xxxybhwq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2suxnnsir.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bppatmgb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sunnqutw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kvqffeck.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ousefpvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2undpuzny.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qnrkemqp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmuylawb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vumrdnrg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzqbxcpu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eonaulzy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jsbmbema.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uolgbzxp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uejneywz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xjugexmi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rzkxllom.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tcvlqzos.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qimtsbqn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ncwifost.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ovblxuev.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2whmtbhpw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2chksmxhl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sowzljkg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wypioomi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jbuposch.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gnhmmiwl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2heebfzvg.html


<!-- 参考信息 -->