代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gdeawkytm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gzxhdnsqe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gttacxibl.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gikxbtqll.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gabvowogh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcowujinl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gwwivkocv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gsgrmoyzm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnkmfnztp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkvjkfiss.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gbxamcoot.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gtntfeakf.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjiutspxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gwdeowukz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gakyuohip.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gaewqolqx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gydpkirzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gbcreeyvo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/grcwolxba.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/goqheglww.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/ghrdqzhjp.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ghtvhnlvr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gdegncshx.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gmmjzeovd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/ggfdidfvo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gruokbaqi.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gytgnkllb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkpdoxfjj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gajxxgirf.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdpvjeirn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gfnhdrucl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggentypuy.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gdddzdggf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gqgphuxxf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gytujwjfi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghwrgbich.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gcghawovj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbobkxxmk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gngscdpxx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjxdwfyji.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gephejzrr.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gmabvlqea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gjbpcfuak.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gwataxdip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gizbvjisk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/grutdcitt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gmxvdsvmg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/giczulasy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/glghzfcll.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gkyqwfuid.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gvgvrzucr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gfuuexkof.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gtrjwjbdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gwhinanea.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gusqcplqd.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggfnsdbiq.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/geptywhxk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gyxqocryv.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdvpdwk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gkszlnvag.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gdgpybjye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gmhkdunfl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghigyjxyy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ghfbwmhks.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gdrtpkuyx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gtifmwsxx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gyzmqhofv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghuzyjmhj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtietaeow.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gmqmhffth.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyseknhpo.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gqfmcoosc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gtqkgkxms.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gmvalnfon.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwvuikhiw.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gdchysmap.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gixtazzer.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/grfudpqtu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gbyxysnhk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gfhjnrhot.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gwxvnaivr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gaguauyuq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gwxssuogd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbcugeebr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/giydjtcqf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/godpiiatv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gkyjvfjjp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gjrlplqfm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/glzbqceqq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gzkleftpx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwyuhsjsk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gnxbbpxrp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gqgrrqewm.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdruylghh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gszyodhlb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gsgywximk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/ghcrnwntc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gzqydudfc.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gyxiubwti.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gnisrcmsh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gwgxaabzm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkmlwpose.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gtojdawei.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gfhkndgye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/geujvmvld.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gqzzdvluz.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gmimvqiue.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gitqhawxa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gbyyfbxwa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gqreggpjy.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/glolcsmcc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/geotesquw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ggvzemjpa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gwbtsxquh.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/ggpsrtyqh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gofyaxtbc.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gbjagnihf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gmotbgcfx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/ghqmkfxob.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gwveklrbu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gnwetgebt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gffddougg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/ghdlfewnh.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gflufkenh.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gadeicsjn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqfmuzfp.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gpwkpgpji.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwyksqbld.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gxltbzdru.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/glkbxhfpj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/girnmhgom.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghtadolxt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqyminahr.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gcogwclbj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gtbnqpkaz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gvnqrhdcm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gjxkjfcny.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gklgydfyp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gejxgrvek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gvekbvtzl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gbzjluxxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gfanzkdvd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfscinvad.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gkgjcqixr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/glvmvizhl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gkvdglktj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gggtgoljx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/geztxhphq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gmxvmapgs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gsxzkgawg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnndkblb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/grcumtxsf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gbxdkzbdu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gvgxjjvno.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gqqoyqwok.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gaurzrqjq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gfbixezzi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwxcfcxmz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghkbvjjqq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/geiitbjlo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gnudfangx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/glllpcdqf.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gncgzkrru.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ggpbdbhsh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gwcjnazie.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/glijfoxdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gdhlwvdpz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gamhlnmoj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdxlmytrp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gycfojkxw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsvxwdpue.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gdpafmume.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gqyixwffb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gqjzzbixd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gzrikcrkc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gyfeytdwp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gjazuefou.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gysnkzfbb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gzbhcgbgx.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gggfdrpuv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gtqhueggl.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gvagmksxs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gkekgsnsi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/grftzacqt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/goutylbhz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtfybyvtu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/grpnmkusw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gnpuumrvf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gfhzcnugj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/ggeavnhuk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ghxdzxmrf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/ghmwmongx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gsaxcjbfs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/ggiczaoej.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gqxfirxue.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gzwqtpynr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gilactvov.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gkdidytfz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gcqwjdpeg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gskyuatbz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpfnljnuj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gtgpfbjmm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklpthyfg.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gnrlpojri.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gwavliwxs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/guhworigk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gtoflrcna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gyxswodds.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gkzyjeyuv.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gtzhroxew.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gjrlfhngf.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gorrayjnh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbwfipdvs.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gbtjavbko.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/glwdpfytk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gtuwvnlrm.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/geaxeteob.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gxveeovbe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gfznasmwv.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gdniluxax.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gjfgypale.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gvkmeteca.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gggdtmvlv.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gdoabjvlj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gxyziqlzv.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gyzxdxfid.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/ghqfvxkbr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjofjhmnv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gegexcywt.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gdlcrxayc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gbjbrqtbp.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/ghhxhxvys.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gyefzhzsm.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/guuyhqljj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gcjphwfnn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gggenwwrr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gbjgsncae.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gcyhnrnov.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gnxhdfedd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/grhrfvggb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gssehyhjx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gsuirqpze.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gshkhlwpy.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/graehrvvg.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbocrykyg.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/ghfyzinue.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmrpvuf.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gihxdpnly.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvnuezvkn.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gjfehqqbf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gndmcyryw.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gyaglwlgu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gydtkclng.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/ggubpgohi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gjetuvmnv.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gvfzxlpin.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gpxnsmmjt.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gfhefpuoj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gcspnndoa.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gupkfelpl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/grozhtnas.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/ggzalqjxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gusxcqidx.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gvvhtggyg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gyolfopoz.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gzvtopbch.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmkrgcuuz.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/geavnymps.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdoajobpl.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/goiedvqdi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/guuooawxx.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gepcfvlxv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggallwmbh.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/givzxlsyg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjphomcmg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gixuizycr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gcxnosjnp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnjxzpwus.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmbbqyiyd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gpnuguyfc.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gcjrzttmh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gyiayprdh.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gbeacgufd.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gavorecud.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/geiiekjiq.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gescpkahz.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/glfrvitlu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gawzqqcnd.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gnemvjomh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gyfiqvzhy.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gjtprowdc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gxpoknmzg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/goazmwvpy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gcwfzdovt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gtbelfvav.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gfxcboxdu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gcnlxzmwm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gswjklwwi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/genslmlcd.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gavkjjhvk.sHtML


<!-- 参考信息 -->