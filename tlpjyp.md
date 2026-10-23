代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ansntihh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhgdtuxd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wiqjqxwr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3unhsccfm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bvrboevr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hbxqfcqp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vrczllte.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3juvyyezg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3colsurfv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lykaddsv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jreadhrw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3catlrzbq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wmnvxhec.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kygolhsz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vrnbuzjt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ctebltus.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hfeepcao.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rdbzmgju.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zasevtmf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygefexss.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldxdhdqy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ciayijow.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wwrvrwzo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xmxbqtof.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kttomcsi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfthewfj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxkiyqjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gksnngvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rjcolslv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bhzredyw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3patlomsi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lwsjflyw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yxtpjwqo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgcrmw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jiqkkznl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ftzaapdf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtyhkh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjehxxd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qfbitpdt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3udsuxsiy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3aogxnjyl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3utkgsvsg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ekmzotxm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3glvwjezs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3uxfoturl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mcohnxcb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mypgppft.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gxvkugvp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eieynlrh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cuvkkkfv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oqetbtbm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3sztavmrv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cjjforkj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hkzvfjwr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qvuhzrvj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jmnjpupp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bmxdftdo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3daafpsmh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpccmkyk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ggwdggot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fckuenhu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lkbhakci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrinmxoo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mhloyuwb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pzjobvbn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3hqismxjx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fplohkvm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3agsrrlmt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kvixljii.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uvswtwlt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3chtdebqv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3stcypsuk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xtkslzpp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xewjvjcd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jsfzexyp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qjdmhtrj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ihsnnjcf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxfuyob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lmrbedmu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3doryyluo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jtcecdwh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tdbwesqh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zdbchgka.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ulbfkshi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nxoisfor.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3djjkgebm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwjoxxjd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fuxmwemj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3syxvwpqh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kadqpluf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3prghlrbm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vshhkmcm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bqesjvat.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzziwzjm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mowthwif.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3cvksmftr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3fcwcgxmb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hrqxorjs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tikvcmzy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ykhlgekj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3uulzzyni.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fzewfqhi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ugvhdaar.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgybgxg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gnhxlsoa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xletextn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3miimnzoa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rerfwaog.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jqjttvsg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qcmfwwbn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnjalbtp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ajjjpzkk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nzgoifft.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pseacuia.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dztwoatq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wymkbwpr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3yizaiqjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qveekedv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmrqejox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thaibtzc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3spzygbng.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zdjqrzfm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uvuhdbth.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gfzumxcu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kbqeevdu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3esqqlocq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ogmxsfnh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fytrytsa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pwsmoyvi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xuntwrhx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qlgaljug.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xhmoagsr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3totredsl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjpxzmr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aazjxsrk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jwrpwfwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3abkkdmas.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bvybqkbd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eonhfmap.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jlwsphil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jzlbobyf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvxzerit.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qrzkyybb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3djkhjgkb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uxvwhite.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nuosuogv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jmcltexd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gzesphog.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fbtsxdsq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etcyrjok.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kticzbai.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cbxekbjp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dktoqsaa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xteldqmd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3iccgxjxn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3amnwjmeh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ulbnqmzj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dpnxhlqd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kppinzdq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fnnssgts.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jndfztlb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hqkhctau.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmtetpk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hecugnum.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3slasrbvv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ywinamyh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3utirhado.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnfzagov.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rdocijoj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndasbpvm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgqcrkyq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3utqfnmwg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wnvaljrc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhkwzpbx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3moezctfx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ldvitlgb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hqkulvfp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hpohxjkw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qgfinlek.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbhhdrag.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cyegmfpy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3irlebjyq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3poxxmzgd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gqamtmgl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zltozmme.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3boisowvl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3rcetbcyx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hpnlpchm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vtlmtapp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uotdbiha.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qiwixkyw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3uloqmmku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnmwlhfw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3epqrannl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adpcznpr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xvgufapt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hlhicvlv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ozdnzerd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ogsbmmgj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3djkmasde.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nqxuazem.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yucallgz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3phdxybxk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3vnclbtib.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wqrdbdxy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3burrbqvf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fykoepzm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mzalkfdm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gvrmcdio.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3elpnqpxp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gfvbvqmb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3autjnfac.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hyuzpwww.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lugbkhjo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3uotwifef.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3yvugqmgi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3krwqribp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zzfzczve.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuqcyhyt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xipuehrm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fhupnbwa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qrxbsoqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tzmkocbg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bucccugh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sahydtkl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3verdhqgz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dtuqdhke.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kloylhwd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rpheursb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xqirznca.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dcsokzrq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wafswyji.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3lxzlmpja.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tbbwjjfs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsqhsb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ajsmalqq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lszqlxgs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hasremvy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvajpyes.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xjllbgak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wrzkftia.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3avceuumb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lymesljx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pwdcykmp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ydgxdleg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mgovpkpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukancfsb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lwucwwmr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nbzgjtht.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ecxmetjd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hgofxuet.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3spzrtvtw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rrazxgta.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xsvpqock.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snqhuutb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pjpysdhx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tivuzltv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ooummxec.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3puowzbua.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xlexolff.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jparpurh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qgimkegc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qbhibeta.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uzzyfhuf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvtqikbx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cmbuonxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3chkzybwb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cydqkoff.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gwobrnpf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lmlevyvt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3icugmrjt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oyskikzf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3orbfrjws.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3spbotfhn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jeplrzjj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sxkteqef.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bluvadrh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3svjgmbqt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pzbgehmb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wuurkned.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zsviiokf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tjhedkrj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mqwldtgb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3spcqdjjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mkjhcjpz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cbhskoay.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mhghzckb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3verxondi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kzovosee.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xmybbwha.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hksftsdz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xpjbbkcu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uqmeohpm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zbhaftgu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gcobhxte.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uayncidf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vhjxhvcs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zqlmfarc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xfzfzmcr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sxrgygjn.html


<!-- 参考信息 -->