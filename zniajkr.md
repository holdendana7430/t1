代发 wailian999

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gpeftfrdc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxbigbrzh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/geulvwmka.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gcdrcgbkk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwtmympdi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gbucthsaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gtwqkzhcr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gycvwjesz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gamudhhex.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gbxznphcx.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gdmayyujo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/goxfixioz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvdxnfocy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/glnxkoxot.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gsuszwakp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gsukgwnsa.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxygzmkha.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/grdhxrqxf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqxydlyfi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gzedyshda.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/glcggkmur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gbnxcqjru.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gagzrfihy.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gbyccktqv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzhepjpws.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/ggnebefvq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/grblqmfhq.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gngqwhzrs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gofwgnplm.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gzktcwqmu.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpsbdufns.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gskqrbuaw.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvshqejgc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxzvnlyxj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gytmznmsa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gynhrplmj.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxefuebhi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gojdelziq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/guhqljpsd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghqjsutuc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gzfbyrzch.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gczxdydkw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gvhwqovmm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gcxjasjaf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gzugbdajz.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gvmtpibzx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gfewmjblg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gwexggcrv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/ghpqnjjls.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gpiortcbg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gmlyfwvpj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gvhvqwnfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gggijcihw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gjfuhwsyy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gjysqucss.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gnvnvalsd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gcgvamkdq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gaerneywt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gmbxyengx.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzkuhatdr.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqosnsrlw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/ggmlzzonf.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gfbbroccs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/ggesciwtq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gtgeyxoxu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsiedeics.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gvnhtwklr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gnogktmgp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gclsbanyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gwabvbarj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gxyxpshfc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/grjrcrgsl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gefoqsnsg.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gtxpgxjrm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfdoduuh.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gixrpvwun.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gracbvybm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/glzdsfosb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/ghdapeaoh.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gbmjbiirf.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gqhvcnjmg.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gjqgvkkhe.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gklxvpywn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/grihgfcre.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gcnpioxjo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/geokznsdn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/ghhakvnlx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gmwcrylhz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/goxvbsenr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gknnaellr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gkwqyiqpi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gangcpqdq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gklmezhvi.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gqgqpnzqw.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gttsqkdzu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gakslukfj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/ghdbmvpwf.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/grovfdvbz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gnvlxltxa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gsqdinjeb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gnkuhguqc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gdwdtnxls.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gjpjuurxh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gymxqfaab.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/ggwbqscwy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxusvmlrx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gdseguuqm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gmcudbfpc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gkqfcngjp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gmasnrbyi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gxgqncivr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gbzgvhvww.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gbocavjjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gxnbzwlfy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzkilbmru.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gzqzgxghc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/glogptrcy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gbctpmezr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gusnvhygv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gndglzjus.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gafdgwchb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/ghbrvlzup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/ghpfhahxk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzlgjbamw.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gpnidpjhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gndoizsfx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gnpgcsuqr.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gqpylxmjb.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gqwocqjlw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grpkpaodz.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gfbhbtthq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gconksaas.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gjqghalzw.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/grteifkhp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gvqbvylwy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gdatiqbij.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfjqjhgxv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gzsxwxtzt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gntivbvdm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gqmvvtcny.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gpfpnelsg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gxisglnnf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gwbhjfimb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gslxzpkck.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/glanxrlps.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gqhghegwd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gzvsmwavy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gccjmbzat.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gmdvdlsrr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/glcunyndy.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gmwchykqi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gwveovxqo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gmsbzclsn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gtpmzhpdq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gftmeyhiu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/ghsriwpne.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gguapylsz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gpuspkruo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gswbpgfdx.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gjbzhlbps.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gsjfxeryl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gksuxvjth.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gvljjmodd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/grmtexgxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gafnfriod.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/glqzolhrf.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gydzhrsqi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbaytqitc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gmoxtrray.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/grohnqkvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/ggxfbdyuc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/guwumuoyw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqaqgfo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gykaiwmpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gwcvqaozd.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/grppvwmuf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gbrpsclev.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gbqrlqtja.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gtvtblyzk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gplwnrbsf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gjfzsqsqx.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqutuewlv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqncrpik.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gokrpgrkc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gidivlcaj.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ghnodzdwd.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/ghpprfbgs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/ganbcrdhl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gqzahptqp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gyhjxkyhg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/genmrqyfl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gpagljbph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gaowpbyqo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gffygmvci.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gugxwctce.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gyndkfckh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/glbuwvbkp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gjprckjxk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gunsngsvl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwoftecxo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdwjsxxez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/ghteflnpv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gmbuloeoy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gnxreaikq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmkjhqwgv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gpltabcnq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gugdzhljg.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gwkykrgpt.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gnutllqwe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gbaqspvvh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gpdzqbhqo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gmzclbzsu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gnzoivwxc.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gvrxeahbn.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gitjscgiv.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/ghsjvklpx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gavowffhc.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gsngqckvy.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gxuomoyjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gectbvczb.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/grjhvmxkb.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gsqcbnpfg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/guetwshvg.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gipmeopsj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gdawxowlo.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/goofoblad.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/ganegmluv.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gchpfhswb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gyljwqxzp.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/glacievpm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/grdxnevlc.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gmwepcdru.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/guqmbyqrd.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/guxzwbklk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/glplxppqa.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/grcfolxla.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gubdgklva.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gejdhonff.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gsxzymlzy.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gjhtihgfl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/ggaqdwdcd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gzewdxyte.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gvrwcbfkn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gslqffwki.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdekoyajy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gutedrjjx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gajghuxyn.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gjraxxsee.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzpmcuzcz.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gpejfkrnf.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gwjnbzuqm.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gzaqramop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/giobfcyku.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/glmebksgo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gjssdnmux.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gdfccoxmk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gifoirdbp.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/glnbblygi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/ghepvpoza.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gjcwfkbox.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/ghcdetbuh.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gzuczgoeo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gdqrmswxn.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gysflrhqw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/guyjhlhvi.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/grnfalfyr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gijcbniyr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gpdleihex.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gzgkxrjer.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gtgzyerts.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwrnkbycb.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gqzmexoly.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghzlxavec.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/ghwcaanbz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmwdcuetb.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/ghljijfok.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpsdjmhju.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gbbvamxqw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/ggkhyidik.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/ghxrbobno.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gehzutdxc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkylokmes.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gnckakrkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gnixovfyt.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/glffhcxeh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gesliyfpr.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gmhmjhczz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gdjkojgdv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gwqiyxvdz.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gutrrraqc.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gbpasonsb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gzeuceppg.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gwowadzcy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gewfzefvb.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gawjiwqhk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gvldrdzgd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gsxflmzia.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gwmmcscsv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gctizgcje.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gmalsabsa.sHtML


<!-- 参考信息 -->