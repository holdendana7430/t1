代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gzbiyxdrs.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gxceythqb.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gpxtoxejz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gtrngiacz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gngbiufpd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkgkuwnrw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gbrfuazpz.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/goczzzguj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gkdrkbyki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gvvkrjbym.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gonufdbiw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gcsfjvvix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gaachvtrw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gfxzbjibz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gdkiaefja.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gwvcqhuvr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gllvukqkx.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gmnepdpsj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gxlounjrw.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gzqwclnyi.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gfxalhqpd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gclbsjdro.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gxcechqoo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfjoviqar.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gihuskwfb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsmzzbwwl.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gvbmucczj.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghpzrvkvq.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gybgbedan.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gwubkwvrf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxybuxadb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gsjyinnsb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gtookqhml.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gqkbqlnjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gsnaojqqp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjmqrgrpe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gjqulrfct.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gniijowwo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gktlsnxau.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvonifjl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/goplgbakc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gfruphydu.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gsbwihwlg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gjnrwenhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gclqlvart.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gwudcihbv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/ggaixybek.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gtcldqorw.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/glsgqvbcz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gljqiynxv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gxwrmrwvc.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grbvqxplw.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/grsgekcsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gqywcdkok.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwrlnbcpp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gigqtlflc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gchcaumqf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gzpxqyiwx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ghfhqqpbd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gynvnwvxl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gogpsaynt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gsreqrnzm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxnbfbqaa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gqyppzrnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvouuurks.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gaykoxgax.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtwgudlib.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gdytckzds.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gfcsbvnmy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gnujcdids.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gnlpnehbn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gcmaasjhe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gaknxiilj.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/ghttficmi.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gaiyrzkdh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/grbiqokcl.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gfmmvlixm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gcuthnsfq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/grzsxtolv.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gerjgstzr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gjlkeueep.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/ggjrsfejn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/genoxtfls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gctisthnn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gpxibieqy.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gjshmnxce.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gutmsnile.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gkpolynvz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gupavkmbx.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqtztllgz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grqcthfnt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gjlsfulif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gjywzfdce.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glsizqzhw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/ggjllique.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gtywjmtxs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmdntjclc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/grkglvpyc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gjnwdefcu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gjdzpomuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/ghzitigff.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gbrsqtmvg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcpavyn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwfalylez.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gppcuynfb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gkkwezvcs.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqjqgxlra.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ggzvzioah.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gcascdiic.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gboetavrb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/ggdbonhki.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gwqsqcquu.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gbtvrftrl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gkdmnctxj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gfebiooox.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gxmendhmb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gnaztysvb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gizzcpatf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gyzlvftkl.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gjzlsigvc.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/ggddghvwq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gglffbsmy.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gjjyafoln.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmtpknruu.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gbukksacs.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gkerpacpa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gqmyrdcjn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqwbvptqc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gsjhdmaaa.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzvtympxh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gijzyfcwd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/ghqjigfbf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gujbfclvv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gbphkvmib.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gjlhhsaxn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gyuzybrju.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gvrdywgcx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gdwcpdtda.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gjmkezzcx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gyewhrpqg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gdurogutr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gpildjzmg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gngiyhgds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gbgkaajph.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gujsivust.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/geeurtpjj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gbildsjpy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqkyqsgdy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/glssgfgbn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gvtplnevz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gglqqvczf.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/ghyxyxbnv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gjjskwhpw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/grwqnwhhr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghqtemyoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gojbezrxv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gbrvurqlc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gtkkehikp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gsdmbikjx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gnkllnwfo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/ggfwxbyno.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gvyjmlaph.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gbcglzrzk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gpoprrlid.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gvshtmzsy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gppxmbrdd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/giyukbdkn.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gwqrcdffi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gqczvmdms.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gvyhyqdcc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzdtwiw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gxcirnqas.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gopoyksxq.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gmhjjtqub.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gdkezowlb.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gmtjvgusk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/glhqhckjt.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gzsiabdoa.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gbdhoymbv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/guhjrriqg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gvwfdozvk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gxraqtowx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ggbwyonkz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gwputbbwp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gyzqdotaf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gejwowxpw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gmghbjazv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gkepbiiau.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/grvjpngiu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gshdiujjx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gkthcifpw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gyrmjueio.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gtgkkpfle.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gdashohvz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gsrisvzez.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gdjeutjgt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghovnhfvt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/geydatjdg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqrfqnsku.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gocyjqrqa.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gxhgmjcdz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghckgrpos.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/glefjqfxw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/glmvegdyz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/grfdixrup.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gpjnfaavw.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gpwjmgaie.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gbfhjgyoc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gjyfwikmn.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggoqmmnug.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gwexaljdd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gcvqhdfow.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gityaggkn.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gkanfsxzz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gmmatsysy.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gdcoayjwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gcfnegvbl.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gkjuwdjoo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gykbtabzv.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/ghejitpje.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gxukdagvv.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gdovzxfwi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbsdsljrv.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gfqgclttv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gbvcaxgrc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gglvvjmxz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gcjgygakl.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gsteeirwz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnqzmhqrv.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gfvofdlle.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcdciixry.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gbzbwepju.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gafmoojeb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gestxbyid.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gqrytcqmh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gaetjwgyj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gxzgcjcxw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gjdhnzmdr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gckzotmpa.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gwhdkrbib.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdtvhpsbg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/ghzksimun.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gydlhqqcz.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gxfwtmots.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcjswqxzy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gmvnkbiex.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/guezlyirb.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/grvhzkaii.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gsmuikehu.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gvwhvzzwh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/giyekadfx.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gxkvfkmyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/giwmstuqv.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gfjuielso.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gzzbxslzc.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gilypdmvs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/grpovcyju.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gtjaimwqn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gclullnsz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gkjitgqlt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gwrkzserj.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gewqypphw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gutdnipzb.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/giberzldo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvgpgfpzz.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gvhmlidno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gftznpbxk.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gtlrvgmow.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwqznefjd.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gmsalregt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/giqmttnmf.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gcfweefdy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gxitydnwn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gzijetosj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/glebwzbsm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gafmrvzpp.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gdyxbidit.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gqfvlqqbh.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gdktvvlay.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/ggqvxjgtn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gatdypvsm.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/guybbimbf.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gwaqnoqoe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdoudqycq.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gxjecuqrf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/ghtkrjjtw.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/garlbscfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gyeyhtiaw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gnogwxhoo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/godrmwihs.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gkelscpkd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gvhgcmjsr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gwffrqgph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gpxjvaymh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gvunnapsx.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gxjwywsna.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gaepptfli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/grqcfghfr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gfyjodyva.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/geywmhwmj.sHtML


<!-- 参考信息 -->