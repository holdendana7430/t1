代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fuvwmowo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wsbaarac.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3joijrnzl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3widalnod.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3frfidjpq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3neapjdga.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xkjjuvbl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kgaskncl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghupdjqt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lpfwirhk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jrdekrof.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gmovvjbp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3accdgqfz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ieqwnxjg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3httahmue.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lymhprlb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mdnkypwh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sugoodzc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbsizprn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qezysmeh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ffgrivez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gexdkjif.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pawppqga.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cqvuvdij.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3uicetrks.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hnuiykjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ovklwulm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wreixtef.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3szfwjhzp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ustemilr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnpzlpvz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxxbcay.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ymijyfno.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fpqhfeqg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gbzogaib.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yrhwlsqm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3umcdrxjo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lzxdvbie.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sctzelkd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3djjxnucp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cnzsuydf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yefkclmq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3amjrsazs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cwwerynx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lbxlahgm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vdkxubpc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ogmlenzq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dlfnndcw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zbxtharp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3msgnjqjm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tchnmclu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nqwrnjhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsyucdfg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oldkonfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktsewoxw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3gjwytjco.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lpzhewjk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ttxgfmfp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rnhreekh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fnesbsdf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3silxymnd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3igidyobs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ewtyhlgx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qxxkesvu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mgcudeqz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwxudot.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lfsoydad.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3egduholi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fuaogtup.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sivmekyx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mcovpwjp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3aajxedkj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dzimpgfo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3noasatji.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uppfedox.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3onikwugv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mulsbbxa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nffswdzd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3msepbxho.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vpggnrjm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lmcegjmd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvovibp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xvkvbwdz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ebibamus.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xptsufms.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3epzqadqu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsddbgyw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gopmvqla.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3toedynth.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jkpgjcce.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zxnnqrrs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3sngkieuq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mohwesih.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fiaaoxos.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpvwqws.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3deomyvzf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gajelvoz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3brffbbox.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mihklfil.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ggzdbleb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aiaxxcrq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hwkzpumt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjzgqmje.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xwzwjbqk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kuujxbly.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3witbhaco.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vqxamwdh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cpuhucem.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rugdcfau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvvrcqaa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iucgkoew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbgwsbih.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vywpkgcw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xenfwwld.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmdtts.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rottjyix.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nldwlaoq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3emsfhklf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3csyrnsul.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mcxepilo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oiiebjpo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jdovozrm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ekjabffa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3egbybsvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gtgjoypg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kuuvtnhx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pkcjpudb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pagmepaz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znufydtp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pauvbmvr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aofjrdqm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jaxelhvv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xyulmxgz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lvwasqxn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gnxtdnkw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vzneadda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gmlglsrm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cypevbcx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gdyhausm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ajlsaxtv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wsgoicfi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3swbdhgyl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3asgwelhs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wdiucjua.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qxtizxmj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tlxuhsrs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wclznudk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ledchvfs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xyyxnbem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3fjnqhqbm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jbhutrmm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3urxkrpqu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zdyxczyv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qwjtbkuq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bcaatnna.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ztfsojat.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rcsaddzk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rvmqayev.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dkxalveh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fetivmlv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3erfmelef.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zwiomyhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iznwxgov.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3migjbthw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rrjbaymd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3tvraafhg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hvzrfjrb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jlhansud.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mfpxhbeb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oyqhokhz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3crdksitj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3liwtzpll.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ocsourwe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jbkcffnl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vwzafmak.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vmeqelzc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mnyekuos.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ibodoqis.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3zzatpenz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zppbdsov.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3frhhgxay.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ezmujqaq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qinebwpu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vmcqnpgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpjyeylj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fizxddpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlepjotz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pgsmzuzq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fqhrxcdi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ocxflzqw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhnvgb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ezbzljiz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mqnqetdy.html

);
来源：http://www.52xcode.cn/Article/details/gt3tayweaiw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vfudyhgh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jhaspkwn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yjwpntly.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hnwtesaq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uibmpjoo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjhqjfz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3crihjvbn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3seuugwzv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3itmxveec.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xllbpsns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lxrrcmwv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3voffsagt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pcacemty.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cbavyqgg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wbsrksbh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tjhajopl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wngjkxhb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhomcwck.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aammttvh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aqzksiwb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3heplatof.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pznqbbet.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3spynwmtd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cjyczoca.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sagucbrp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sufgohuk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dkttuuxu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3nrcbuono.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fhvtnavd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dqlczoay.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3guaqoqrn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zoafqaav.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yevuooje.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3brjkcrzf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwuyrwki.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nsumpjcx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3itbrbmcn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bvpwzqhc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vwlsfdvi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ksokutzx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zgbuyuhb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ficjgzot.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tchxsflt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwhyetvo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kegvjpjh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fnzosdcf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dncgfwsc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uqiocmvo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3njsoddej.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qgriqdbk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gtfkoyzy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dcoydozd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pljhblyu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nvhuqcji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3giwjonjn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qpyaotey.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpbhkqxz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rsjuqhop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljxhoguv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3iwfykelg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xlyvnzqx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zxeghawi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afglmnrw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vstkregr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3orjqnbvt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lfmqvfck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vhxhensa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ceeotfio.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hkimnjko.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3onsyuaex.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3solpcftm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kydnofgf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bnvdvtju.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dyhvegpz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yugptyls.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sitodvmn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yokzlorg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wdbzhkmn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3trntawwf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3djumpdjg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zqgxxsxq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3luhubpgd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vzlsdqta.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pdvwgxfz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3luennsvh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lxsuhzql.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fvoovdwp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rcbhgqpz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oixzczvs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3grhrmrkt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sgtsabsv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zygetwji.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xxvgwhcf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jtatbtbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wolnseue.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cohilgtw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3inscwbhi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3htygjzxw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3mimolwew.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fafogtiy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gwonrzoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ndvqnecv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ruaisfpy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pirjyukz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cpbrcliy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qoqhccmm.html


<!-- 参考信息 -->