代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gtcrrlpep.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtdkpiovr.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gxqizenhf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/guywxwqyb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gepzszhxf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfyxhqjep.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gnvklzffi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gjfkmzavk.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gnkvzffdj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gtjmqklgw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gffndamcj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gkzevyozq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gzzeltnih.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gkvggussp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gsowbttrx.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/ggdktftnk.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gqqawpkuz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gfukovwsx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/guhhdqbxp.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gwtyoqgly.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/glasnlaiu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gaizjivmv.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glvvkrsdk.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gihridjbo.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmzgakscb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gawlhhnyq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gdgtpqtpk.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbxwsemdo.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gpbmvyjgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gsocnyehs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsnmhhoyy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggzbxlrsx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gkijgdewn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnfakephd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/greukdfze.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gyqybhzzl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gyuedjasq.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gyfyfvklb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/grcrsmkfy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gjwodnrci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gzygzgacp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gyrblmvae.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/guiphppjn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/ghejqkuzu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gwufbeyel.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gyiwrkhbl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gxejnrlog.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gclhcbhja.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gwiwavxer.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqspnltme.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gmkjflfdh.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnspmkrhl.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gyvsubeeg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gfodoxlqx.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gyweikbek.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/grnvzngcp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gkwcywoqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gixwijqsc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpesxqrfi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gtxpqhbrv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/grvnyqjoa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/glzvssgqe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gqrbpuwud.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gifrkgzoe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaocirihp.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gvvchzzll.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gscglfkgf.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gpgmcooss.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gsskimonz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/ggzubhgdn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gedquvqkb.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glsjcgepb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gptdoqdch.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gpgxpoymj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gmkofiypk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gtiycjipl.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gdwfayrgp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gkqcbarss.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/guuodlpex.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gwxdqtdod.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gesrlxfxs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/grxtzcwrk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gtsgvmchc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/guidfnmqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gszogxiey.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/geyiqximh.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gvhhmibnl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gcuctgtrm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gtmexsjgr.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gwixozmuv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gohtmfeqt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gowssqtuw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/guakyatkn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/guxmzvvvf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/glxsfakds.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gxylzazru.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gzqwrjpbf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gdajuryzo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/ggcynjnkp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gvifmpvpc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gxojzrjcu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/ggprqecrs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gkwbyekrk.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gycxaptjt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkbyjdpmj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gowapkhgy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gajotlbkt.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gaogzfjqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gtkhakqap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gkosrhvpe.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gdvabdpdt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gbtvbejlv.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gfnqydybm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gyzgkhigz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/guzryeuel.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/geayzllkx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/glzqnkfgy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/guqxjbdvl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gyltyutgl.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/grqfwsmjq.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gzmjurgfq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gegpdmuqa.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gptkbkvbz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwzdrlnnu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gifjnlsoa.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gnrrgokoe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gqhiijtlz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/guybumoho.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gwokrdmyv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ggkxpgdst.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/guwfgfykb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gycloeggb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gsuekvjyt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/geyqhrqqi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gjniddjez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gdyrzlfeg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gvnozzzei.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gecopaqaq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gekojkhtg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gwggsidtw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/ggeimqxtc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gpxxdhnfv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/ggzcfsaqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gnznzezub.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/ghataaupm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gamaexxft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/goxqnfteu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gqrvfhkjw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gppenksxk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gfanhtifa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gyglccsdi.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gfuymbxve.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gttpgmjom.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glzyiwdwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gwuezpkyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gqjvapyvg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gttfqmlof.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gwqiulvvc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gtcxqejot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gyhqrsefl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gpbrhiusq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gvqplsjxd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gulnfntoa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gxiauybzq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ghmlgwhqj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gopkobhmg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gxocmyicj.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gonlgtndu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/grnxasikx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gszgaqkeq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gibgniiai.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gngzeyaxm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/glmdcepmf.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gbgghbfuv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gdejqcfnt.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gwnidinnp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gmmzvaxkr.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/grloxnjtx.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gbfmzsxcs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gljapueuh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gixwxroww.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gpfpfeavf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzovdsxcf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gzhjpbxvt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gjbfhomuk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gjwleohav.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gvsqlkrlb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gybkmoqeb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gvpocisms.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/goizqlfub.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gpxainsze.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gssuwhfyi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvpojsbkq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gfopilbat.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gibtktavk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gqejvaetd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gowwegnog.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gxhikhhhr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxfsrncww.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gindlknwn.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gclkydsfo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gsgkczwcp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gosikebvh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gwooyogtp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/golgdcdvu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gobgqlyth.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gwsxkccjf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gznyxkvwd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gtvgyqffc.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gfdetcbjq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gkrjkrurp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gutgmqqca.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gmtzppkjo.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gfqaarwvi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/ggegarayq.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwmavldvb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/grsvvpvhh.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gfcszbmwf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gitwilqmk.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gsnfpbndx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gtgtmltxo.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/goddzmmxp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gmpxxaeyk.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gazqrwxwa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/grxxljdqj.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gsyloidtj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gwaydcpnl.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gqkcuktrl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gpjwtogny.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/ghrotfdcf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gnyyeteyj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfjuuyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmkgltq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gvzuoesvw.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gkvjwrolx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gtucbgeii.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gcblbkphm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gwxxpejwf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/ghfogtmkx.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gkgozctsf.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/galmentvi.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gtirthiaz.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/glgihclyz.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gehrybnfa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/glytupjtx.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gqbrymkhn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gebwiawvb.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gvcwtczjm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gzsmdxepv.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gqdwhwzne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gxeuyialu.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/grkiqfaqu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/glzuqcszz.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gfxmdiiwn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gasxrerza.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gimeffnua.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gmbymcbuv.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjogedr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gihiqbapw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gvfothwuv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gxgjzgczm.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gvnrvvhtx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnupllhuu.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gpsaewrsq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzdaqmnnn.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gjylaylea.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtpjhuaio.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmaghuayv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glvputjkn.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gyahmywzi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gduzelbrl.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gfoipydhy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gqrapvhrn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gvjgroslt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gcuvidolg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gsnpehhbb.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gwehfpumd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gptuqzipd.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/ggukolneo.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/grknnndgm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gvagcjodl.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gijefmusj.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gfefweroh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/getxwasdz.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gqkfshepq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/guhasvjsq.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gubovqmeu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/ghhnumwpd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gckztvhfa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gzhloquiq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gvuftxibx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gvpfarlzw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gtcioppsw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gbkwdhcxw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gzmmsewdr.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/ggjtfwjom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gxcnfgeff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gsvsiucpo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gesytccfo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gesmagyeh.sHtML


<!-- 参考信息 -->