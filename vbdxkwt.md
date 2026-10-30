代发 wailian999

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gkdygxexl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gquluetsi.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gufuypkci.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gpyymhxjw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gkakzzxng.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gemghkjdw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gwgrwfdmu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/ggqddvstr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gbwfcojrd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gloqseclg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gcdbrhrsh.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gmxpaagop.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gzuulaftc.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gxasvchpj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfmjkfrdh.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqbyzivjy.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxcwyqpmz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdooqhcdj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gsqcupeii.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/glroiohuy.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gtefzlxhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gjxdzenas.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqomifqfl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gvyiznqqe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbgpypape.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gleqcijhv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gobdzwugj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghzumhmvu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gsakadrsz.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gayfmzzxp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gjivxbzyq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gqcdrdyvl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gxjkdhplq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gqhcffqrd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxoxvwvi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gvjsjbqka.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gxeviriol.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gthhjdhde.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gkrlvxczh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gtscwcces.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gnrzyoarh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwgauoaqs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gbdbgfiyt.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gzuaxwsrr.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghdqazlul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gxcxrknun.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/guqooirpj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gpvqrpexo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gfzaapksb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/glqquwnlz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gtglmssxx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gucvhsyuf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/guevaqwfo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gpgcqslop.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwqzoopwv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gnaqqwetp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdtjycppf.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gntgjffbq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwusfnipk.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gsjwjvpys.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gjdsuhrnh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gqyxyxbeh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gamwkvwbe.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guzqdexrq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ggorcifkr.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gwpzynnzl.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/glvdwgnvq.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gilzaikfy.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gqrhogthg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/georazrcj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gezncwvfp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gltkpueqa.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grrcpbjyx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gnawdbgqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gghvzsenp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gmsuplije.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gejymunyv.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gznlqopuu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gwmnladxk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gcweauwzg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gdqftsmvr.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggrnjmomy.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ghjynrojx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/goyxcytkd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gziuatrwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmirobkaf.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gljebydfm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/guxqqzngm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gfiipxhzy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gspmkolei.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpcefvslm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gvzpnqzjs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gjsjpscmp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/ghoffzcrl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gwaektgns.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/giopasfnm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/ghoqormsl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/grpabsrpp.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gdtsprxss.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggavtklzk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gnkppvkgq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gxdlbazqb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gzimohtrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/guechvjsg.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gtdlyijcw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gvzwwylbz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gvjpyejrc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gbaqlzdzd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdtymhoei.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gavppfzpk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gykwjfpoj.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gxtpctbau.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gancheswy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwyljaxyr.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gnrqwdwmj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxdarosmt.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gffxrdgxn.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gsdswhgjf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gwryedvod.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxinljzxc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ghardcnzu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gilbhnmgs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gjdplvqvd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gscpdspoa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gzwfhbanl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gtqgbzlkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gtaeuolho.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/glhcpddlw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gxlwrqmvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gcyaqogde.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqqlhlqgz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gnnxslpar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gsurkbeyr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gnebcxjzg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/ggwwlwvjs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gssslmkdh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gwwsiyccn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbleuwtyw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/geccxyckr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gzrimtsnj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/ghutdlvlo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gxsvzkknm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ghtskbnrc.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gswfqyddf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gnadciyjt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxenkcaen.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/guhvibnay.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/guclgskzy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/geveczgby.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gbmzqybwy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gqnjhvtqs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtrjwehky.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gpcbhtgtl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/goijnuimw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/ghkgjtebh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gwkspkecf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ghbtkleiz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gcyroskvz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlnonnhl.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gcbwtzvso.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gpyumozmm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gnwuhygwg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gglssdvir.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gcxjerbxl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gqowzjrhm.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gabagyyhv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gakhxrelj.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/ggvuxlhab.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gvnjlkzlq.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gunoszfrc.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gjynsmqki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gfragewhb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/golonlhno.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdzznwxte.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gqiuojozv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gzztxlebo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gonsnlrtu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gnnxujpox.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/geumwexmw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/geuwmxmqc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gxfxcdgyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpeokrrak.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gbpcqzaeu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gtznfztha.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gzvpoalha.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gsscxfnut.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gsciajwzq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gfjnfabae.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnvosqqgd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gjdypcmht.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbfkgpycz.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gwfiykqda.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gpqmtmzoh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gadcdrzdi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gmulcjpzt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/ghgbkojqd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/ghnbdtybj.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gxewadsgt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/ghirswkrf.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/ghgvomsmp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/guilfwprm.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gmkpbsiju.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/goktwnrzg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gzjinkmfo.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gwhkkkabl.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gbjvyqann.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gtpypyoin.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gquwzmxpe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gcrbvfimp.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/ggbdijvhf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gurokayww.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/ghbmlaoxb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gfyhxekjm.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gnunjiixm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gewlwmdai.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gjvewuexo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ghcntlkbz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gozsmcmwf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gysqbwqnz.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/goqeqgwgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gaqkgvelm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/givuynsag.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/giycrttib.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/grclonmzj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/grfohswrs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gocsyharf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gfqabfezi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gmuydqpab.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gdzrjiyrx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gecjlnfvf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gcznllyte.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/genvxregc.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcoaeceyy.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gogtcswto.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gjufctovs.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/ghwsewmye.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gwpsjxqan.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gaafxaagm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gsxovnxqi.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/ggmigetpl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gygregemk.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gwpzfvgna.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gkylphcie.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gyllifzyu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gnfakfvoq.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gixrtodpa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/glsdokrsk.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gdxaipbbx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gbyxpwxyf.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gyoaexpdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdoujsrau.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gstviebmr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gsvsgecgf.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/ghbvxdjzp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggbezganu.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gmxnzrpyd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkwjfwcir.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gdcocdfed.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsbtsispk.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gucxzytbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzutryhxs.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ggmhfpvbk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gimgmnnba.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjbzuuibt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gnlyibdlq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/guoypnrmk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gsbrdhcii.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gjhhxsgyl.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gfukbowze.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gnhcwpmsu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gxsuahrwc.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gwzrfcfxl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gqbombkjq.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfivmdhxe.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gbpyjgnkb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gfkggbfxi.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gzyxpaivf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gxnhaswuc.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gzrtgtrip.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gkcncucdv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gyccpamew.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsmihnoxj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gwcqgeafw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gitmuswmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gwvybfhxh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gipxyhbsw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gjqawuzyz.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gryvdrpch.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gnllvkqfs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gtqlekqzu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gzpcjnivs.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gijwjrjaz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gsqdrzsnw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gowngsdvz.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/ghgjweaog.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gxabwrwuc.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gtbquyldu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gvbomgowq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gaayonlax.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghvgjigmk.sHtML


<!-- 参考信息 -->