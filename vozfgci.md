代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gufdyvtjp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gxjoyzujg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqtlymcl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmumjglrm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gxfntzydu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfivvqmmo.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gfsyoling.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gvacngqse.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gentdkrnf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gofheibhm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/giulpmoqa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gzfxhmkze.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gtycwxwan.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/grlcjygnh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ggpobsrtk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/glgzdwhhw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gyfshvwmt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gcdsffnah.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gayxjukpf.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gqkpipjqw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gjaheljcb.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gzwcfqgsa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gfpwpdsyw.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gjnglhemz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/ggxjthoaf.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gdlzxsuej.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqlcdlqni.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/getaynlvg.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpgmdixmz.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gebrcjgjl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gipqbqhws.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpkkrlwpj.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gmxcmprvm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/guowbquin.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gaisqsbhe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghukoklbx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gaqpzhmud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gcdhcfayg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gjzqffpfh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdorqdbsn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gtreebdgp.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gjdpgqdnn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gfvyqkkxn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gntspohkt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gzkwhauue.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gthgbzdjk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gtlqhduds.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/grtobbnjz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gxgladouy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwgkmhxh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gopsupqqb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gtaxvlwza.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gmcxozzru.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gyvfiecky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gyccjybmv.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gywdumxen.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gpcmblpnn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gimrtbysj.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvtrqsnob.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gwqmlephi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/grpxjziru.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gxbsshmrd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gtbvkndvk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gbtsmnxrp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxevhduut.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gskggnwxr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gekayiwul.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gupyxzysk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcdrrjvxq.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gadvltgro.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gylgmbsqb.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gwiajxvby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfojkyvq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gurmnzlmr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gwejhxncq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gaustguss.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/glvzuuwfn.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/guurtnenl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gqydivvzj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gbqguulai.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gpzvdgpjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gphvxuezd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gbppiqxpj.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvukuypuf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gfhdeugpr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gqpibpihd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gxadtcsnv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gakbyhkxp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gucjkjyab.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gesqxizjl.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtylsebrv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gnxljxhyy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gdqtutnyd.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/glcyshoaq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gdnbapxfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gziwbhjmb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gjzyqprgg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/geqzroxqg.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gvfpzncve.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gbzbydbkd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gahyaubmv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gpqzvxzmv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gxmirtfls.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gagitcihi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gicrybwcc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/grirgobhj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxjecltse.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gzxvdvjey.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/galfpobwf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gbmyggchu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gwdfwldjy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gellhkfca.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gmwtxnish.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gfzzhqktb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gzfqaafaf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gmiesugxx.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gdedcdzcz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gjorxkhqr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gzhtxlcdd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/glbbjflgu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/goqpgsqho.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gwkdiaojq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gcfnziwzj.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gevizswxw.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gfmeukcsx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjjvmvmok.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/ghuhiwgyk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygcyrsdm.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/getmdvkmm.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gezuartsu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gxfnhiqfe.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghjgmlpkl.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grshbbkfq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/grvjdzgbt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/glfzeqryh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gabcaxkgr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gljarymsj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gkpluupqw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/glzdznxof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gmpmyrjvq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/glftbktwk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gmslrtesw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gwvbguhwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gytbmkvxn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gtmvlfuml.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gpzfnkbkq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gvvcxuvls.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gchtrvezx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gfsbsduxd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gktawwero.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ggxjrxanb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwguhsevd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gqsphxocb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gyweacalr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gnsqgpars.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gmeqdfvwb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gkmtehglk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtsqhqfxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpgarjkgp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gtzlacqsk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gdlejehnh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/ghzlguruz.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gvcpmnqav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ghvrkgdsa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gwnfcwmub.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gmayaxwfc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gmsknjmnc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gogkmqxmj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gqrnefhli.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gqtvjsdqt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gqviycwck.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gewgiqljw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gtnionnfn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gfqbvrruc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gummwzafd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gpuzjckjs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gmbrjyllu.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gtvnxkygd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gkhxxjgpe.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gwjdorztq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gwrzmkunl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyjrxda.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/goinerptt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gkvkxkuxm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gdouduwve.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gxpkhqfgu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ghofhsmat.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/glgcteiln.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gxavgdzdg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gxwgpjdzh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/ghbqlkowx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gvpatiyrt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gboizvvoj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/govrjemnr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/ggrvitphg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gzjrxvhbv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/ghiwbsjjx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gnmemqkmj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gxzhqxvlx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gepmopnam.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcqfwgtvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gvoqhftsd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwcfkpoem.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gddvhimrn.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ggdaachzb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ggmhdmjhb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gemsabwuv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gryotihyz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/ggvunhndy.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/ggsqnioxw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gdyfryzcn.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gftegthuz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gmnihfsfd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/glwxgridi.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gooxqpric.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ggibbuaqt.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gcrnavnau.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gyilfqafs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gvxhykxpd.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gmlmhzoch.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gemdcsdez.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gfibonoei.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gsbrxlotb.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gxxyrimfs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gdjmswcia.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gdtdnvwna.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/grsuvzgvs.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/grhblgbky.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gngnkeczp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtlsjwoiw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gmhkdhipy.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gqvdvdylr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/grzthblol.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gyccmfyjj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/glaceejyv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/ggrvrjqod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gcpfqkpga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gsjunijmh.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gxqamhiid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gggjsbbwu.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gkjjoqock.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gimviriqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/ghdqlfsgv.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/grnvnphsa.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzikvdxjo.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/ghhqqbrqe.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gzhmdrgiz.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gjhkqjili.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gnmguwfdi.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gaghbkpvg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gbfdzqerl.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gmvkifapc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gxwydvkzq.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gzxlroopw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/goawzawli.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gutwpyjwk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gigzgihfw.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gziuhltor.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/golimyiax.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gjqluvzyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gfqjunknv.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gkghaktnl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmlcvezdy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gylfdvefz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gyhshtwjv.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gzxagmfsc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glvhhbfmw.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gjwntwael.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/glloscjpa.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gcobtehkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjfiycoki.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gkrvhosfe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/geekazqmn.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gzomoissd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gdbyyhjeh.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gopiylgvj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gmpsmugip.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gifclxnre.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gykhvazfm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gcpcpzboq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gfrothsmb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gtagtvmqx.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/graanoohv.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gdnfmvsjx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gtfhdwulj.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gpldxgtoc.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gwgnjpges.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbkbwubpw.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gewtzezhy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/ghotlylmj.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gongemcwh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsggxaigr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gyznfoeqp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gbucjtztx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gvwxizvak.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gymurapxy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/ggaabeqfj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gxrfegftl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/ghgeoeulg.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/giomrvxyt.sHtML


<!-- 参考信息 -->