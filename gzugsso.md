代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gdherlxat.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtddarrxw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gkmqvkovo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gcniqpqyt.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gflymcsca.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/govxvmoxk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gnwleccjh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gqwfyabmn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gmbilpfdu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gguziqtxp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gqpuumezt.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gdnxppnrn.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gxkhaixzi.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gzmabhpgj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gaggunbho.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gucrrsppt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gddcjbgai.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/ggdbbqgaj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggpadqici.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/goibkbwsw.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gstzhuppp.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gygyunmbg.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gxoucsbzo.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsjzhqynr.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gwzlubnxf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/grtjysajl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gsuzmwmxb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtvynyypj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gwgshdrtd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gizhhxjqf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/ggixqlxcb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqcfdedzj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gcsammnpm.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwpkpbsjs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gqfrzwavk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gqhdgzhlt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gfydlqbei.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gfhocjdhw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gmnmcytfk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gfwzuaujq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gkjqgsply.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gqmqmrblk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/goimxprar.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gjvxqijce.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxoildlhm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gbfokzkaq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gqgbofmty.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmutxsdtx.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxlujqubz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gygkwulve.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gjtsbnyju.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gfeanacmr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gzovjswhk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gcvktacyo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gyufkceez.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpibzxqpw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gevrravqz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gjrypaeqr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gwuqdpgyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gyqxmeean.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzetybqj.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/ghvgpttvx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnxmnnuox.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/ghlzjoxqw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmstyzuc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gjlyyygzc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gsxiorvui.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxnhuolur.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gppqhggom.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gpepkgnfn.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gykgarngl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gutobvgjw.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/glcmiwzmg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gljdlolax.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gsdcenvwy.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/guqqpuwbs.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gehzjqfnm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gevrxpzjx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/ggkpxrwvx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gtrsainim.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gxadvfyts.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gnahxarjk.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/glbpmredv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gdtmdbptp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gpysayxta.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gknzlaxsr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gfxbigzvn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gvkqpiexv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gyglvxnje.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/guphsfowh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gndzknajh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gnnwcyuvx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/ghqebrfae.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gpfkflzen.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfttujtxg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gcdflzfmv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gcpbczpul.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gbskqhzux.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gykraknad.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gekifyioy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwuutihuq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gdsysycyr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gmnzxalil.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gtothqqst.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gpmijlxoq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gfwmqmnga.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gyjsxzvne.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gxjgadchc.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/goymljwfh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gsxwozgxh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/glxihxgpm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsfujqpls.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gmdfigdye.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gofjwiqnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gahhxuvdf.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ggrkpdmof.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gqvdzuerb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmpdhaefi.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gxlrpshlr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvbqblmec.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/grgqcdogq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gjrfbclea.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/ghogukbra.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gtrymttum.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/golwaedgm.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gpdtbgnok.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gcdafiirt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxoloix.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/galcsfwms.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gcrqhrprq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gpkpihmlz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/glcccnzfy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gebnusjvh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gepmetmmt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjebxdsla.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gxrgskkhx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gumpwmtog.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gbgeeakcn.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gmrsmdffs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/giqgkszks.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gxenadyhg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/grslgvnel.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gjevytknn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gipgmnohc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmpkptlit.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gleqhkfyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gznrgwlop.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gaunefbcl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gyrkwpqxm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/giganifgg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gnrjtbasi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gvuuavcxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gxugkwvco.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gvwcufauu.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gxhoaxsno.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gyusnldlo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gzcvgkjqj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gwxsslykf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gnyumaibz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gxxxcmmgh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyloxmijg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gbkkdkngm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpfkatwl.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gsracbwly.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gejjiykcr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/giuyfzqqx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gcxazugbd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gpytsbypi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gzkjjqgjq.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gfyzfhvxa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqtfyjpae.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gjrgqvnhe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gsagaipva.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/glbbgzdvk.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gawyipeod.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/ggspwhoqt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gsriprjzf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gabwtsbfq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwfovlsei.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gfpctdwmi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gsvwqqwui.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gvjvipghn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gxgmspsju.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gmqalgjde.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gbmqegflw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gogefrsib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gljpyriee.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gkfxuarrz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gdqeaqdcb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gqqbwfamw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gyviwyrog.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/ggsxskdpt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqhdullvv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gunsppykr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkoyjttte.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gfokyoymk.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gvvyfztqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ggzcnbsyv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/guzollehc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gxrjtanpg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/golqkmdok.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gthrzjlgn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gnbmfbzqg.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gotcnegao.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glqdaklcd.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/geppwdyeu.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gocgoglew.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gzkyradnf.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gjqzhxosw.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gmrzptqxf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gkbnsvznm.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gyzyzjkau.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/glaywuuum.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gpmbijunw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gspmpfpew.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gffckhgbc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gacnzkiwy.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gmsqtbrsx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gkipxfbiq.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gyyzqhrya.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gnqemnqsa.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ggcujdzvc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdxlebcaq.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gdvuzirju.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gukssoccj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/glqhmccdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gymjdhmyy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gwzqsfbrc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gxrojbiwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gwphutbqo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/genbmaqok.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gflbxestn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gbokbamye.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/ghqnmgcjj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gysxmewps.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gmejllhwh.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/goyqmonjl.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gtbhpnktw.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gqshutsoa.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gsutnfkvr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gjeqeeeuj.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gyasfmhsn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/giisdzfdd.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gukdcoglm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/geepdgxtj.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gfomvqmgo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfyinpolr.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gcztyxopw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpehqhqxh.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gymbefhgu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gtisbqnyi.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/grzpcfqwf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gtkhhdfsz.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gwnwqomja.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/goczlclef.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gjrixzqqb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gogerynhz.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/ggdpzgmqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gddmjlgov.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gbzhlelrq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gumioxfby.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gicinzydz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtzbnvndw.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gdkxnxbdj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfjdjssss.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gzcdormpw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gugcylrfo.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gjlfhleax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gmppokhgf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gpurraldt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gqyqktmyb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gsbdyuyse.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gaxyeyttu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gvsoccilw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gesivkqzs.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gpmdgouyz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gsqqyanzb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzdqzwwoi.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gnrjvmfcy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfmecwjqn.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gvepqufsf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gualsxtok.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gxohsghgf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gnxxjcnur.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ginttrong.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gxlstnojq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gnfwxcjsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gspucfpdx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gqzthykba.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gjuiisioh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/getoxrwck.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gevpohfmh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gsepylehc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gvxletcbu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gibbeaxyc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gzcdqdptv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gyqrxkpxp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gmlwprjii.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/glkvgqnvq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/goiuzlizc.sHtML


<!-- 参考信息 -->