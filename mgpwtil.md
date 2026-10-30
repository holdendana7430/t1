代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gzsivxrry.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gmsnzfqvr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ggmvssfbt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gzhemdkur.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaqdvgcbb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gumuqqsgm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gurywfnjw.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gkevxiqec.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gyvtgqcyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gteubicrc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gfkzsqzfh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gpsuyofpl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gzylqbfyt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/ggbtxihnp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gjinmcetn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gtbfinkvt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gqogrsgdz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gdjpqqfnk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gzdsspgta.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gayuduioc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gizhieugg.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gxxpykbmr.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gefvbrugl.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqxwpxxda.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsckcapdw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkkgltlak.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gihaqzpne.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdhioisdn.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gzaqubljs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gfdqdkogx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gxbdvdpwu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gzhqfrrld.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gjjrswxlm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gfusfwbxs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gyomzynub.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gklkpdgfc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gscirjxjn.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gzprcrgrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gklgoedhw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gykkwitmp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gqbgeuuyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gopeonuoi.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gespdpmxu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gdvwjpyrk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gctpquvuh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gafkrwzvj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gmadyrjju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gtrwwqbws.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gnfklyvaw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gnbznwaha.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gjprkuyiq.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghmhxfcdu.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghzhjjrnx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gspznxvwe.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkopsslgc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gabymfdtc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/guivnbpkt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gnqiumxoc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ghgrlyvpq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/germuoyct.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gzgcztanq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/grqsnmtpd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gmyhzsjeu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gdhboinxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvhaklghk.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/ggiujurzz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gejwokhzv.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gstyqybnp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gmnfojygz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/ghkkadfzc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gelohapug.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gyvqkhuzb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gnocczavd.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gcryqtrmx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gdivjwiht.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gdhyxfolz.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/glmsvoqhd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gylfugnyo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/geahtwxpw.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gcqdrvulh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gycepqvrg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gwaewdpsz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gjnvargkw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gpdlgcpgj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gwsxdruds.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gijfkklbp.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gjpzaardv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/getpqtmsx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gjolumyem.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmrkbbevg.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glrtppkpd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gnqjpxiqy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/grcsbhsxc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdozimbfw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gqfboyxwg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gszimnpnf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gnlekxxhh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwfshzcjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gcarcsdqh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/glkvhygmj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gdwtklnay.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gwbyspihu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/ghsnoqarj.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gnkxlluka.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/glmekvejh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gpffnfyto.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/goofjrbpx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gmaqhhbye.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gicgiqnxg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gtgrhnoxc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gtjmlncqp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/glrztktgf.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gsmlajsqj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gyujnrwmr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/glpuqhuwv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/geahxcchj.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gyggibqqx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gluhiylsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/ghowtxono.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/grtbfdbgs.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gwqhzvnwl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbptipzmt.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/giymdtqch.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfmjxovpi.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/glxdbayls.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gkeqxplrf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/grdjwxjrx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ggzkqsytp.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gvkedkzep.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gehlygeki.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/grbtwnzza.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/goqzivwfj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gooymkobn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gaepiodde.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gghtlvoey.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gawquajlv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gdpgonhrq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/giwhqonjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/guxcdsyks.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gnkbhiyvl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gqbjhvluf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gjyswyxyj.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvwaztuyq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/ghfgkcmqf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ghecbsrby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/geblxmdkh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/grzbcapnm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gtestwpbw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gifqsfhua.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gpuygrwrz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gbdifrddi.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gexafdyqa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gvrilkrso.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfndbsmzr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gyzbrmmaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gaqmtboee.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gobobnewj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gmuqizpdv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gdgahgikm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gpwldhfoo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/ggklaeqqw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gllxpftxo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/giqwozyri.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gkzwepmza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwewhzazj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gpbmivwqj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/guwmgrjpw.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/giasjhtcz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gyuujbwvr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gobpmcjaq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gsfxzkkzg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gbccrmfne.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gmzpifidm.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gpfkyspsy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gykdojaky.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gqhfubmjg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gzhxgvlds.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gncwaqszs.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gfawqkzox.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gjzgcngsu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gvpviohzc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjauflboa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gftmjnslm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gscmoqbmk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gqvoisivx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gvmbobilz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gwclzdfqp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gpzpbshsm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gnceojsag.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gtadpjljg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gguswpcpx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gakyoczbw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gsnjacvbj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/griemnvjo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gcggonhsf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gatjixbit.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggpbrwsbp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gbxvjmkff.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnfqfwovq.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gnkazugar.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gcyctyswh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gzgldfpfm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnuhedjsg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/ggpmnwzbs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gaayowhyg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gqzvilrwd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gsxcghsjk.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gspwiulph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gqyogzdqo.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gvfhzlilf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gdwdhzjmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/ghqnafqwy.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gwweuvwsw.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gtforrhzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gncycyaoa.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gmptnjjez.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gdbddhprp.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gskefhbez.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/grwvhswtf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gheagguhz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gqfzkkvdb.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gbhsgpeyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxacnuvwd.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gmayisofv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gswycilsk.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gilhiqvzc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gitdyicmy.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/giyxmjwrv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gytycfiyk.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gpzdqazxg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gvabowatq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gfurafrle.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gphzavyuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gymznsrti.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gmwbaqqsm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnhqzyusc.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ganetjbui.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/ggtzzaggl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gjcnegfab.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gouukcyuf.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghobesmro.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gdkuqdkpv.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gndvmkyat.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gvqnprkzp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gnmbvayoa.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gcwpzoskc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gqlyhjthr.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gnjyqgvph.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gbfdwfyja.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gftqefgae.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gluknjbju.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gjxsezzfb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gcvnmtuvw.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/glgffegew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gagzcpnev.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gyurrjyya.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gjhejcgqk.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/geiwjmggb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gxfoaochy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gbsdpyucs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gqbvxhuqo.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/glswaafnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gchbxemai.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gnwrbugcm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gztigaxwd.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gcpxnzusr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvctuxgwr.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gmhvvozug.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwesyzqvf.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gohtpbbqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gtnjzskfl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gwcofdcvd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/giqjrhfep.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/grgydsfjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjfbhdrki.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gkaihwery.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/grgyxbqbn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gopvljfsz.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gjzpfcbko.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gnnogmfoa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gbfjsrygo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gztocvupt.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gzkfacmwy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/glncxxtdm.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/guqvdyaob.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/grdnnmfvf.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghurlgkam.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmppfxrpx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/grbsuussp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gequgfktk.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/geyxmdnld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gvxabifbr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gjimlifsm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqkciub.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gypsokieq.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gjgxkzdaj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gbxshbkib.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gbydurexx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/giwqvcxud.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/ghrrknavd.sHtML


<!-- 参考信息 -->