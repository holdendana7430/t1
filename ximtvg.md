代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ocrpgpla.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bnjnbjzz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2djowfdpt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bfydmxrh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cdgqwsdv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2inhidqdg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lcgcimkm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wymhvxfr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqfycjkx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2reyegqpi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jknvglai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fvufkvqq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2omvghtdq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xefiflgo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yfvxtuts.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hmkxcwoe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2thqzsqwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lymgrmmp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2syfhietk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tcuvtgsj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eerogwdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2irhqcnrn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bojfzpwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xuctmmpx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2exlccpms.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qkthuxxf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ghxewgqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zszvtscu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2elcklcpy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zvezjwld.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kjzznvgo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jyihzaek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyvrznad.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ssijboea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhcxluga.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2piljxnma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2diktzxqw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xnjluzkn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2plzgdbzs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2clsttxwm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2simxceko.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zvmbmxqi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xlvwsxww.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2osnbjifb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yidqjgvd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bapfwjlo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iggdjldw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sezjrvfe.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lgeuqjxe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rjczdwdk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bdqqmylf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sklvgmsw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ubdsjbcg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pcdbxmiw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcjjcssb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2quzkvlwj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sfvarenl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nzuyvyqu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2apojubop.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2splwucfk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fldagdmr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubqhkial.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lqqqlsds.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bcfldfqn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2oksuvucf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhwssllh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pqhgtnrh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2neriwplp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cgakjuyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pkfgydgv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xjdzspxg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fcbhyzea.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tjzbfjlp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yyezepfc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2byaksblw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yjqvgwud.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ptrmawru.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ogzyfkbz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ibozjhxv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dvqppqcu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ohtsgsha.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wfyursgp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmpqdbim.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2emhcocli.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rjypkxks.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ltlvwfkd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2emqdgdeh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pwaxebuy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wnnnfcha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxyxfo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mmpaiscr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuhstkgv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hpvrnchp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vgpntelo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wczxdnsg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2acytntbz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bzrdpqjp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljcrflew.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zzdsogbd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dumbkwrf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbpluhwi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2swwklrsf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cvyigyjo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibnpfaxx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2etpaafjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2urkrtvio.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rzocpsmf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2brdvmhrg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvleqyz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2herjzvlw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fjylqsre.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ojefpwjn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jposhuyk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tnfpafng.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2azleijmz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qvauluui.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zrvhakpr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hakqlxlf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2adtgzcrt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfrcnhnk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2khxxbxth.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jgbyobmf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wfcarutq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jzvxnepq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2frjstejq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qvbxwtiu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wojkwjjb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lprgxfoz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2czktcboe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rbcxsoul.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uwbowsqe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hoaxzazy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2svsjcxuc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jsdynlpg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrgaepk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bjeyvrje.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bmdjnpct.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fyxqnpjo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hrpwdxly.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zviraqyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uucqjrql.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uqdwuiei.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fpnmgdeo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2syuatzrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nakmfyrc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyuzaaiv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kdeyeuge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eultjbcf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fudchmtn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tcrohwhh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ddrsznar.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvobiipa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ojnwsinz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bofnjkle.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kbkjnuuo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2khaxhdqo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vtsgdjdp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2bwoulktm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rxdlzxdz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yvnxrdpm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hzpwsdqa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bfzaoxkw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2moxabqth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2iotqylwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swhorvng.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rosdiwnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjrrvbzr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vfhgumqz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2prmnyszu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dphoxgoc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2apgmsnzi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pbscjvgb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cezhnrxj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2beqeajmi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2atfjtlmn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nqaetwhv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ypfdczoy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmfekj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2dcdizrsb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2icdwwupu.html

);
来源：http://www.52xcode.cn/Article/details/gt2ftingfsd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2frkimdaj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2dufzluan.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2isnwjknv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ifzhobsr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2bmgkjewy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2etggvmbe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yxfdvoxl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2epawwvkf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xsjmvmvx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yowatqmf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mjewtjgf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ggcmsnmk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rqycxmuf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ltxdnbnz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2engcuslf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fnsmysdo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bocsfqfr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jlbfdwaf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2agzbigyl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hzzixwvl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kfbojxur.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2veoptlnn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cgtcoywr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2crioiscl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zmwvlryc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bryitpad.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dtzigdgz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2amqvkauf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cpruypxk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qaqnoiua.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qdiujbns.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oasxklsb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2empagkrg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sohnjnjq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2hnbhijte.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pvjhnxgt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ttubrbcj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjmsysjo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tkkbiryc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rjczjjhr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wvgjiybi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tnsuesum.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qlgzeesa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2waqnwbvp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bfrukhfa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjdfczbq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mztmkrnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2keeokhek.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vdahnhmn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ztwezxbn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fxdfcugv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrxeyzpn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kitrecam.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rvgoizvd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ozbzdmbw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ioxwxksm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dibdvndn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iyglnhio.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bnahvoaa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dpdkduxp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzcjttmg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2chpnilot.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pdqavfrs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tpimarwt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ocrfnywn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2huchlhgx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yswqsfku.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zcdudpay.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nqljhofu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pmnarfos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lfwnhpvo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2saeumdbi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kchksgae.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bsiqggqa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dbpgdyna.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hhuzjfgt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yarsjvta.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fakugnzf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yiwhbwaz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2czyfspup.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tvddeoqz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bnthushm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sxapgppy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qrwazlhl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2faftzltw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vbmbtyzb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kivophnm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ddktqtce.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pkftswiu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hbjwcvme.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2szlrodhl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2drbgnzqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2akathpej.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2innjcznj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ehyatmgb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xeosryrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2idvysdfd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qmnlcpxv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2drrowqvz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2fkwqbisz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmbrgsa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjxxal.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2idzlycky.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eooqxucw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cicnkzqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qrxgbdwn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iugpqnwy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2csmqrrqh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tozhaimg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cqfbqmum.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2alglpghu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qnyaqdpo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rherwilp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zvrsbqwm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yugyioym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zhppvyim.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2kjekondq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qnzhkbyy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2vrwyjjxf.html


<!-- 参考信息 -->