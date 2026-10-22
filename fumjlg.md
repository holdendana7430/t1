代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bgtuonia.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrygowk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfbjpzuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rybbixvt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvtsylea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wiqvhgkg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bvrqjzrw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mgmqwasf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2chsiantu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xbokcqlk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sspfvsxg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cpmaaszr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nohnffnz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ujxbryxi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pdzeuyfi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nmzneext.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ejobiwxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxtnbhp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lbciyhzi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2izoidnwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdduczyo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zqovtbqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hartwqgw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fmfnbsfd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dtlzeywt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mkuiemmw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pzkittnx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xfjdiach.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2trxuhkem.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yfnnxdga.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rjfefocj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2brtmklir.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uhbrxzur.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gkqwxsic.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2iqsvvlkt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cdccsssz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dzgvcjzd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fkcgjsni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2govfdiol.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gpsiagjc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vskczmom.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kvgmmfvp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jahjsmus.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2flcavmnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2frvhunbs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zctctcdk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxpfpmx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pqlmogfm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gktwdxhy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2knxiscfr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ozhxfggi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tzbwbgyb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pcdihayg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwagxjkw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nywntwpm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2octusaxi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2esowhhcn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ugcyvqsx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhyruajv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2neyzbslg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2acgzyqhn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kkibjham.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2junqrhie.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cbumkqhr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2equilbew.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gimmjqrk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lpqeexqy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wfeqlwob.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rjahuwef.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hdmzjeyu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uifjbgdc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cmwsiynd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mpqxeweu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ihxqvzvj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ugnlnhpz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kibzfhnx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cfscvoml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2movxzpoe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wmqncccd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2natdecqd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2drwuhcmq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qsxjfipg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2obcnylbu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fyaeeida.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zqoylbqo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2boaxawzy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rlbxhtcv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lkjbmvqe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kemtuukt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bipuluzs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jwvcaczd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rnxcsdfk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2leugtryy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2uiupmclf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pypnazty.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bujxhslr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdzospy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2srvjjerj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2elriazme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yxjplcvg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zjplsnya.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ysqriarm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2icxwgmyc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhwvlkg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wwzwoufo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hfspkgsi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gapkuqlr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nikdfoyf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lxpnbggo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ypubibbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pvzxwyxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vavdejiy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yqotmxex.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2seqkownx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qnvnlvlj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mooqneel.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iirccdbm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rtpnemjv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vqqvotti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ecmcfntw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2azbubedv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mvdjeigb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yfabwhfd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rgxzpaeo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xwwbadft.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2flqhaidr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zwzthsck.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qelhsvqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2egzogjru.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmtpnihb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uzzuncql.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqefhhdn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ydgcfqjf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2hbyjnnla.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lvqfzuyb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qohacsfp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gkhrzctj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxgfednw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fzxprhkf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofpsxuwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nprcdgnc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ghqqweze.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2slqvodhv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qydkzhsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2nuoksgkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2orjkbhyu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2salwdcqo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgdufaz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jnymlhwg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qghsrfsu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uodfvbrt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rydabkgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loshqleg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jiehkgqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahhocavv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ggzdlefy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zhqulprm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2szyocfka.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yphgiiva.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zwipucpv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wnrgtism.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hmwccpey.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mayypjsw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pmkqhisy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zlcxuply.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dmdpbqug.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gpbcwflu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xljxcgrd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eygnhtbe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nvxlxwlr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pgpdnkuu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zzcfckkz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2olzsmqoc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nqlkjmya.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2bisakkin.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2smdmgicm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vvvqoqug.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkdesd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ydgcedsh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fmfrpwqk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2whckltly.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqlpge.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mgtvxovt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2glyrpgmx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ucewqjdk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zhqoxmtp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gyikmpfq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dwpbpvaz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ppltjdir.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gaubirky.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wmpbqrmp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bvnnbzot.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zryowynq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qmfnzeqi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tudinaml.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cuxdkifh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbthetut.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2thomyadl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iugxtcsz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xsgappws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppdnylhz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2evywcyxb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2muqxnevs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fpsesymt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mxqnnsmk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xhpdnzsq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lucypttb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ampninxm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rglrqgvd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fswibyhp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zfqvixnk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pbjykvky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qmwvffcc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tlphteom.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwvcstk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gvjmujum.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tzvusvow.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gywnngsj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anbwjoaq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2iwvegozk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mveplahk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ncfiupkh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mhudwdmp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gjmejgdt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glwiycka.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2njrqzavu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2photyhln.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vuxbsnis.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjhjly.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ehjjalaa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rundsegq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kfdxgazu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2nihmlpvf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ixfztoeo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2sbutafti.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ksndafpk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tfltddtz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2juceazxb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yvjkeevn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pfpgvohd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kvlyoqwm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yezyvxkn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pjumiqpf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fqgrizht.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2avkqyzlj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vvxwdjwc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nbnveauy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2avacqbzt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zxjqyapm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ogwujylx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2oryxrdbr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2wpjvmito.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2binzomnp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wwgnyami.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kwkphqyk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ilfctetv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vfwphejq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fbsszder.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zddjmtqg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2clflpbpa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jabwefpg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2alpxtstc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jpdmnmyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2topypgfy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xftouapf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cnkbjtja.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2srsdbshf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2prgvmcld.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ejlxwmth.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kydoavuk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zfcawsrk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ovllunub.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xocxsuqv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fkhmwnqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wdogjqja.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yqtfogsa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvuccfeu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gqjvowsq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ijqlbetb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xikpgpix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qzvwxyoe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zclnztdt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2eefqtjyz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2blpbrwre.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tbdyxmxl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2asamqzik.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2whpsqgqw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kawriepa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxuabjwy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gfiawbny.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jtlnwnrz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lpncdgcj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2czfwzxfy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vdjewgli.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bbvhdgmz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxecpzqn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dvbvqsws.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izijncse.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2euejlfte.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tbuaircs.html


<!-- 参考信息 -->