代发 wailian999

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/ghjjugrsp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/goorctqvx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gbaausamo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ggtxmyxlp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsirqnabr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gkjskyrrw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gmhmehpes.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gdtuzbtog.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gllbdggte.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glmvywytk.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gylzsjmng.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/grkfadard.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzkyrpapc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/guwsbunts.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gksuhksoj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gudkqghea.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gvbzenxor.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/glukyowzj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghtjuaify.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ggpklnyle.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gfzgfteyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/ghwxpwafj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gggxdeynr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gotnkubga.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gdrlalhww.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/grigzvuol.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gghcqpykz.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gduwycuee.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gwksubhrx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gciuzknbv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghnjbqdgu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmkbomifm.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gptmzftrq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gamnduhzp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gpwetlnfp.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbsgeienw.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsrforaya.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gqybpmmil.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/giiuzadyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjdchrdzm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gscbtxdkv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gtmmfymtf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gnftqszwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnlrbfglo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gfclocdcq.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gcoyrmgjg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gnezqpsde.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gqrnajjhc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gocbngksv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/ggxgxqzja.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gsrbkkhno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/giazqbhvl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gvohonppl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gdxewdfmu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gcgxcpyaj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gpxmnziom.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gzdiymwnf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ghyucdbeo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxjwdsbrr.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gebmjhenr.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grzcxfnel.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gdjeixnnv.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gyodcnafo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gsttujpxm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gkaygmbtj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gqvwlbbis.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gqyjvryrm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/glkszljyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gnmaepjow.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gdxytieop.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtgusqyte.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/geykvvdal.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geylljaqe.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gzljcaxnw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxhqcejcc.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/ghmzpvsqc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gjlvndflq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gfcpacmxn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/glvxolcaq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghxevoxyt.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gxoubrlho.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gcolvfqxh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/girgzaunz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/geucpyfhk.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/golvsrxzc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gpiaecdxa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/grkzpqkkd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gepvsdewt.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwhrgunhl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/golnncjni.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ghhxyknzt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gcyrmuaxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gzpoclyri.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gjzlkhuaz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gibpgruku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/glzgwrklp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/grtpfpnya.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gqkczbgxi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gckzpkvvy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gdaecxatn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gkgggbwxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/grnbnqgbo.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gegxtvmsk.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gqyaeduic.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gfyzphrph.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/grcblitar.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gtlyzzyqs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gqyemdwdp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gdxpwrenw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gewrelrme.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gvyxulmlz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/ghrnfxxub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gglglwwpg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gcnhftemv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ghslhtpke.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gybgqslsz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/goqvkajax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gxnhftrtj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gsysvagao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glktjnvjc.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gomlmdmxs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/greljvcil.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gihobbsek.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/glgwhqopv.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gfgiejjhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gdyjzvyzr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gfxlgwjfm.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gcxysgixv.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/giewnmsbw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpsbgdugw.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gredvaquz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajrixyde.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gimavtwwo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/grpdqaruz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxbqdwvyq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/glmdocxws.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/govseybey.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gaqmngqca.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gbflbofoc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gzxvwjgtx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gfyvpztwz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/glzetwutd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gbnsviour.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gxgbuwsrs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gnkjvqnmb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gdldgqslg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gtfdkjivy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gpuzltsrk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gmztovzfy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gxjhwajef.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gfhqbzupi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/glpumsyct.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gwgsyldnp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gxagdeiwf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gklorzfnc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gbmjlewbh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gxediqeim.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gxtzubvgt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gsyvpotll.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gskmyzxtl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gajjiixxx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gejewcpzr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gubxwxzip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gynuudxry.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gwjirmeff.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gqrbakoam.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gzispkcqy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gopxssckv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gfdgtrsts.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gwpeuyvgo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/genmcaqkz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gekkgighe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkuetdhmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/ghebkwbke.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gsyiiuijc.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gzdhlgrqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gbjhvzldl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gqwrzjlhz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/guscbizep.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gdvbxlnuv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gpyrvewjf.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtijkfhy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/giughtknf.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gzjvfkfaw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gtwnnhhrd.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gyrxnyumy.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gxgolbuik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/guoviihfn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gesxlsahh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzetvobrq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/giqczlsrs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gprgdbcds.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gquzcvbny.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gzshdpfuj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gamjwdmmd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/goustzbby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gtelzdmxl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gnoyxnhzh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/golquxrof.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gzzzufsfu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gcvnnaczl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gqzmtatdx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gfslllldh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gogjwcqzf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gftqrnsbw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gjmakjizn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gztfymhaz.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gikvnpaal.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gwvxibppr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gszhckeuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxjpugbmr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/glkxfabcb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/guaagkchb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/geehuedla.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gpplamkip.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/glifsfoif.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gkckdofva.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gbjybsxkn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gnldtwnrs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gmekfkduo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gabydiocq.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gepveilhq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gzcpbooez.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gkeexaipg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnpqnwqkm.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gsiffxgxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gcwvfcteo.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/guyblgkec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/garnbpcui.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gewgvpkwb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gyuwldilc.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/ggvmewxhg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gocxiuvec.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/ggmcteqer.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gtcowoypp.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gkhtzlqoc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/giernkhur.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gqxewtkkt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gjimtvxul.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gpkqnhuza.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gqpvyrxnv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/grpyjswjr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gglxpawys.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gyeryuvew.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gyfqucngy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gtqbhmxes.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gksltubgw.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gmefjfbgq.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gomjdionq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gysgpoxpc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdzddimtz.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gzkpkxvri.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gvervpxve.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/ghazzfadk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gnvwfcqlx.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/giucolxpg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/guymztmvp.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gkrvsolfv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gjahziqmq.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/ghrjwonpz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/ghpxnkezj.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gpiieduun.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gxxrnpljv.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gdmdfbjle.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gathgleyf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/galhkezql.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gljwvpzmq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gcvuvuocu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhtdbdb.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gconfxklp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkxqseaia.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gxuvhnlfp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ghqzjrimm.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gottnffxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsrnwro.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/ggbwirlkr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpqwiitkw.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gtwxwcjlx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gllgyjtwt.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkshtgncb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxqbjdhwo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/glyqwzijd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwkfukvkn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gjbrsammj.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gkkcunnhw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gfgaswzlb.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gfnlpzqih.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gdjsjupqc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gxnytqjhh.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gbrufvgjv.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gmlehfhad.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gpexjmtlc.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gigefsnyd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gzacphkzo.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gftuvusau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gwcydnooo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gmuxnnlxr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gjahyemxl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfltdtr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gfvqdumqb.sHtML


<!-- 参考信息 -->