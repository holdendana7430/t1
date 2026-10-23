代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lycnymcw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pdgkfuhy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3khqvoesg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pdhahavt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3osobleev.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gasdxpxf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3meobcwlq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwpdddz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3irdxtohk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjtljqn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jhfmjfrf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mhionbnd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hhtmohcl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gpxmimfi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jvpqiysj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3txhkvuff.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3obrkbxwg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bbfafnkf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gyraqvbg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zbiwjkgx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kakwnjmx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qjjldpcd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mbchkrhb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xdggrdyc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3icbhytaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bwzaojmo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ptgkdbrw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iaoqifzp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gqbqtelc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvsbrrg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xpbebyvy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uiqdhupy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvnwnxvn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3eyycwaqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghjjkwya.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kwsbiafj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ismnzmly.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jpgvfjga.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cgfdkovj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vtlwdsro.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pnhsxvbh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xdkhydbq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ythfcczd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ctsonivp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jnzvlkux.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jnlmpphv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kzmsgjnb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qkmdwdbr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mmqfamzz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fweicnke.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wvirlkrn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mjnypjnx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dwkcpoar.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xvwwyqyg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfzrbvne.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nfbkdnto.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jjlbhyzt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nkjrjgeo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrlnhddh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dcjvtijq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bsbqbvmy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjmhao.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gkgzdwvj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xmbkrfhh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dhlframn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gykcnkxu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kglidgnt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3etgejkez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3amqefrej.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3empapchn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dgkbqzjk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ayqopvoq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxqmtvt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tsxnpwzr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvbqphw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdbuuytd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcrdets.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zfisiiad.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lyqthgqx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3twgcbgfl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hfsjhdid.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3igvyfghp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xfdytopp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bpieyolg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bkufiztw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bbbufpew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iofxqxvy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jkflcwep.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pyhuhdht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neldylbk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqhnddxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyidgwek.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mcxntbcs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hohozobw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fecsugcj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kinirone.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fpifhwzf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yqurrxlw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ljpgnjdl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3woezjzat.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3etfnadmr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3igmwzbvq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mxoivbqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqddjoua.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pwfwiqvc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvdupb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ouqzqqqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3akkmylid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cimvaqia.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vqywldvo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hfncuali.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lvbrwkrg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kbsnrmta.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xonzptlc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3djlcwjcz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3pkvcatjt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fjwvdwbe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jqltelzc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlcebc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3daekadmw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3odnrlllk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3drorjbrr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vdpnihmv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kfktnabz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ymfbxqzl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uliwqjqp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fqbatbor.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wjvebeyh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bhuukhmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hafvgmdx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qnqijylj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3docqtzbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3djibubmv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3aslrxeci.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cwyqusea.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3prdripuz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3uplroeop.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pvvbfper.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oogwdiup.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcjqxnjd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vrotshic.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqbopffn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vooddkpk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqvtwlrj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gyktfakc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwwzyfcx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3uonyjpgw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xxtwtgww.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3dglajudf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vsvjhdno.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3csqtbraz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lcttyxuo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dwxjlowf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zvrhehlx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vlmrklwq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3eyzmdgbq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jlfsvksy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eikoihgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rmqxhlbw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rngjiist.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3weendmbz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3amegycur.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzbrfuvi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zxftgsvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zagziivp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cigwnfyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkdtiifn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gjrmsmga.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vlfhzxat.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pibuimfj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aiuvceis.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3hmwftbwp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ccixbzio.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mwjhxidq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3okfybnfw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vqairrdg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3joaphxfw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lsmtxaci.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gwmgqmtq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cdtqitml.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aoozizoj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ifatzaos.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lzijmwam.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wcazmfya.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jbxeszjo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yradqtcj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nnhjwkyg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mqtcuppe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dgaeevdh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tcunjkqa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lwfybpay.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ullicqjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3osozingy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zifaxuvc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uhxnymis.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qmpeycpe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgufavyu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fohcamjz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fvihizwo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3azemqbkx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xgigrqrj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uvmuzmmj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uixrtuts.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tjngfkks.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3thbqmvsb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3coyugibs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rcfqvubw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ckthtiky.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ambzrwup.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kksuuigc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amhctztr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cuavzmjp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zrvoahvm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ugkjbcld.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3brbgzspj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jjmdmxih.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qiqlcwqw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gvokqzjg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lycwbwcr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3aejynsow.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3simdkyie.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rvlyjodt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bisbxfys.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mzzytjmf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3whghqbhq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xwfxusxy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inkfxsoh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hmmhrldq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hyumfbwm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tirguapk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdbvsaix.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qjuhajuv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhqsqbru.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bavbelag.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbngikre.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gpdonxla.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jupuocvi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3klieqtyt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vlcgzeij.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lyiythcv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mtnybixy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dsgxlfbs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kafgvaqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3awmqkpqk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sfxdmbte.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ggwhmciu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hdetkzjb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zhmhwznf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vrpgekzf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3goyepjay.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rblnqvjf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oovjtqsm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hwyqoxgl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fslzrpil.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xwbavylr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3hozaxnur.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3agghhzin.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cktffxsu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qjbupvhc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3tbnzscaq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zictssnb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kwxiohjq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bmadbbyk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kbmqgaqn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rjahpoix.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vzbheaio.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3udtvixwo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yxofwhuo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hhilmpti.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3eryjfilq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wxelafhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vtmcqkvq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gvdzgvco.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tplsfokt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sdiucjvm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zqjmohfd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kijptzlm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bhnicfww.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gnigcjiq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qsyowiri.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3quttfrln.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtpitwl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3okkwtsdl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mprwqdzk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bahjultl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3akfgdcke.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zeumvtnu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mitehxob.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cdenmtfe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xmqtriog.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hfpokgjw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3clifaraa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qjqgeypl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mmuvnjug.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kzzrdkbe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fttuykaa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nvqkcqpc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lrhqnoye.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3okliacqp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rfhfilkd.html


<!-- 参考信息 -->