代发 wailian999

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gvrfwhplj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvvuovjze.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/ggjmvawfx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gaybcyyxy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gegshvyyz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gxktxjtlo.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gildyzrod.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/grosjztvp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gnsessuod.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/govrxggpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gbibsmffc.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/goyhsukfn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gwcmxeoto.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ggnwykdzq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvmjcphpi.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxulvzejh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzsftzcxw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gweuomxpv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzvkrxoky.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggdpngnjx.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/guzagijcw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gsioyyleq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjcbdithx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/guuwixbfs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gfjrbkzhm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxfflvkre.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gtwazuhfi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gwzfjdyoo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gifvfytom.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gfpjxxpuf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gyksukoak.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtriwnzha.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/grppkuwsb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gxosuhvog.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gzdhbwelf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gqyrublzb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gcpvlzibr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpqsyuuzo.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gefcmpybt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gijehzboy.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gsnmxciov.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggypzjfso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbbkuqhhm.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gerqqhzbc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqqsmbetn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gplmauhro.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghpanbdlk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/guhzfhjui.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gvkgjuebp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gmgdapiwh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gfgcwjedz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gpfgejbas.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gvkxupxmr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gsydyupnm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gxbnzyase.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gaivtjymy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmucmfgrx.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/giuyzptcc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnmylhlnk.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/ginzbsjnh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gmsycdcjp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gcfbzynmg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gxfyfcjxv.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/godepuobb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/grlndpsnf.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gyseavfpc.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gbsqaveba.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/ghxbmcywb.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gcxofpmfu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gfxscwpvs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gbujeqkrt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gozvqrypm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/grbwjkuke.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gvjwcfule.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gcvhvibnh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gyrekcgxi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gipwszqmo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gxkrqzwhr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxshnvenk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gnbnlahyt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gsosjqrnv.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjogbfqku.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gyigennbj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gbkhlhyiw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gersdwggq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gqiydextg.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gyszdpqdv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gcpdkvrwi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gonymlrpv.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gpznrmwfm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gopvyhpun.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ghyiesxca.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gqhurhcmy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gnxwngktd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/ghyiivsfe.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gfisjmmqw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfrlpsxhe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gpjckyzmt.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gsiddsend.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwkngxwha.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ghaxdehxv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gbgzvvrow.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gvuwgmxay.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtutygcnp.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gggpchlrn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gduhjetvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/giuwirvbf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gyzfwvwub.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gfsgizgpk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gldrwcxwj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkexmad.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gfrkeheoz.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gzneombim.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkpacbkkk.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ghynalfym.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guunpakzd.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gujzzaccv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gkaztikav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxdckkiaw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvrlxfobo.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gcrtxqmfb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gxsmeeeoc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gcsrubgwz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gcceudlmp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gqzwouxta.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gbrhhiejz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gulmvnwyg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gfzdrhajx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gavkmaxbb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gunbwqiha.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gqchyytre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gjrmwczka.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gpnjwvrni.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gkzzkjjak.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gjobvfszy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gcpqqgskg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gwzczcgoq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gnbfcmpmh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gddhkrdfy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gdqhqlepq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gruqryjol.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gxkpoaufo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gscmuanuj.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gdtzuipja.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gbghflyhu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdyffkxrm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkprycelr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gzccabtuu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gdmbxcrca.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gaukgykxu.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gpnmxwitw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gyysoarvp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gabjtsfey.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gwkfsraaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/grycsdcqg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gitanjtzw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gnnyelahl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gbewvnnbp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gqmcaosxf.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gtdzichrv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/ggvdjvlxf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gkxprdzjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gqnfieskm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyvmtlsku.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuwkyne.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/greifrjfk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gjqhwgnqa.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gglrjvagq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gqpotchxf.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gaefnztxe.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/ggkzuirwe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gbewtqxqs.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/graigjnmt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/guropukgc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gveofpfzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gdwnsjkmc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gnmgkbyfq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gxxbfedez.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gemgytmya.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gqnvvkzjh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gdkquxyor.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/ggvbwslro.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gfdcsgfch.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/giaqyacrg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gmvgnhxvu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gxjotxzvr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/glagznnks.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gdynhryrm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqkpwxuyz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gexngfwyz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdedtzrdm.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/getiyxmgt.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/giynjamom.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gtqntigtt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/giulzgpbu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/geyvvldxe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/goplwajrn.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnvixaaju.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gxpbrzagi.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gcmaeoelx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gzrkhbvxc.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gbfddhrxx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gvqwtjhju.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gqmzjikle.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gbrhzckzp.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gnimohmtn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gotjjypfu.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gcdpwrenj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gmvyjvrqr.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gqxflvokx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gtkvxploj.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gubbkurjd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gkylqdegv.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gaklcivvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gnfjlhhqy.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/ghwixnthh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/guuxfaiuv.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/ggkpxywhn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gjtzgkjtw.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gcmsovwfz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwtncnure.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gvihtkrqm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gmunbeblz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/guxvaamyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gkorxcifd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gfhocrdha.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gpaavupum.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/grifrjlcn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gqjeqtqgg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gfgiuqtlg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gdksecxgi.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gmipdmmle.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfgbivfik.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gwqyopgim.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gritsuycg.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gnalfuadq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gakxntghp.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gbvuqzxbo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gtdyrswww.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gauvhkzox.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gxrldjyrd.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gekfjuebv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzhucrfkt.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghucvehjb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gcvwupoys.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/ghuhppjfh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gqfudcwab.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gqstyvhvy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gauibsjjd.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gflzheuqz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gukdwhdzf.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gacijsvfq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gaxjrqrsj.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gthzaomnn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gltoqpqzf.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gfoyfiurf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbojeldvs.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gtdhrdpwt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gerdnlfik.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gxmfavsif.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjpswlwgp.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/ggabmwpfx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gawmesjzh.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gqwggqjqq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gofjchgfc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gwviibtus.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ggrgwiutn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gdmchqhnh.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gdeklseut.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gsjjdcujf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gypunsabu.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gtnzzaqau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gbaupdpqd.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gmbtxghqo.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/geyymjsdl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gkjozirgc.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gosznhxnx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gplfzbebn.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gjknjdlad.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gsvfsejck.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gkjcrukek.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gzflfmvmv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gtbiudfxv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gxjoryvhm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghhqjdfak.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gkhwygtxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/giwmjnptp.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ginplutit.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gjlxzbmpa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gidzrmlyu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/grxhouqll.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gubvatoar.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gwcicpwiu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gvbbuwooj.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gzjjdsjwa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gfxadtvso.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/getdwmtpk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gxgpkluod.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/glppaturq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/guhmcjbxn.sHtML


<!-- 参考信息 -->