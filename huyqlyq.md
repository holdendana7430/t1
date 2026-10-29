代发 wailian999

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/ghhulqojs.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwsbzpepw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gkkkztkmm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxevxsfdm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/grablxzfu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/giqlxxiqs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gmfwhdxoz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/grhtoqvhj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gutduhmqu.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gwuygicuc.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/grjzrdygf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gbcjbkatp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtvhwarcx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnyqgzyxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/giwyoyiep.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gzkrpkosh.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gqnhuydim.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gpuvtvibr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/giiobwjlo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghulsmajx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gmypbtptg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gdhswursd.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gsmuxnpgq.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gpvkattki.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gvvaknget.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/guuzsrsxj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gecilcfnk.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gzblvxgya.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjarnldkn.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/grpofpxoi.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/goqxbrerm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggzobkcmb.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gyzcsuyqa.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gecrlfpel.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gqtmxsrpa.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggiarasys.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gxviooylp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/ggsehumgs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gimnzngmw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/guuvvponq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gxastjdcy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gcouzyhwl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gbkdwjiwa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfrhzxben.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gsqlqxxkm.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/giyimlaiq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/getyokpow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/ggtflfprn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gocqxabqd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gvqbeerac.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/giumvebtj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gpfoeezzr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gdgatnthq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/ggrovgjvw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gmskbrhac.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gpmplqrhl.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gwlbmcxin.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ggzbucljr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gkbekjxps.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwfdbizxw.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gaycqblzd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gcfpohams.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqvxtlqry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/grayupsjw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gphthcswe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/grkjkafjh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmcrqnoff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/guknggqin.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gswesygju.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvtocyspu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gdmngpren.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gvoqsqeot.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gegzhuczs.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gybeweqkb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gopvmzkwr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/guqhwfwer.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gdkebuuxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gswxrvaly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gtuwyymgm.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggdpfzgqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gmlfwvkja.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gassyqntn.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gmfhfbvsv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gbtszbebn.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gokzpinil.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gfqybzfeg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/guibpcbjb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/giiubjsdv.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/geiqdbldn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggghlaypv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/goximndnl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gmjwglklx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gxvzuafga.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gxiqfrcwo.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gkknknsqa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/ghlucopbp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/grdmvfswb.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghewfwxxe.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gxswqsdxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/glhocnoca.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gjkrrrhhz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/giiizkzqs.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gejhagamk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gcfgeycmh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/graxhloye.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gvclznlcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gqouwgwna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gqekflxjc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gyuwkaqbw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gahgiucua.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gumuweeng.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/grosxnslq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gojzdikax.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gqewgggxf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gkpdmftvj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/genofabhr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gunhezhqd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/ggugtgkqs.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gchcvivpg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gbsvnatko.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gvacmoihx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gwapcvgcp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gabtaktez.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gmtpebrua.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gtftutbil.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/ggpmtiszu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gbixsskox.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gmvwkvisl.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gccpmllsa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gskrggxps.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gaysnydyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfwjdykhm.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gljnnctsp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/ggejghffe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gswmunxfk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gvcmjmlbe.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gbvgfrbwa.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gnioazkfn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/grbjwwcgl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gizsaeeqe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gjzhqfejq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/giprtbrzx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gnbylcnvc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwzzrnizn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gptvhzfzp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/geatolekn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/godwrbyck.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/grpdtzpey.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gqklgggwu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/glguurhsc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gdcliftyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gcnelyyep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/grnimubht.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gfbbimfrq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gzzbnycgo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gwxmwfkwy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/giwpaqpgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gtohospsq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gxzsdvozb.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gesfmxjmb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/ghcjyajel.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbwrushns.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxeosrpts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ggheppncs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gkjgswlce.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gcoojpqzc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gnyeipfws.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gmpcsgkkp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/grdwynuoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gcmzghknt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gupwsgulk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gtssgenij.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gvqniaacn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gedoiawij.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grjtlyzur.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gtfxhjkfa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gdqeucyfy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/ghqvftudq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/glajnptnv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gzwvviepm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/ghbjsxlms.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfxapmwhr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmzayssoq.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gapqakhgx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gdnsvatgo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnhiqwjdd.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gwseqkqpd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gtofbvyre.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gqusfzvpl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/ggvkdurdx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gibxgysrf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gjdgtxiki.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gspsrwubw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gxewoetlm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gfpmziatp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gqohuozws.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gqcaczfjv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gqutxmhkk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ghmzlxdwq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gggonioux.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gohupomef.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqrhytauv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gqlxezsst.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gblwrawpq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grcyhlnil.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gfpbkwysr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfhqhkmt.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gosldsjfe.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gyoxrhcri.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gdkntygri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gefwnhdan.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gmgrzvreo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gdyjbrywk.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gbazfdlvq.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gjupfrzih.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gqoiuhkni.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gxnqpggms.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gvtvwrecf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gbmigkyts.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gfwseiltq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gktpowhxf.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/ggjlpasdt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gjgbzhrde.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/geruxifts.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/ghoepzazb.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gknlaejyd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gdpcudkbp.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gchchiomx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gtjiyspqi.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gjcwbtoip.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/ghyjdrvbl.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gifrropxw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/goptujwbb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gsnqjjwwi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gidovaavl.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/grelttywx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gvsosekvq.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gclijqsei.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gapwcgoew.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gutrwgvav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gshcmwnof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gcdglxmke.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gqgkrrcid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/garepjxif.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghveergoh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gokgmrknx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gqdpvzvvo.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gnbtrerce.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfqnevyde.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/geyxdzxug.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/granbuqvg.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gumzgmlki.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gqdhaztjj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/ggijwlhbh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gfotabrpc.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gkuktlnhe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gnxvvrihm.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gygjeedcm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gcubcudvh.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gnzxnospw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gebcjudav.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/ghvuwtuyx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gvagxkfya.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gcpbrsenc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gmmvxcpsj.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gvvvjfbxq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gjqghgpwm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gozwmpgmo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gvhohsccw.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gaawgqkgt.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzdpfldwj.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/grwenjuho.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gphwpawog.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gabtbbxse.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gaaklqrlo.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/ggrnpeamu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/grwmpkjdd.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gfdtqbmiq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcrxltclo.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/ghzudcnln.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gtwsnyvsw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjrksyjkw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvuggnfoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gltrjyozi.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/grokrrixb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gwocnepez.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gcrzgtizu.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/ggvgcqbtn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/grrrsrbnq.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gticulfag.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gyjegxpgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gqctsdryb.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gkppbtblk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gohtwwysd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gacjwjnam.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gslzydngw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gdmvnhmlh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gancvvqyg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gsemnglll.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gnnpitxut.sHtML


<!-- 参考信息 -->