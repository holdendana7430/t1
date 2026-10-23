代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pmrqfuuu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ttncrndw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3eoibnxpb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qqbtzqif.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3teslhqlw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvexto.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vwyposvl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3aiorhzex.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rwkbifae.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uxvywuhs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qykrelhh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3auweucpa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhngfrwz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xazpbivb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3icwussyr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlosvyul.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kinmcaow.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioiccatk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qbrnemlg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vsfgnflj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rppewbnz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3faijdjdt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wspvbsgx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gnpxbisu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3alfchbee.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nfifqgrc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dsblaxiv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3llakczxy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pnneetlj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3shcwdmev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3edarqzhz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tcyuwcka.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3noolbczk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hihmdyno.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bslimjky.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wusenjbi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zhlwxprb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsvrahpx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uyvlbwwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vjyvxahy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymfekmwu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rlblnzqq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yvpipiqu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uycjklxu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gsffuxnf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3egpakcsh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3afcnzjxc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jwmhuzre.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ixwjzzbc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eewceggw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wujsyjuo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgfykphf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3thjfrllt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3puwjtcuk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vshbfnqb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lpclortx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhksehfc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ivlqcplp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtefondw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dzwhoqga.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3oqsfmtbn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejaajoar.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ubdrmxrn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ywvnaooc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uadrcvcg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sdefxvte.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tuoagoif.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3sfsgnyap.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ojdjphts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrohkqx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dsenttmw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3boivpfpj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rimwagcj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3buzofson.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qwebhzii.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bxuesfql.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gvhsmluy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gyrnxlnw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ntdtlwht.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uxclqgai.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kknnqduv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iaohfbaw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wefbadoe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3uzwaqucy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcmddugm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wvxupikr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ocrchibg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jjumdmka.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ohkfoeny.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xdoiedun.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zkglbbsa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3awvmzeyv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dixaomgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iwnewtcq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ricsntmx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tllfgkze.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xlbeqpyi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hyfqznfh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lebzbboe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lgquitly.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rxouoqjp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xlievoqa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nazpkfcc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3erayiian.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gnjjvyul.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmlmji.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vvvyobec.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fjoaekws.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hwjitalm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3twdifhou.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gmhrdfpd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hcheaswv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3sznezxht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhatycgt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlaycacb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bttoojpk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xkwpooce.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kuhziomb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tcutccgf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rifkqjhf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3amqauuun.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jlnlkmhb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nghfrioe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uweknarf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hjofeaow.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kfhvvyya.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bmhvalfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3feamymhk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oxowkslz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3eslxthtq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3euobstdw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3elrqncje.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlflawm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dxveoylw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uqvfouaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3iqupysdj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3majicwxj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfmawsfl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3splywwae.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfsrvw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tjaluhqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ycjsoosf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pcfhgzsi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3luddnefk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3afbxfane.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dbsgzlln.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gcabxyht.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gtbskqlh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vvksptwr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kucqpdbr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qazokqyv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bdlkvbbd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cndcnrly.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hcosnczk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3trpcjlfr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zxzajslx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpyvihos.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3eqvrqjbn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gcxagkdi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3gffsrriy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3lhbyatcq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3eiimejeo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fihvwirg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mwqhxjqo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rqckdvui.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3udzzoksj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwokaujm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qnonncjd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pnuymnql.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3soogorbi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yhkdqzty.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wkxcowsi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ovehwidd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wacpwctp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xcpbjwke.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpdoeydd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xjzldofd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qbqrdgfi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dqblnkhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3smuqjewk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yaeajjzq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhtlnfat.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gqxjrcya.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mysrpizn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dwcqstgk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mynfuxus.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3agwhzwjc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xsibrnbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydxmxsnm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3psszvvlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eafxsowy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sozgxinz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kdbelvya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3irunqbjo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jxfgqdov.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3bmnjctgl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3aucjbhjf.html

);
来源：http://www.52xcode.cn/Article/details/gt3fiojzcbi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pbejyvey.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qtgxbhad.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ckszvhbd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3poxuocst.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ptloigcj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pagqsgrr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzpfwvx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zzhjnewq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lhrrwhmx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ryomyncp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cwrhphky.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qoiuandq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ygzeszsw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ozipcpin.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vfiwkxyc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wwuzknjr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vrklbrlv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3owpmtsod.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3auixfapf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wtolzkxz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cfrxgelj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3myxgvbsw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3huxozgjs.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dwjkfrld.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yinpntwx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wczkeaep.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tknodnvf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rrcbfzcu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3thzzmnci.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rfkegdfh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hmovmbdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jbvgnkil.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rqffgnzk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zlymfkkz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsiezzeh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qczcupnd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3adijrmal.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kfmqylhl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3acydijtk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3obtzhkms.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pfoblojx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ndtkfpzi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yxileqtv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lvujnpeo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xcbmcjbf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xnrataey.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3etadbbgu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tzznlvsf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yijydnfi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ahwshoxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wuecmfmt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pccviibl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jtsawjhb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qqrwmgsv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvguzw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yoqlwfjf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3euegvoed.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3cieqhuqa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhgyhzdm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mflslump.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rlwolvwa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bfwftzdk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hgssougy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3unorneql.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdwgpga.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3oxibkgqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cxxxljay.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ykuwzqvl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hlbpqyat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bufwbmdv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hgponueb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3oulywkmx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rgabgmje.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3spmaxwhb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fpndtwzv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pmrklxhi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3pscujsdv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ttaqcuua.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3macigonr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wnaqwxyz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3usprakuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dghtdure.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3shffbxmr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vyzyrccl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gdwbiddr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ebcercqo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rqrghdpu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ziulewlz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fikguukw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mclntpgu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dhodamvm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vaikgjnj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3usrnmqdn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zipizxak.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wzkbzsuy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mjlzouix.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3exsjvqxx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tdarpfaj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjbjsfgl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fzinrdga.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3asfjuwok.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lnylnsps.html


<!-- 参考信息 -->