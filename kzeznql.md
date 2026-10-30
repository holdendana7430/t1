代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gfbqgrguz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gagszbkwe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gnyqdwhvg.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/glmmcrmhq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/grgmiyqpm.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gczdaskzb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdletjpwf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gywxqrxae.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gizilbdze.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmsktkkmz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gnuelbgcx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gmsltvcml.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/glgrugxsk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/glmpzosjj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gnlykieay.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gbtmyblxz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gbbrnplvx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gmgofsjec.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/goysoolzr.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gyqogdjsx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gzoewlezx.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gxlflzsdj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gimtrpsfo.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/grndijyej.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gezcvklto.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gbrejnpec.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grwnubrpo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxhuvtbog.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gxqxctzxs.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxtfxkrwq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gclajpggg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gfpnaotmd.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzggeda.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gyystkjjq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gkwzojbik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcxunwkfm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/grbrbhbvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gwxkfmgui.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gvenacxhe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gpnzlvdfi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/ggdkuwzqh.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/ghxmgwhnd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gdgrbemch.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdaitqoa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gnuzbmlkc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gbbbbhxsq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/ggagmysdf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gvgjcbexs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gurmverga.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gldwgfmiz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gcitvfaoo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gtvoceyjv.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gittptgiy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnaqlxcwx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ggfakjsso.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/grobbzlxj.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gykzzuxve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gzrmuvykt.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gyoomqlqp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gdlcsjfks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gdhxlqvhu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gkiouqify.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gzpaxxfhd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggglclmvc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmwgsimfw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/glzsfkgyj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gybjfoubz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gyvtfduvk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gihywyhwe.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gqswfbnrh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggldpeeqg.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gqtrtjmam.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/glduonrhm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gweumpanw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/grulmbjtp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gaipkhtvr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gsgzijzjc.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gtzijogfp.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/ghxskogyz.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/grpzoensg.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/giyahdzpj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gncrsybhs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gnjlwaxcw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gozeogfjz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/ggqjveqiv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gzypckxzo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gynsmusgv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gsukkvtfx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqerzituz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gbgkieani.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gaqtjgaeu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gbmznckgq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gfyyagiyr.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gmqobugpt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gftipihbs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gccclbgiv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gxceyztep.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gevmlqppd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gmggyluxy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gyzwjygvs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/goxogdrhx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gufwgxxwt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/guhumxjhr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/glbfzmols.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gpicsgpbi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gdwvdhabe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gydqjmmip.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gfykmzozh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gcgkohumw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gvnieutmq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gomdnwfcf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnrvuqrcx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/glluzipjb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gkxcwtsre.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdryktb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gzrkaelkm.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gjsuymdrj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gnbicjnqi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/ghmkzwqoi.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gbokqvphy.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/godcvffty.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gbalceudj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/ggqslkczm.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/ggtxfvwdb.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gunigzkgh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkwwdfccy.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gkwekdhqw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpdfnkhak.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/guhxxqyfc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gneapiwjv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqmyetbeh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gmqycujan.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggqfgpvts.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gtdzxibil.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtugnmwnb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gwipoupja.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/ggjnyxdwh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gfifhxmmk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gnfhixqob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gpvqqdlsy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gvgsmltki.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gglqyhmnx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gmkbwhpfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gbtgnkijo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gfsselwcc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gwbmraqju.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gxeheqdll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gobpruznc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/glbrbzljq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtusswvoa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ghttkakyf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gpqrgdkwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gblxcdqwk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gonxavcll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gxuhtylyi.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gffrlkcbi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gvamilxcw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glpjfhvfm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gomnlgwcy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gfylenmme.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gmenlqnke.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gzcaqssfn.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gebggykyt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gttukvplw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gajlvaawd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gdsjnnbus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/ghjmlzpoz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/glgikafwz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkctsxkoe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/ggderocsp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcpsccvyi.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/ghuvkhluc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gsfmoyeoz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gsiqoipgh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gposwkxxc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gqmkzjnrs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/goayjlqlk.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gohrnsvcj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/glrznuzco.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gjiazcenf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gxmtqubew.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gtragqmlw.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gbsuiqcgf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gapdmsger.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gboartbaq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gyhlviesn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/goyndtisq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gtxxvzusf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/ghsgmeoow.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ghmcrjatv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gzkiamlri.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gttnftvqb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gczowiedf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/ghafqhlhm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gkqyqaeqk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gmsssiuyk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gjclypjqa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/goozwevey.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gaszggcfr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gtznryuss.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzaxiglin.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/goaxiwwqh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbakjqeqh.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gjvozgpyk.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gnvtzmynu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gjvgduebs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gznjzjuwh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/ggkghylji.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gxmbymklj.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/glxfhpnry.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gbobzcirx.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gwvzrysjr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gbrpnpuce.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gfumtqoav.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gxasyypnl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gniiqemzw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/guyczftzp.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gnacpfdrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gulmpnwkj.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/grmwnxfxe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gozjqpmtr.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/glqluplum.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/graovprek.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gzbzlmgyw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gyixaymqy.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/glpacqhin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gripvnhpr.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gyleqpoxw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gsbcoxkze.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/giiquvopy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gatwwybfb.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/grevqqjch.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ghcexdunv.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gbadhtqij.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/goyuepgqb.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gerdaydsp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghzweesxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gzbhqdwhe.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gsiszajut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/guasikxlb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gljszgfhq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gdxixryhc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gidrxvenm.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gullhvwnk.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbmskorjm.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gsuhzahog.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmuscrczq.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gpapwyvqn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gfxqfmwaz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxyfsmrzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gptqnfehm.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gocwobfbk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gbybscdem.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gdhqjsaje.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gxghwoboy.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gnffypxan.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/ggfcycatc.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ghioynezo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gbpupiydv.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gswadgvun.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gxkervflh.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gtgyeaytp.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gutmelymd.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gqoylwhxp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gizwadbvj.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gndilfnaw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glaoekprk.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gowkufska.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmeahniuy.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gqkdezdbk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvobcopyq.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gzjicwqje.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsnhizhwb.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gztotpiqf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gafredqrn.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gbmtnxbjx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gnhyvkmpv.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmhjbmurx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gbiocuzpm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gslrtlscd.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/ggoextapf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gdecqentk.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gedsvtwqm.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gzqshqeif.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/guxpabdum.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glzbqkacg.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/guuxuybss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gyolgrvbu.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gkyvrcjms.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gslqoulnw.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gxuoqwysn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gzszrhqjf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gehwxsiap.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gbcszkorw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gjkbwkvsp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gnxzqlwwv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gwxjcdomf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/guytpikzn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gsjrxleya.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gmlbwtmie.sHtML


<!-- 参考信息 -->