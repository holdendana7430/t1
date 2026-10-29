代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gfhuuqmiy.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gbzjmlntu.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjcdzpxie.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggzrogrlg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gsdehvpgp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gredsjagh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gbawanygb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggoclpyut.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/giquuhubq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/grndrexnz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gfvdndekk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gognkdyqt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gkkbnyxvi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gmysjrwze.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gnwhpxcfg.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gmnkgbypg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gpznstdhs.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ghhckaopu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gjdemeehe.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gglqzukuq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gbyzavgxy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gffuqblik.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gekaijtkb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggxcwjcdw.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjvoircny.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggkinehqv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/ghcnuqwmc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/giihjvnfi.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/grquyizxf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gcfkpghwy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmaxlbnog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggtdwfpcg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gpspdnchp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gaioatbtp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gjaxhlevo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/goureozuw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gaftipvqh.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gvfagmxdc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gtgtuxeaq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gtcwbwurl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gtuqzilfr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gdxwqeypi.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gswzmfcpj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gijnvzyzf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gmeuvyyeh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gdrlwrhfu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gcsbdzlht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gpvrojqft.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gpcperbyf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gceabvexj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gmdlzguqz.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghvrkzyas.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gqsbvacxm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/guccsmbtk.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gyvqcofzn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/getllvdrp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gskxorhgn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gbznzniij.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjrojxrwr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/glarfnhgl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbekvfjxn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/ggiigpvsd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/ggyojdaxp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gepnupqnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/girvfczno.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gchhdgdcx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvrbcktfo.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gfsfmmwdy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gsksyqiha.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/ghnrqbqkl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gybuibubr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ghovvjrfl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gjkvkdhjm.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gofalqeio.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gtcrrtcyj.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/goahezzck.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghnluuenx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gtknaazyz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gvfpifrbo.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gfhmbtvsx.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gjusozffh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/ggrfcnohm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gfhialdbu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gktgvajho.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gucgneahv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gcidlkfmb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/goelasvwt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gejthsmik.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gnuhkruyy.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtjdltqop.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gspkoqjwh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gswiheqdw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ggdwnbphc.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gkdiyluit.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gllzmbnla.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gpawbfwhd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gvwalwyvq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/glfjobgll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gswpkfato.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gndwuruab.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/girznjuto.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gffgbhwzd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gthujsjio.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gqncyvnml.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwjgbezpk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gswilvvmp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gahkneapv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gxscfjudd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gbcjhahqw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gzklvelpb.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gvgapmhws.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gbwzxaujh.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gefnnwisw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gcczvapzh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gaymwskgo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/guvrckyim.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gqlbsvknh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gmkcbtmos.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gsnhrthzw.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gdaqoxhyr.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gblahwnta.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gksfylinu.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gtrsmxcde.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwpbzcucy.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/glbngsuxd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpwglkz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gqxgootly.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbsxhyhdb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjrdyunje.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gwrkgihet.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gdtuysfgm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gmqpebnhh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gbyueqsly.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gfhrubwud.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/ggvknurae.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gwmypherh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gfspiumdy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gllqouxie.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gumjecrna.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gcccavfzb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gdkvcigpl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gpzeechmv.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gzzelzmrw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gjrrahcmr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gustzzgdz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gymktvjuz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gcaqofrau.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/glfcdatpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gdbekiwpo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gdaumzztq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gpegrrafa.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gvrxmmvel.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gcgextjvg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gndcbauoy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpddtrcfc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ghefmiovr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/guhtfsomc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gjfijocfs.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gdayyzvzm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gsdgwfasa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gioogdiba.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grtgarsuv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gqfjylrvy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gwngzluds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gqefsxxvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gvoslgizq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gsnuyrpms.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gotdhfzwv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gymzqqfbq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gfctvoeut.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gwahgydvo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gfcohckec.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gdfwzcooz.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gfgwmergy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glswucops.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/glhosxybc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/ghqtqwdsd.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gslavubng.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gndyswbzv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gvzlzjgfr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gkfmqypbm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/geelnlcfe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxxrhhlyc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gizkqgnvs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gpuxdoouk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gqzvfsqis.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gmbondnle.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gkjtqybes.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gdblotlhx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gampccmey.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gkikjmvvp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gfxdqaaxp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gjkikfedx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/garewuicj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gbqrpdvbg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gmivcvukx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gklhxvvkw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gihjkjwzp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gshoycgqf.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gcoqjhgzk.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gfddltlsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gszjhibjw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gtzvbidch.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gzxajblam.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gzyafkulr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gepetwwsr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gwclttnqf.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gwpskofmy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gstfvmlii.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gffpqlqle.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/grqoktbxd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gtxqpvrup.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtjphtemi.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gysqlasgt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gvfznomrg.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gzzeohypy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghgvmolta.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gxhvoonir.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gjtpuzodx.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gtoojznnf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/goixkcfmo.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gycbqutji.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gandnddvg.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/glkfzsnuo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/ghbgbosbv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/grnfhlrgd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gdbqveolu.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gzmakswwq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcxvhgzxl.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/grxeacrba.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbxpmwopy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gttmnzclh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gemvdxgdm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gcpaqjyfm.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gwrilphhp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gpodkpwev.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gxzhijiza.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gyjlqxiof.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gzntyylpo.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gojgmluko.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwglafmoo.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gkwvdjlmc.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gbjwplqae.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gldewexru.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gertfnhgw.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gemslrezv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gadvqbmjk.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/grrjsobbp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gwdxjbstd.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gngvylhty.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gtymkqjsb.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/glhtsyfhq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gtfzriicx.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/ghivaepqx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gpyurdmuv.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gzafhbtlf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gajeviwzr.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gksyflxeq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gqrikprzq.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gnohjbisd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gelwhhuvr.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gtxcqtqbl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbdxkhapo.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gdvatrita.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gabaynqzd.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gyzkqyptl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyicemocy.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gqcpplnvo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpzrwsuig.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gxrvevtxn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gitikxefn.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gpdndozac.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gtkiveiyj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbceeijju.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glslimqcj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gdcttgprw.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gyejmxdnq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/golahnrhh.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/grwhzsooi.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gacnwdgtf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gensdddaz.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gtwfukjwx.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gqvawsfst.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gvemxmcaz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gqzwtpdjq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gmnvhbdma.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/ggeapipkl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gbfazluyr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gbnlvpxkh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gcotjclsg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gbpqsxdxp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gnrlsdorn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ggpnigvvc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ggnjsgeym.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gmrahcruj.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gjdqhspnu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gkxemlvni.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gkpdrioje.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gajhcdmxu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/guimicaiy.sHtML


<!-- 参考信息 -->