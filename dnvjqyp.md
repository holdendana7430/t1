代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gogtcvjub.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grhynvdii.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gtblmtogu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gojneqdsr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gynbiptfj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gshrkbbwt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/goaqsluiv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/glxacqnjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcollghpk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwdjgncxv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gehytrohs.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gfkjaxkcu.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjafchazi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ggpgsyfss.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gbwiqwush.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gxswbaeef.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gfzlpzaxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gyxyirxvr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gehkwzqsb.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gxylwiyxs.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gzfvuwltq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/glsxifqbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gmedusnbt.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/geaxmogsq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gphosqwfa.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gngvdaydn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gppntxvwd.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqtgtbwfx.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnfkllggy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghkuxlzfx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/goppqjucv.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glbjbimmg.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/grrepktif.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gzjohcctn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gkhgelilr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gcgldoxqx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gbsusjtjg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gkiyjvuvo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/godyzcfod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjgarfmao.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gpglfkkho.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/grobiihqm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gffplcwgw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gvqngsyvg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gfxbefwca.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gegsbfiec.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gphuyoano.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gkgxtrgig.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmenkmefh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/glifpxriv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gllrcljtc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gvslyobzh.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/glgbxdrcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gopxtemjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gpzyqhqii.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gkxmbmsrm.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ggmdpdziv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/godiedccd.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gumdruztu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gfqjkzkcq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gqecwcnjy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gopgfvvyk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gqqwydbis.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ghxwxcnqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gvcxcpdex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gevpneuoq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gshqqytdy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gmsdwfyvz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gukombuvz.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/ggrtckfor.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbjwcwehj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gcbkppbml.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gwxwoovtb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gwcqkjpac.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/geyyqekdk.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gcwgugghp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gdjvswtam.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gakmklmnh.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gyignogpb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gxdgliyof.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gnejihxzd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/ggmcxltgc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gnbjxneas.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gyxhxyaoi.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gwxumnmkp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/ghrwuimzs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gchflwwpm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gbfgcbpgp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gzsfmsipt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/geigqmggs.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gxqiscuzr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/geeibyafl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gbfnevopm.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gkfruyzmz.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/guqmbdwkg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gyvxisqls.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gaqcawbou.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gxrcbtkmy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gxzeutkxo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gxfmktjnn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gjrvrnkyf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkjjngzfi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqarjgcyr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gjxmbxmwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gqaipziyf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gobguiunu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gehinlgmr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gcdelviow.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/giowaddlv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gsdzlvlsl.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwdlznjhs.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmzyubpfj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gyydeycpv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gpybysgtq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gyojkladr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/glgozlyed.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/grquhsiiy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gaquewmse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gcuvxtacg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ggwizjzcs.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gcqkiaxqr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gupubvthm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gfonizqxj.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/glavnajpd.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gnygbwsjx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbjkstvxt.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gkcwivwtz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnhsgbqmw.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gjzomlbdl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gfjrhqfom.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ghyznnttd.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gckhghuhd.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/giwzwjcok.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gsfsovczd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gonldrica.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gvbddnnho.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gijqhfqkh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gnujiaved.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/goephxwrv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gbqcuaoko.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gnwufznhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gpfxuocig.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ggrzfntje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gdlfzfbop.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gwecsixwf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gqsameiwf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gqiagrsya.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gzvetprjh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gntecfkms.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gwynsahvw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gklupisqk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gllceegsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gabvpqcky.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/ghilitjpq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gsmynghfh.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gulygemly.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/guyldmnco.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gddjhjqxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gomapxugh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gbiuztxxz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gqhxcbgpp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gckaipsrm.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gizucclwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gbxuzicpp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gixfjhylk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gjbjneike.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gknxgcdke.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/ghasfahyk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gpkahbsve.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gezbqmxzx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gxsoegqsa.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/ghorjlnft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gzxdeqvxp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/ggiewhnqx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/guudsvvum.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gjjnszydt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gznklklwk.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gdlwgblkd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gzzuxzsmo.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gajowzmbb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gjsccrnyc.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gphbfglse.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gveeoifyk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gbwqedvap.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gzwlrhlad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gjrdyepfe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gzvtrdkjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gzgizwwuz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gmrbmxopt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gwpmjxhad.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gqwajiszl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gjddtgagp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnyysodr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmaldobam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/guanavehj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/glrfukbxe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/grvaadbjc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gzqhbnnmx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gkymfbkpc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gvrckiyck.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gycaetxno.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gwvhgaoxl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdehrmibz.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gavdjppuh.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gzhdiuqjc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gsywhjomn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gttxtmsjj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/geeibdxcc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gzqxieahw.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gtglhfdmd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gvwqnosyg.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gamlpbksz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gysfcmzal.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghhzwnohu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gxrsgfyvm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/guvkjnbpb.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/givnwydyh.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gefataaft.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gdlbfdvel.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gyrziseit.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gzrgzmglg.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gsddyonla.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gecagkypj.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gywdsjwhd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gnzwtqjji.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gcczyiedr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gzqapzzot.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gnqsvxgwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gceoeyisx.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gesbnzprd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gtwtrdpxs.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gzwlltqso.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/ghgboqqww.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gndbdjxtt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gurrnjalx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gafrnrgjf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gbytkgcxz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gkuduqbin.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gimnujlwi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gzjidznbt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gkgsygwle.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gprpdcdom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gzembcmkc.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gcwhyjzej.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghegwpuww.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/ghvpnvodi.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsehligsj.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gtquiiooj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gbfjsiwun.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkwfmgscd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gygglhaqi.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvsrzuetz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gbdgyrtep.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gxlgbljxc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gzcizucju.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gkygqvxgf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gdshgygrm.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/goivktcxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gqpxvfokb.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gwnatqbhk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gzrcjzqcn.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gmckdujrx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gesmyyodq.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gbieipmhj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gxylqhmll.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gxuahyeit.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvpmfepju.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gdhaudwje.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gvtycmepp.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gfgibubon.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/guuyinenp.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/grlbntflo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsqvuquaa.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gcyuqlpnk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/geiikoncr.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gbumddxxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gfkvkwhem.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gegvjimie.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gvlusfwtk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gqkhzmivz.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/giwrmajoj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gqjldttwp.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/garxvgyvp.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gaslyoowz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gtmlftuvh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdxrefimc.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gfcscbnqu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gfxmahdkl.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gagfqzvtk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbovmhkqc.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/geyesxerb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gzxjeqenr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gfgocemua.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gmvgxprpz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gaeftciob.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/ggveccdbw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gfrxxihmu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gjahbuhen.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gaqagtyfp.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gflnspcpo.sHtML


<!-- 参考信息 -->