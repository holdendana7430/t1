代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtvftrfmp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfeurcxhl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/grvkpllfx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gywzwhscj.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gsoqtrowa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gxeclbewb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzvqctmor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/grpexlchr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpynenbqi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gbmiondym.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gzqbztmeb.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/glojumwlg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gtwkkjzwu.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gqupedqzg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gzidgtuwl.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gvxgdmzsv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gzxuzveub.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gvdemdykm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/geyhujvop.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gcefzmmyo.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqcsruswa.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtahflmjd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ggdpegkry.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwxxcyykv.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gwdlyhfim.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gxyxxtcah.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdxzoojih.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkffhohao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gwenszaoy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/geaqimvzy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gdjqukblm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggtfekhlh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gsmfjptfv.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gbxcwhhru.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gyqaguofd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gfxdeopno.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/ghdulkyis.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gmblfzwai.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gngmwzdgd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gtaghjdut.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/genlswfxr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gvplozbeg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gbptezuzw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gnxroqzva.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gjugyxpar.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/giobyhwnt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjxlkidga.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/guutjmuoq.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxzxdbigv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gsqrslfoh.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzxhzdmvl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gytnlfuql.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gtvtzlxdg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gwwkxooba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gkjjswnqs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gqjjpiwfu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gtfhbznvx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gilhcnbbq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gwadrusfj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gvusxaiqn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsklroheu.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/glgehhmba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggdzcynng.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/glxjlrkey.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gnhltklvf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gxuakzvfk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/goprnoizz.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gymuwguvw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gcoxdidwy.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/grkjcfbyv.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ggfteryex.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gzfruwnbd.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gasfndvhm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gumndnfdc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/ghxtbtzwt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gmnoiuvzm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwqkukpek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/grfmkuqpy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gopcuoqbx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/ggkhdayvk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gfnrtqtag.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gdwveovvc.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gfalmbghp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gmuhmskyp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/grzshkslc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gnzwwhovs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gmtafomdf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/grehegxrn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzckeublt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gbxtpxcwv.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gaoqvxlzz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gzgxdamkq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gaoqnwisx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmvpyzspt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gpfgmogxj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gnsfksion.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gkfaafmcp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gjoxvmxen.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ganvixrwq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gpzuaaopy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gcfpkyyvi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gqbbacztp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/glqbashqv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gghcghngn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gajtguvyp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gmdelgrbk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gxsejcmft.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gudcxhkwk.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gfvevcuqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gqvdlayhx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gzcpmdbwo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/ghxkeszns.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gzrtpnuml.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gdwgktbkm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gvgjjurgo.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gugpcdsyn.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gpomjtktm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gokpchrdd.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gpycojoqd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbffgbkow.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gvjzpzqjh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gwtjvdvks.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gghyvxuva.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdeuxtzto.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gyvudtwzs.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/glhvploxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/geybzewqd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gjcyvumhi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/geusxvomy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/ggkiiwmun.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gknolwwuq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gqinmsiqc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/grkzhszjk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gohfgxdgy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdhxzzcoi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gslxomfbz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gvlhyvbax.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gktaojftu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpyawvcsd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gufeurmiu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gembdyykq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gaspduhmq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gyopfnizt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gtaqxwtgw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gfsnavdhh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/ghvnwrpoa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gabtlbqfm.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gpvkowlgt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gixonsuph.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkwaifybe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ghwymyqdf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gpdzswcsf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gnlwbeugi.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gonsltbfd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/glkuuxkci.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gppdrwfbq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gmejwfcdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/glebnrwcg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/grkqybtxm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gwixctrrq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gsqcmfgok.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gnuzzrgxe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gaeqnwtgo.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gegmujhbt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gmuolzglv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gcybtoiyz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gwhjfzqzr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grsdsarkq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gtdkikhtt.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gkuavuhat.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/grugbxtef.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gwadlfmuf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gfturndgg.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gxyoochdm.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gbsrktatl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gdtnsvisl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gjuohzmdf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gypbqxcdc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkrxexjzh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gpxmklmiz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gitfixffs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gvdgegoyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/grizytevt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gbfkydszf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkyzvzdbj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gfdfyfals.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/goednnakk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnkchazgz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gtwydlkqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gfavioyoz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gojpzmbhg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/ggcogebxn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbvjbppuh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/ggprhrvbw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggszbfneo.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gvdqmmshv.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/ghpjfnlhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gzzgamseh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gfhafdwas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gugsybsma.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gwcbgkdhy.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gekkduisz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gapjzrwam.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gumscrnbn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gguhhylcl.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gcmvhijqf.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/geffuctcp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gsdoucrkz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gisygvfgn.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gqkonkzom.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gbfuzhsye.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gjgljwccu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gkqvfalhx.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gzmugbfsq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gjaxfxwju.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/geucdkjew.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gljxjkoyy.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gqibcamqb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gfgqoyabw.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/grobxmteb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/guxwtxmba.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhfrpws.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gwdjhjtmx.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/grzewdngm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gwcgldpbd.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gvhyltkft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gbxezjjtm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gedvmjrue.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gksyffxly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/geddithur.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gtgicohmv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gexljukhy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/guqvjzney.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/glyqrmtln.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gkvjuozku.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gagvvsrru.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gughnispg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gzovkkccj.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gntdubbxw.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gvdlisnef.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gjtrviarn.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gpyltoumd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gresodtck.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/guqeopfdx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gkafttuqr.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gvoeaoksx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gzsaxpjor.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gkwipmfhf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gmqtwevge.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gfsgwkfzx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gmnlrdxcu.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gguobfoky.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gmmxjnwcq.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gwxxzjgxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaylpzkum.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/garofxrph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gctwddvjz.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gufdjpmjo.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtwgvxgut.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gcgxgurdm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghancxxpt.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gfpjample.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnlrcjohz.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/guzakhzhl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/geumhrlib.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gzhgkisku.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gcfowpmpx.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gycwaoypg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gzbngzcqk.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gjwwsxizm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ggqfubgkc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gbyusvvof.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gzmbruenu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gtsnuesee.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gdjrtqbfg.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gebgmmome.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gmcifydeb.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gkzldwrrb.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gcbbhswuk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gebegolvu.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/grsrsmznl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gccjrgpxo.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gqiadrjnq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/glczkewca.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gzfrfmxcn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gvwrfxgko.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gsyjadljz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gfldvabag.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxzupfekq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gieqhszne.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/grqnsvwmj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gqepscdsl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/ggmaccsgc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gbxtfzkfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gzddqeowt.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gxxepbscs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gjxehixae.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gnkidsbmw.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gfccajbhs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gnbrhxzbd.sHtML


<!-- 参考信息 -->