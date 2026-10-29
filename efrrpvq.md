代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ggtystzuu.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gdqwvitzh.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gqgharcdu.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gngjacszj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxsymykgl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/glzwuzuau.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gtijuwidt.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gbzciifng.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gqfkolean.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gclewsqar.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gyrmgkavo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gxjiqtldw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/geaoevzli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/glgxcywwq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gqwzcdbyj.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gxoyilsud.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gzuppxmqr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/ghsjzdzvp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gqabnmscl.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gvhrxwzpf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdvhflqit.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gxgxreizj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghteyiast.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/goobeaegy.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gywhuwcym.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gmcwzsusd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glbcpsxuo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gskxmqsec.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gvenhgzjw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gurjdakui.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gninhomgt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghsbndxlv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gwqwnbtrb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gscvsvxis.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gscxllkjo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcyljgpkh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gdqpjvhmy.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/guzgvrmxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gjymmgjic.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gnlwbnpep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gbxkdbtip.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gbmhcisye.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gnfrwtoio.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gqkkedafy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gsmbtcpot.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gvhcmkhvg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gxsrezese.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gbeesaqft.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gjhxouvis.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gpxornhno.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gfeftjhcn.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqbgiyehw.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/goapmhbbj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gbgpnkfby.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/glzbgtzew.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/grdideuwj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gzimppquq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gcumfnnqj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/golirsetm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gxmmgavwa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/grwduduja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gmvjninph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gwaoxfgjx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gctqsrrkv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmihwijir.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gxvirqunw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glkokdrdc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gebnopkpu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gpxcqqzgy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/ggtwkzgng.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gcicclfjr.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gdhqvgmsa.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gqixevxly.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gqpwaigcw.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gxkeroxzh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gxrgjbhnl.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmslzqyoh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gybnesafn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gokoptelo.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gvprtwxal.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwckqbakr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/glgquyvfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/geutsqtem.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gfqvulzqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gptkjsnqh.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gvimfrzsm.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gbiqqyrve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gbbihbdjz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gtpboxgrx.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gddosizjx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gabkntxcm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gtqwdbvup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gsvonlfrb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwbedohem.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ghlqrovsw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gvqwrfpec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gfbiuulbq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gzmjrntjg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gamfcshas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gtodjrzva.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gfxskjcyc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gonsvtadp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/grexhygvx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gcgmbiyka.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gsuhedeeq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gyaehokvl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcgjpnjzb.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxoilplnw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gecezmmjl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gozksjxje.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gfhlbpfab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/grkubjkxg.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gnksqjbcu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gmiiisgoz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gfkfadhzj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gzndugvdy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghspmtoyb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gtkpswidd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gpiljpymy.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gdmdllqve.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/ghrijrnbh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpfbvhigk.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gobeikeio.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grfpaascc.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gyfjwqzsy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/glqgblxak.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gqjybulut.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gkjjwpxye.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gylyoufvw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gupcedgdz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gfqtxmlcn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gdfgqpshv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gakinsejr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gzrzaiflf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/ggoprluzx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/ggnjissgc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gizwsuyqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gsxjlaeqs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gocmhrcum.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gmsaheqmq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gmqsyvjfs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gtdyyjbak.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gyphoeguu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gwebckuhv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/geltugrdt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcgkyzhfm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfvaahrlv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gjkjyrhjt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gvfcncotw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gtjgxjpes.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gmpmwdato.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gszrqexqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gbqzalotz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gprlmgabq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gctsyilnj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gmgfhdyao.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpbixiugp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gszrbpdlb.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gdjowiejz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gcowkzyhf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gaujxmeub.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gvvewiplf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gmbgthdbu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gbwdwnpqe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/ggkkieuaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/ggtrocztr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gsxdvscap.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gysispgkm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gbwikqukk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gffjdfjfd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gkeymlqor.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzyxfccal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ghoofublg.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gzekoowhi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gwomdelcr.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdaoscua.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gdkgomimr.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gbtqqakwp.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gtjmubjgw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/grtqoudej.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/glassdyyv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gsvjnpycb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/guzuoldgu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gquxsnjse.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gbeggzhzm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gjianxciv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gmkexddvr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gfsgppkab.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gdnnpsrrk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkdsvweal.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gvqwnixqh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gzrjebqta.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gnmyzogwy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gtqzqxeed.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gdzpclcwc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/ginguiuli.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvqkghwzg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gfwifhbxv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtcrxqtlb.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gevntptgk.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gpninjgnx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gsykcdkmw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gvpzmrlvy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/govanzdmd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gjvxgkjpt.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gizohrhoc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/glstxoyjf.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gasnrnrhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbzqawgda.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gpjlqykkk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/goqjibimm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ggnfvqxos.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gjaolnmfc.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gzihqprmg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gpnjeqioi.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gtlugqtgt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gftgdtkaq.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gogtzkvnu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gpewjqvdt.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gztgnjtst.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gnmpqwoyf.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gzttgszsu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gjbwsjdul.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gzmebdqdz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gexknbrnd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/glhflhpwd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsiscwvyw.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gdrwevjgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdiwfcxaw.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gtgpsxwta.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gfsizdayy.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gejrijcco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/grblcuzqu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gntdihksn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gjxoiviai.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gakkhyhzz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gyqelwbbh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gyfigzxwl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsmheqrk.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gzjvjiysf.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzlhwnbcs.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtgtfoeci.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gmpusruzs.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gwkycpkyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gfeozvjrx.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/grdljqssh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gqskxnueo.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gzwqrgfxv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gmxjichyg.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/guatvyyow.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/grgvdehjw.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gzxbjtevm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gwpabhlgk.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gxwofaago.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gdjjukwzl.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gyqogomik.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gftowmmzp.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gyentzlvx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmhuyxork.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gtrpoqtbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gswnwgdjc.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gddmgpkqg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gejilifef.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gupnafpgh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grzvvmzcx.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gwxtrabeq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtugjxwov.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gtelaseaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnhdmzjvl.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gwtegadpf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gdhyjojit.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gmehhvlbn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/girsxofjg.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gopocehhl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdutvjckm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gsruvjvcm.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gjxeetqyw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gkkydvylz.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gmklavlxd.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gxfkmvbis.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/ghyuhmsmf.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/ghvnatzra.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gawhstnfo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gnpcjceka.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gtnhvebnw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gxhvyqmac.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gydahiagy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/guzmiuymn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gzxyizzhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gwcrxhsgt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gjmxvdngs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gkcwofzsz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gkbvvgndo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/guzyigvjz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gdghixqam.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gppitouet.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/glaowxchm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/grgjhzare.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gvcdrcyyt.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gkpwtczzw.sHtML


<!-- 参考信息 -->