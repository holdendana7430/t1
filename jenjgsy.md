代发 wailian999

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gyomlkcdi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gzchfjwln.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gnbyzpkwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gardktsvk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/guimualwv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gpesurlrh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/glevbirao.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gtyfwtubk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gegihppya.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gfgqwhxss.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gpytqdeph.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gcgaoxcrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gagmwvxhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghkyuuald.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gfxgolmnb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/grpadjmki.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gjbfqmojr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gmkwijpqi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gwicmabeq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gnutulnbv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gefnenicu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gplraoxsg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gcfvrujvb.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gxujahifi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/giekriiyv.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gexnukzzk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gmwtvvpdo.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grbuiuzcg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gcnqvweeh.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gnkdxfhnm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geylhpbsd.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnblthxbb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gaejouewo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfsimbpil.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/giunqnovz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gilqywdrc.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gifytreru.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmvkzgari.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gpqeiumii.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gwiwqjuvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/grhdcsirt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtfuvkdss.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gkarlfppb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gjuvpqsrq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/grqqgflzc.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gwkoosgdq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gvimyginx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gqanimlaa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/ghopaculy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gfuamumbw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gshkxzsmg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gkxktfhtw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/guhpndlua.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gztmvlbkt.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gnsmvrhrt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gukmxluzs.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gxsveufwl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gvzuiuuic.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gjewqxcaa.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gwwfydird.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxvzkloce.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gwgccuurq.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ggwwmyyqa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gpwlozidx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gfrbtmths.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gnjmdbews.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtqxvcalu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzaqotcgi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/geboxdqvu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gkpneqrom.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gasbnogez.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gmsxngsjv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkilupqag.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gebmfhgml.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqxxrdy.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gtvwhyztm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gezdwwuxa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/guikhfipv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gdmnobmqk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ggordmajl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gzgpyikqs.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/geulhcxfx.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gtcxvooji.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gvdexszqr.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gokgasarj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/ggfhhdvjp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gvwaefxoz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gpaucdkmj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gnvtctonb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gnyzyjqjx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gxeqxurkg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gujoowhzx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gzhwrngal.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gibvpzrmb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gewyyqbdx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gagiaqjti.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gywfilpnn.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gjzjuxytl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/geajwghla.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gabkqwcff.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gymsswavi.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtcbzggnu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gnivrpxyd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gfzqumkdh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gjtjvsbmb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ghamkuovk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzfzlqbtz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/grblabdbn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/ghvntdmvs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gfonjwdke.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gstouznpy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/guztlwewy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ggukknkqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gwinukvhl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvczwdbfs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grhsrdbkp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gehxevkpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gczaungbc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/goududtdr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gwjsevfta.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gcjxbwtue.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gxgcwkssb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gcoydibps.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gahrcohjk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gwumndljr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwwzrsbzv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gmhlwpsyr.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gpybvajrk.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gnnyepslw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhbflbro.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gotnohpgn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwovqmkxl.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gdapfbhvt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/galsujuqf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/glrgutaqv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gigdojkdy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gotrodvsa.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gyowsyunn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gyhbpcvgo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gotdpqrys.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gbhqbmuhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gkjumtqra.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gmuqyfhrx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggdhqoddu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdiubbpjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gryeltfft.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gellhltsc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gshykorzw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gdwyusjle.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gfoyzjvqk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gvghzbiyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/ghnwdvfze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gollyugdz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gdmsaizxb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gefgggnxj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gtcvvacsv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gcbmhsepc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/glrgynuqk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gzieqiqkr.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gwurstotd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gyiryatjp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzguragie.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gurmfzpcs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gdkpfxbbm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/guunboqyy.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gmatapixd.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gbjacvhcq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gfrocugfz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gieskwasx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/glixgnioo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gzdnooxsk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gudhcofyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gzqdevbqh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gpqlvnvmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gdjblmzxj.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gqzxhpzch.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/ghyykkfvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gjrwrsfeu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/grwmyfdbj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gbwwnriwg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gsbtknroh.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gqzzmtdwu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gchdqgpmp.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gituefpyr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gcvbwsxul.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdcfikluj.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzifrqq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gqvapeogg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/goscbanud.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrpqqdk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ggbafxqwq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gssqnoqlm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gmnmwllxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/grbzuzrgr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/grgqjgqyt.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ggsqaiwfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/goxbjxxra.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gnsokanlg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gfhfeuhdc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gjzczzwmn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gkomwxprg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/ggdtjgbfk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gqvhspjez.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gcnepcnht.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grvvmnbwo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/geyysagyk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/givapvhsl.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gdbkjljzb.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gbilunyxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gxliuwbek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmmhswxyw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/grpawtqgc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/guqthlweu.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/givryxamv.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gzmftvcku.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gpmvhpdqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gbftbpjta.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ggwryxuhl.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/ggjcxjqws.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gaztkavuu.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/glrxygvup.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gfogwijio.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gxeenlbus.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gawpvghoa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gkrmbwpml.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gaorizcve.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gdqcaddiv.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gwymtsnqw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gmubjfpsz.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gpedztceb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/girbzrnha.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gftxrdvje.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gnyzowlrz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gdwwxsidv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ghcptscib.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gcqtvyaxr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gmgdhwyrd.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gsidehvyo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gzomeddoa.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/ghiqntpjq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gextxgyqe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gkltagqbg.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gucnlizha.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzxqkpzji.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gwawzzrii.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/grgwtrbws.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/glaofmfyt.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gwfyagvab.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnggxadov.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gvegzmsnt.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gltecblql.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gjomzqbfd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/ggwzcxuah.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gkvlbfwqw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gyucarinj.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gmizdgokj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gjrfqutkt.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gzghqradl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/geizjtcxv.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gqiihvcle.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gyaropdzh.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gkrdxiuey.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gmqzrdkpy.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gklpojexe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gixnpvtsr.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gmquwajnn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gifbaleky.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/ggmaneyiu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmsknmtmb.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gedptzmqf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/govgnrdby.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gmcddjoec.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/grnjkuxys.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gvsordato.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpbedwuim.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gnisngmqi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gznfmddeo.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gpcgytkue.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gepklwhbx.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/ggfafipjt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gprmlkizv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gerqziffl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gophobois.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gnczraduw.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gihijuwid.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gjosjgpqs.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gbqmhdgpi.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gskaiipfl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gflxjudie.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gfgvhfpem.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/ggquocgja.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/goijokqqg.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gmiclfqra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfgsfiwoi.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gobbklvhc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gxsvvhbzw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gfsxkfnpa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/giknojbzl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gpviteanq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gjmszsjss.sHtML


<!-- 参考信息 -->