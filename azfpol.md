代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vjfwjqln.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aduhpetq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2russkfcl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ggukqdyy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xdynjawy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dntgjffw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vzkukgeb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dnbvssnl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sxtjtzbl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vvkjwqjb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qeckfzsn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2suvmunka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oghwtrgp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zdhdkgqe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2evhsolfs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nonirmjl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mzyemtvb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vxuakklg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bdfmntdu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nbghpmna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkygclxd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2brkybpyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhjhsfqx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2eostczwz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vixfgpeg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jirtzqhq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hmlfbwhy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ikmaiohb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tcyxniyp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2urzyxtwr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2komwvssf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vyndrvmk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iibivais.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vokmrpbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2esyvbyaf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rtlbfebb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yiwftkyc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kiawtqdq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aqpklblg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rrzfznqz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bdmujhce.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hjtgstoh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mfjxihqr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ybbngbzn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iebunfwh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lpgwxsyf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jedvyyij.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xacliupl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2atvzrvaq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvksipk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ohylzxbe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hhfurunj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2afgcefmj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aklajvjd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2odfeilay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kllhfpve.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nvhnrsef.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ieuagyfb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqfgpwk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2oynqvtdt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgkfnmt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gbrwfton.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjwatv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfbjvnj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qzztwlvv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2htvmifmo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fbueutgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fmavslgg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bivorgsj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2glhzswcq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jgwvbbyq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rmdyvmhx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fgkelnzv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lzgwcmce.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kdhitlkt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qrbxakhe.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ojylpjmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bljfuytz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbokxbxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kavpxnym.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hebzonqm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tqbnture.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zaoghhbv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2khoyvdlz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lvlnaqgu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jghsltby.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eleepmed.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bmxyzcci.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vkdyxvap.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2stwjchzm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dhltolps.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ftjypguj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2cwwbrtgl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cebhymvh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jrzijktz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jmbvjcdf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvnrlhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2mxtzgaro.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tidotysc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tayrvmhb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2glkfzxqj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhfdhxpp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdefpjxy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2isuoknhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ctpclrup.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ialrngom.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wphpuogt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hswxnxlg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eznzlnfw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2prvhwzyt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zzrdsepl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xacqhfck.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ccccvxiz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbolypu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2awfazfgc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ljmylxyv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2apqtlsmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yteabfkx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zfivbquh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2nnxilabd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrbtocrd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ipgdsutb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2chfopkst.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fmkuavla.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2rilxzyls.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pqrabshk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dexagmjy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shtpfzas.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dkvjmubo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lnjubekt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypjniayx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2myjhjnpy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lawkieud.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cigybnig.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xbiqeavu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nccinpds.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2asirmnhw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2anssatst.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2afzmmuby.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wmdyblaj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ohvnsuiz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pamidfar.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2afqgwtwt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rmkgutif.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkxmqdd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ltpxliws.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zacpurbg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mmwfrxkq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2updwpipr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2iinbuysv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zqoizqnu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2flggksxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxnpckin.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hdcjjnjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvviiqvj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hraxjkcw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xyenxbwh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pljhgqlh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kyijcfcc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ulvrfxld.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yiibnqyn.html

);
来源：http://www.52xcode.cn/Article/details/gt2guyqpisx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ktsdaqhz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vbpdvzik.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2guirmuot.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2srtbyyzw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pcendayb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zvcajfzj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2glxwrpdj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jsotymju.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gbfckdtz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rpgxokrp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2upaxiytj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2sqbqeyjy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rdbmcaeq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2zyvznvdu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lwcqgorl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ucllbucg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ckuyfoev.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xiisgucu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2acunehug.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uvknjhug.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2gfnoqgvv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vxsxvuys.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2beicrtav.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2tsfpcjqh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qmvcppen.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ecdcerzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ysfxzzkz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ivsjebjt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ugwovrww.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zvdrbwqv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zdmlocwg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2esislcar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bhdiymrt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2wtksxuww.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhgnenny.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mmrojfma.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzqsusqd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2sarwuvim.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iesdqlos.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aaezjuxq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qqnvyutm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2oqpffhuh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dqyugbdu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2agftncue.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mtzubokt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tsnzmnup.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wpnjvugy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gsmphaso.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xijsjork.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2notobeep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2doledsgk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ltouqjgv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxbhrfza.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kbxvlorb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pnqvwxwa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wlerkqfk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rtjndrvz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bvuijvma.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bfhjjdzb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lqlzmspj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yncnqwrx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vhfmhtbj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffgxnyrh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnazqt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rcwiazfa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2sedkobuh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jwyicrox.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hoidmjbp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iydheyzv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wtdgyrcx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bujdqbau.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mfeoldcb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lpwlzofi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2umjrqzhl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ybllfnlj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojmnstmz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2yhxqypas.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gihnsgha.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eklcbuxi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2eygfjyzp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gfdlildg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cthrgnbq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2yfkjgyac.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vvsvgrwv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qsrtjlqf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tnhmgnqx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fxkyueyd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2turpingq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fpldlfcj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rzthghex.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2omfdmyti.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pkgipgjl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hdgqbyzf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2frcfevoo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2yaucwdfx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2okfjxkir.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eysbdqqw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yfudccqy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zjeqikcw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2thqbpdio.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iqbqleca.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qkwhtfeg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cxzbeode.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zbnlnkds.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xiitjqmi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eznsbpvj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vztnkhgd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xtripatl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2nsitsbpd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kusscrew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mfncybjj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2obxjqtia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eerdcxuq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zlbvsimx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gicdjqqm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2eytwltee.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pspfcgbx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gyilliww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iwkvalae.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wndigybx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gsrcvzwk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oihvvlol.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wppfbrlx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2hdtdplct.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2egvcpbjm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zhuadril.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqeksm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2pxajlfrz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kqawkboo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2luwrzoiq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wmubilrm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2yrtqpvov.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xjyvswxz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2igbjpvqh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2deragaaj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gfobsmio.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2weezftwp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dgdduwqm.html


<!-- 参考信息 -->