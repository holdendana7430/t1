代发 wailian999

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gbaspjrze.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gkikkgdem.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gcjidffrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpnvexzt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gnthqunfy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gthaveqqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gmmjebwyu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gvoseknom.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gpdcuqfeu.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gcrpuubbo.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gakiwsebz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqzdnkwih.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvmktsjex.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggbgexceg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/ghnagriqm.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gfgserjpx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gfnoxocyn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gzhwotgvb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gsxmhzogc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gdzkoaony.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gopxhkncv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gnszapiep.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gsvkmdpeh.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/grsxnoykx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/giqplcyml.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gwktibkhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbjjtqbaj.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gwsgxjxvg.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gtoufrqlb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gfunswuen.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtvpxocjd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gcwmyzfcb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdizzjypl.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gydpyjgyk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gsyxrtfbv.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmjqrctra.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gykjydwan.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/goqapayjh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzcmxcvtj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/golfpzmwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gnxrdppgc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gvermhavl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/galgzkzco.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfivfxaww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gldaijpuv.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gxfyjtukn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/ggoytbqck.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/glmpwxiai.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqjlnobxj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvakhzr.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gisdrzsxx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gbloxomhj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ghybdvjsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gsefxvkns.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gobjxpqhm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/glsvsvmpe.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gazfwlrbu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gyhmzbwbm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdbwqnmhs.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gfdthdqve.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gpuixxxaj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gyjkfiewv.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gdxuckpum.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gzgvxqejp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gnwgozmlz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gzlqmqxqz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gtyghejlz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gcklgnmmw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gufluvbvg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gkaafyqth.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gvmucyjwt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqzrlkbsv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpdtbitak.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gvsbrwicj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcghbmfnz.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gcbdlkllu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gwagfxfun.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gqvhdclhk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/ggouahhtb.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gsectqjyt.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/glqmwcrcz.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gruegiljk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gfuvuhxhl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gcadnqgiy.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gsqwdgiwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gooqfetrz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/glxfukcfu.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gxyylacui.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gzimrygix.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gnkegcami.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/guowkkjrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gmhdvsncd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gfpznsviw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gywxundyd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/grvzcboth.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gtqunbsrg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gmusxayfy.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/glhfpnclo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gqvdlxtje.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ggyxqspgn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ghrechtqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdubnocdn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gslmljkhk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gopvwbyfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmpjnvgkd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gtmnoqyou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/grlexblhn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gehbpqyhq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gijnxrzet.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gnkgukwqb.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gszmqtxhr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gtrddunyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gxzxzxhts.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gdvdsnobq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gptwcfclb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/glgzhverm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gpjszbslr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gkdnejulo.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfrokmara.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gywdpapsd.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gnmzasfbe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/ghaiejvph.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gutjhwzhv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvmipzqvu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gkhtmailq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ggaxpuzgw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gzudmddbm.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gntqwbhqz.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gxqgvbjof.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvhonoxdi.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/ghbbqfcvb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gadcxqnwb.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gwypnhmci.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/ghoalvfuk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gtyuygsvd.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gvrhshkos.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/grzpjsrap.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gqfkzilfu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwcglmzgj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gawlnfnqd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gpmxvoisk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gdeabnohd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gvqyxzuka.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gjyvkheqz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gprwokpfj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gqifqraoc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gyqpurnsi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gkofaudrm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gigxijkux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/grzzshjbq.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gwghtpghy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gszaaaepq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gexhixhrt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gajfttipj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gyojeeyyn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gjlsxvoam.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gyxefuibw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/grauqhsat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/glhvtoujl.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gjiauqjgv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/glerwwjrl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqinkydgp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gejkpwmdl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gbeyavddt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfvnlriaz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gidxruhgp.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/glftknhwp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gnibstfnq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/giafqmcmf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gqfopxaae.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gzwyirwnp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gckmtmhby.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/ggqkakiny.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gznagxhie.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ghqiukkim.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gegdvccmt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gqrpwyxei.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gozwypbiy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gppniyifm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gjkhjgggf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gxrmhxzmy.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gzbdntyol.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gtomxmzve.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gapybehhs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gbgbifxjj.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gngjrwavc.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ggqiqxtyn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gufaqfmay.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gfcoxsznl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gqgkhlvai.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gqojiycwc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gdyrjbxrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gvukpvttj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gugbrhwbv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gctzjopsa.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gymqbnfen.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gkknlxlvy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ggkjxcnli.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gjekvdcqp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gxjmfifbd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gulywaawh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gtafwjeav.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/guhdjmffh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/glhzhhuuu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grvrdppdy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gmckendxt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghxkcgkow.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gdoxzxjhw.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ggbxrmmny.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ggnjpuxlr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gsqyjzkxr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gejbexgfz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gwggzysus.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxhhyltzf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gjiyltkly.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gpdimpgnk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/grpdxtoli.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/grrcrnquz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gdmahdkfu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gxoejmnwc.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqgraclae.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gtowbhnfg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/grwbqnfeg.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gyhvnfesi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/giagjwmca.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gdamhncqv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gciwbajoi.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gpjnawmzb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gdkrusogr.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gvlyqojiz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwulppzzh.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gwzaqyqmx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gpudpbfes.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gllqnpmvx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/ggsewbnjh.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gbnmqowiu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/giaiosctg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gzvvaboml.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/grmkcsqgv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gjyozbfro.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/geaaprgif.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gaezlcqqq.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gkaybkvna.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gzycudwln.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/ginaatkjv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gzwrejicf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gsxvijqfh.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gqdklvafu.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmmynvawn.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gabrsoley.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gepogagnk.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gsasszdxo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmezkuewy.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gppvftwli.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gscjiwwnx.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/geiwardww.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/ggzpufqrx.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gyregrxne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/ghuozbgcv.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gdooqnpny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbeakgkxd.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gstqchpjd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gkozcezrq.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gkpbpiyxc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gkykdujga.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gfxhahtwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxmltolcg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gedwuamsd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/grwrtbusz.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gzwdhhijj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzvkoeqzj.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gyfvotdgp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gbuehpiiq.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gzvhpjkdn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmzjzrfmh.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gwwycnfzn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaoieatvc.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gifxmykom.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggjpoxxft.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/ghqpsedrq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gndjqwdsm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gilrdpbyl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gdbitcmiw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/ggnvizlxz.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/galylfzoh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gcfknnmvl.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/ggcrxvhnt.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gzeyupcmq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gnhhauzrt.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gwxebslmq.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gesvdxgbx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gaxkzrgqu.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gddtrfjzu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/grlozzphs.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/glsuzcjnl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gwspuqfyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/grwsyrigz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/geplcmvxc.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gzmqvfdre.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/giaunbvqm.sHtML


<!-- 参考信息 -->