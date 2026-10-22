代发 wailian999

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2czzqjhfn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rictkdaj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kxmkmloi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mapjrukn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2remitllv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ppnvmdqo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdgzpdcj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ujhzhpva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vrleggog.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2eraskbcn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2biolbmyt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jfraczwg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fviizlnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lnfnifrb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lqkjnorj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vimxnkge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnqdkiox.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ngsncsom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2milfunhw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wwszpmxv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pjadpzmh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hgcvvbfv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2daafsmgz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uxpcjrum.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jiogkhdq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ylsuisnu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2eoowejzi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2unbnrvrl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uipswuwn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xyyrdxtx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dyxvqshx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dpeowxyw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wfwryxtu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hvvzibtp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nibrhicm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pqkuytoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lzkgjpol.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ghuhtotp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xazzgqrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2llrrevwd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vjnqfhqz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nqagyeat.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrwdaxk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xtkeijlg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kiuqrxdf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lppozulp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fiztzfwp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nwvwypvg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vecshwbj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnytwtup.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qxqmcdzt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zhgjgxfg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2scbmqhof.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kyhsxafy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hmpfvjyg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ttjzavac.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2sjxpmkaq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2medmgjmy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pbocyyfk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrmyycr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wvkdpqta.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tdafsxbm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2orjzdyvh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xgwhizkt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wngkslcm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nogosmll.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cnvnbllg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hucigakc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vmwymsfm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2whszmlqy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mmgktbco.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cztowdgz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2efeyqkck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpnsvzhn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjcbnxbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heziviuv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2njfyvodf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2prkhlmrg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gerhghmm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wabldoxz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2czipuvwd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2csfgunho.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2brkgswds.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gzfimava.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2koklhptm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tdnbdpgj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rxrmsupg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nkwdrjqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwstti.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hmizkhps.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dgluydie.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2unnjwpfa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alxvelpk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rbtolkvd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zykfqgak.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wmxulcyo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vbrmlumt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2neztpshm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hivsyxfm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tpiejjkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ypzxidww.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmcpiqp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ggwymoxl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mmukgqxt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jfyhnghy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ztqaauhg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2khcjwcug.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jjotmbbb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bgmbejdn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bgohcirc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nqygcgzk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bcocekzc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uijarvnf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pregslbu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dusdysle.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ywvidaim.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xedrcnoj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sfdifygf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2krywpatc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zkmghmgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hzwvmjjl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2crjfgves.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2agacwfyw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2witqouhu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bndjdwga.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdllksme.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obwsjerx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vbbxuqzi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkpakun.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jqzovgto.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2quocqyqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2galqrylj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kuaiztdi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dzqfyahh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pfnldbrc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wcmoxtua.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kjjkfvjg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wmlrclad.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zhhgneum.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tfruxyji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zmfejilj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2komjndbz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2frbsolvf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mtzcbjkw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2aihwpcwk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kgcxmosw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fvbcndou.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uxawvhts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdjakrpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lweattdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spbxqogo.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rldgktpy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zxnbfeiq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2glarzprs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mnkfyfkp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2spcszmod.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2glzrsroi.html

);
来源：http://www.52xcode.cn/Article/details/gt2pncsukmb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2igiijywq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ungebzyd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mbrldopm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rpcvxiln.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rbvxbxrz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2owwvuvav.html

);
来源：http://www.52xcode.cn/Article/details/gt2fssypdqw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2pgnpjcty.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ybzsvvrt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qklfhzsn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ykptpfwx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2orhjiybr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2odhjthaq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zoxroott.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uflneypy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hitmuyst.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rhnyxyvh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ngzyrftw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kzwcuhgi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hfykzjgc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2exfylafi.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fjbjncih.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2idskigky.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2mnidbwdl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2onbskjsi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wdyoblvf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2etgnglxp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2izyampua.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gcxedqbh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ltzlfajw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2axppmgjn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2jvjduzre.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ildhpdqg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uuqautxx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsvrkrks.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kyoxeyko.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zclrrrtz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wmfuilwq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhsdlnt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xkijuupf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cmsqcuuf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qhapmciz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vyhenpis.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2krfnaita.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gkvqxvrv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xixcfrff.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zmxfydch.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2oxrfudko.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2altfuwsi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xarnegid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oynmmbvk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2crcsssiw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sboknulo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dbbgmrwc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vcotiftd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fgtkleud.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fipbcsfd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fglgyqhi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdvktivt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gxqdhmbw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gkveulxm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gmqhqtzo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcuviupg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2yrhdhlxt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2djwvlafe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mtygbqdt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2biofsnsj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zidctkhs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wqzrvoyf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ndbmbbey.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2clwdrohm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bxyezmjh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dupgopzl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2gxezxkxn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2potrdldd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xeeqoyux.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vjovtegn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ormpmohx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bmlnvark.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ryxhbsbd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2eywzcoen.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vrgcsdpo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2upninrsz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wyislxoe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wledkrtu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pivurfke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nfopvwag.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rxkdoevk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cnxkssvt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ftowyjln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2avttlibg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dbcbshpy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ulyaijbg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pmlptick.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2scjvvqoc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gksqzkfk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gbrijvpc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2flvsmlhs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lbgmqvej.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mninqoqb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2milzapes.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rhvkcaxm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dywtrnok.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mdcngbuy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mfhzzuok.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ofmclqdl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zojrbyjy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lhalrvld.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tbaebcpa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2otebgdue.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vqnjsqjx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vipbmihq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wxuiyjyx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2frcwilae.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqnbbukk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jppswlli.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rduthiti.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2utnwctde.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wjyyuwbu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2huodbdrs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lodxnnta.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2achzbrkr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lirnulzv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zkadqixo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nhudvkhv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wklgjrof.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckbadvlq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sednrrbv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2euiuabco.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2shydczdq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eyevcahb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2mgtqgjnv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2notjsvql.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dyweaxjp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bluwmakb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xvsmubfc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zlxljmhm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ozsrywjs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2sculvxbd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2aiytnvlg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2drtliqrh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qvlbkazi.html


<!-- 参考信息 -->