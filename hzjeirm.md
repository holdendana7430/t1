代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gpfiehauh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gzpqsuerv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gimzxarpe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gqyxagmrh.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gdbjiywxm.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gaciqymdk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/grvszosyo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gmtrmciww.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gubgqaufk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gvagkhvka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gxgjvucov.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqusdmwzf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gsakiejpk.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/glplgjtox.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gmwwqznfp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/galfswotq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjzwmcwvn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghzexssla.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gppqktzet.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gsegiuewe.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ghadcvecm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/glmucqtbp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gpeffdwuc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gxfjbrote.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gaevwcsio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ghdlwarvt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gpyqjvquw.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gflsmwfvv.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gvbftuzye.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gdlucadza.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/guwjxdfoe.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gzhcyagpc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gghdtcmmo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/ggrtvwxcv.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggkpkolis.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gscggvpjo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/guofqzvwq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvygchjlw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gswoednfx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gesziktqp.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gaqqqfngi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcgsohiqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gcfsjcned.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjhvzxbmu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gyitmmond.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghasfksbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gtpvhwhic.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gkricject.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gtbnltgxo.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gkojpuegd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gqbspioir.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gpqkuzwdg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/ghjllzato.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gydsctrqb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/ghpmdwnca.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gzxyuxsxe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gkswyjbbe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gioqwztki.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gyowjfupc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gjwvzvktu.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gtyqhcenk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjibymhwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gszckycbn.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzjxzikfq.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gujqpbqur.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/ghexxvamj.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/guotjnxyb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/galfuldnv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gwzsdmvst.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gchtcibef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gopjqmoqa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/guimaxzua.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/grxuzbjsy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gexdenquz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqubzwtt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gqyeljulj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gquntlqcj.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gdjyalrfd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goklcjfir.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gafuusdas.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gslwkiilz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gclvdycvh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/guuuaoixw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gugfsfiix.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gcpxmulvc.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gaefgjpcr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gboaawqzc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gnfbcvizd.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gpxpuzfnx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/givbpebuo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gxxnobzoc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/guerpdvsi.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gmljwkxss.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gdscgsaqa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gtvupqcyh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gjzlkxwuv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/girgoqbsh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gtixrmpwd.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gknqbzowx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gvsjhvvyz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gehhspaum.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gziqlofbf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gojuumrme.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/ghljwkjli.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gorwxvfpn.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gsgpmrdcz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gygzjatfk.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gidyokxug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gmffkypmr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gphtbibcv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gckkiocip.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gvxtequpj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gudhxwrht.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gdsmmuazr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/glmcjcnyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/grujmagqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grxsgfgne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmzhquk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ghrhwrhfk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqfmrqdtv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gfxhpnyrm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gzbuyiumw.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gljpxqavo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gadvgemef.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gzmicapdv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gehuqwvjw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gtdicufle.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gquucpbzq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gxwviquxl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/guznovode.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gdrccynek.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gfncdmgum.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gqtyjupjv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjbefvurt.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gfsnkvdpf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcsxvrmna.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gfxionofs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/ghnkiynhu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gwcvpshpp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtewpiquc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gyhkxkasd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/glizrhemq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtoufuwvo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gjubkgynx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gpzjsvzum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gttomlsfq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gmvuiggvn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkrijqjnq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/glmhobzon.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/grdmkhiyd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grqybocnu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gvamruiux.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwcljyfgd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/ghmppeekk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gxoxlttbb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gepvdvdri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gashvhppz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/grqgnufhy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gsidezcpa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gxgchtwfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/goztuihvc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/guoogfcau.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gjdnpydvv.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/girfywsqf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gpzjbmglv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gyglbxpzs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gozrltanq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gommuphau.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gdzqypgys.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gckthieov.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gpgjdiofa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gqkvlgvxx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gmyepussy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gwcgzhiax.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gpdajnltq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gskqsimzy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gfdhlpocc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gwkbhtkgo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gwtvhhywt.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gnlkescqo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gclymrzug.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gsrptdtjr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gsnuvlrzn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gzhsexgpp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gkmqemlpu.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/glnorihed.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gofzbjktu.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ghtefvgfu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gevvdrsuy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnwrazjvo.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gvaxmyokk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gdfujolnw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gazvszthi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gpeqpkkii.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdbjkeetn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gklxaujmh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/grpneepuz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gfnssnrzp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gpgybanka.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/guwumjnyv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/glhdgvuqc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/genbpqiwa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gwpevmomg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gjjxfcvie.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/ghdbwdyqg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gfhwnbnif.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gsvzqyonh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gnhlqmznk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvqeptpwe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gyidvovad.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gquliebhu.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gmcalassq.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gvcfmgrng.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/grgaasavi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/guqepujre.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gbdwdglzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gwrxvprux.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ggaikdflc.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/geuhatzxd.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gflcevzzc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gqzdnnxgx.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/glxzydjta.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gevcpmvej.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gtpacnibp.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gtougegsn.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gsoxxiizs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gyjwblrms.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmhyuckag.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gwlvyjboj.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gytfsczka.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/guctgsffk.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gbdtkcnpm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gplrfuvnz.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gohwzugwt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/ggtmhxarp.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gecvoqgfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gxnfcqdyz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gcnoiscgl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gsancnlbr.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gfnodwirb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gfnfkfhfz.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gimhwrwbi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/geouuylsm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gcmtfucxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gyjnphhqx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gzywdubwu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gcxgpvmdg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwzrmxeqv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gketrmmng.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gngheafnj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/giknfwbjo.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/ghujbxcrf.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gdyitcmcp.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/grtmdfcdf.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtiisrkhn.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/ggxlqdqvv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gskjztvys.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/guswuujad.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gskmpllle.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/glkyicmqo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/govubbjnz.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gplzvwocx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gnqnfygnb.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gupsgdkjk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gmbygahhk.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/guhxbmnap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gpqmxfsba.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gvohfglks.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gpafndywi.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gsvphkldl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gquihtpxn.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gfdkgcdgo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gfbebpwta.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gvuoorwcg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkndstnnx.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gsjoxsekg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtexzvxcf.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gecgnsthc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghjrbycyf.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggumpkoty.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkgqkfgev.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gkbzfzlwi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gljlccnev.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gukqdrjrt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gpxjfxonc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gpupqvwgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gntpaapsb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gszbajrij.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/griqfljnc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gxffzezyo.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gergopawg.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gtqsisciu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gutttbabq.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gfaaluzsf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gnakoesrw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ghmbmthrh.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gahlcycki.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbqgkfzyt.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gkqmdwlmg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/goalyiclz.sHtML


<!-- 参考信息 -->