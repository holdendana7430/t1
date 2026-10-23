代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3flhliagx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cgzoalbj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gabqwjwh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tktpxstw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3supxcyae.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzbcylvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mamrgolz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eiggbxcy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xrgqpfnw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vxngopsh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xihtcbsm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bycwzznl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pbiivalg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rtomsrmi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3llpivjse.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fsasgrpf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zbhuhwdp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ukgmbgna.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ltfeqwlv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uodacazx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qdcucpgc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3unbchtmp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vmxmewfu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3irkuueyc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3atzeehgp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ggrwdctm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3guqsknxr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nnxmqdvk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pdqemqea.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3aalycyrk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sqodecxq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3akctaavf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ykwgtluo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ehhjmmxj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xozpyufz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrovpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfxzktip.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3lkgocctv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzacxjpe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lzyxjyna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wbbezecj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3eljcyzwb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gbqxhulc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ywgbxlai.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ffsittag.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3buhcknwu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gspxevev.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lvozhwsl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qknicbpv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwxllu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rdytrqqz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gaahyepq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yxxlibjf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ynojnyxe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yrtoinhm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ptifsrpw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3oytwcdjz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tlfmjwgk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qfhjproa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rvewsqce.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3sbkjaczv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ezmibxbt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mzbmequh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ybnwstpy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jjcoydpm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fxnrhuvq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ykkzcdpk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3icarjnsn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dgsipofj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3toyiowyl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bvfupccv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dbogxhoo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mwkwythm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nqdwqtmh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ojghowxf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wgcauequ.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gihddbis.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zllxdokg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3duxtxmnp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mwljpcig.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ilvcgzhv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xeltiscg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rfjloidt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zngihdgm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uurpzpkz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hcwapsyc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ukhpzdbr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ngttwctn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lvdwcesq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3muedemyc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3upxcxivd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3lrnaehpt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gpchzpmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fayxzfdz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3etedorjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clsahdcg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3asuwcojh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3txqmokxa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vdnpqmie.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3joqawgim.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ctbueihn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tppqqihc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pakceppj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kssacxdn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdfgthty.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xtzgxwlp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mfwfupdp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lyxigpwa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xpggoykq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhwqnqm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zehkhyza.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ljguxhwa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfthcjw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ipiwttkc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3sgyahiab.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xirztadv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gereudnw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cwaogfmv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wcutiudk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3pvfkfenq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3fgoxkkhd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3jgjyfrkz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3klcwkkvu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kvswplsm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jhyywwxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pmwzigye.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cnjdfcva.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ssoguekr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kdkzgbve.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xsdjhnzq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jiblgjru.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3idnhhdgu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dmjqcaii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ajpmstlv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fqmvgcka.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jqveodft.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwsfjwtw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nlbvqpqz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zsjbmhvi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ssbogtnd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3loyymxzn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cjwkhifv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fgbramak.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otyirfql.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3hpemdsta.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jfwyclij.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fdjgzyuw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxjsaiqc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3myipvvea.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggllxskd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qrwwqenp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fcqdotyz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hujnggbe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qbxjxlro.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lntozbde.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtszmoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lxgprkgp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kaidjewi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vloiterj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3shtqpprt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oxfcejxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eemrcwxm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vjkrmaul.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zamzctpw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3textgvbk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mxrmvood.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bxleuyyg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qdkgmtzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhvexasr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hnackahb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvherrkg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wejktwvr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ttwhdanr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lpqohdko.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3orhmwloc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jcrikdir.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3btbivdgd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3acakmtbo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kdwowlom.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fhhtkryn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3myktucen.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bxnrkaxh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rnmpraap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xrlvooci.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xmoyspyw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ipztinrq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kbyykeae.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wftheeen.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tvmqvjtj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vpcmsukr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bqzqnufy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3phegdqen.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3oeyscoib.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jayhnhdy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hzejhmdi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pmihzara.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3siwebduo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3yzlxguwc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nxrrnnph.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gcebvwsf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nffkfvkt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3remonshu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lcagzjaf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jhxtffej.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vxasklgy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pcbvzzhy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3enfsrmqj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ksihvosj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fggsyunb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3fvzmwusz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3fkcqopum.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ljygqvqj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfaqwfep.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3puetyvms.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rveimdnb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vebgxdvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfhlmf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hivuhwph.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ttnyqyyy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sohvbyyv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qipjfjxb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tktkicgs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vieposwh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qazojpmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nhsjycxv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kczjnqqm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wjknfhlt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3sjtdaufl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lcywurkq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hlkwjkby.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxddhjik.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fhojwrzw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wguglzju.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ilfzloll.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iajzxgen.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cxpqkhzp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufndacwt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cwmwkvth.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ybtmhmmp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3avtjuvdr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drmjlruk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fmctdofd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lzxpdcly.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3osfdzgyq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mqwdambf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlssfzvg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nhwsyyjk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hoyejckr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uvacmrgq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uvoignty.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3uekuofqf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3urohjuxt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3zelqftek.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rybbuavc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecaawnxu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qicipxyp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rlqvyenf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pkxdrkro.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3stxrrigv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vpcaofxy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3oymikrhi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sgdmjxik.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tcjblsxn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mjasjdtf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dmzdcmsh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jvguevgj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ohkzolkd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3blohqche.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mvlijyhp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3twjfpwlv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cohclagq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qhdupcps.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kpldxzpb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rsntuyoy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nacyjpvz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxsejoi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rdmguilw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dmkggjch.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ufyocbnq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3umkkdsio.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nfzyahyt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3osanngta.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmrzfjxy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nbcpqoex.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nfjmqdxb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3bggonogw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zrwyfnfl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ennnhiol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lczitjbv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fudhqhtk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3poujpahg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ompwwowe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ccxrkpzj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mqnwurqr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vfbfpcdq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ebglrxpr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sytluqii.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gfirgykw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3twlvjruv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vynqyhnu.html


<!-- 参考信息 -->