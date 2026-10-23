代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mwnzzjgu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dydopdjf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iplncptl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wkdknrsj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3okppavwd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qrrxsecr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rlzjphdv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vwzuccjs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iwfxjutn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xstytokq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3umuofjuu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xfotmjuu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ilzuazyp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fxzksbzo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dzgkbiyr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xmrhzgik.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbdpxomi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uhhlwwso.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivzhpton.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yiapjntf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3psoqdari.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qfvejpdn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zaapefka.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukslidsu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3insetcax.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ochatxxx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3njhyrtnn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cyrbghjs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yyuzaqon.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uepalkyc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tlfcimnc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3unvpjyug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oplewgio.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3txdybqop.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3asadyvia.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3aflpyqso.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eakvcxbu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhafvj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dqrmjubs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3aaoldzfm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3prsknync.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdpzxhsi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lkgwnksf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nypxahus.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oiheeutq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ufsttmlv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ljmjdgtq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lcldkqrb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oerdfcwz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vtwxkpbv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nboxzera.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpcnmhhu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zamvepxo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3muarxmiv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cqxnckvb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ooymkowb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oizmbqpq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xoajiyys.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wjbdpihj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3isvricxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulynzszy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ohcqbvaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffealclm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qymdwnco.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fufzeocx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpdhepyq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jynyfkra.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3obhshurd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gxcmmwip.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ugfpkoow.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hnxazbtv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xtpfkdjx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xetnhvtd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mmzxitzy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ipwlxlvh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pgfgwgvb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tifcewox.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3egkjxnwx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yimyxkde.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hrdgvlfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rmkcmxeo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qukhpyky.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyexdpmp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zmqjcmhi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cnpsdrle.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nydmpcgd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cploomon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fnypbpve.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oqjealxd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sfolbyxg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gnbqhpmc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hydboqwq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfvuqe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kczkjbln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ybtshvfa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3oqolmugj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3btkbeiiw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tndyutja.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkvacxzh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3csxvumlg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3meepwcjc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jdqbgzwy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3thfygfew.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lahbtqme.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xqrptuhk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yobemtvt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbbtinc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxtkhn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vqappcqg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jmufeqrk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlbeowev.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lyahragq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fgwhcsrw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qahbhzno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ngadzxrr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vszibeaz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nbqqusox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypqphjfw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rjutjsjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhsssgko.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aczkaoew.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lpygygeo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xndatijp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oyriuvqf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mzwamfrz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvvsqjhy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vyswpier.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qjptnzci.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tkqeuiny.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3adxtuowv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tjgtmgfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqdnvuyg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bicfiagq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ozluumtb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3thguolas.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3swbzirta.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cvoodmrf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yxwksolo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3srrhjbmp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nmwiqmeq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgnjkfh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxnpqz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yadbapyv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dvukjscu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pcjuhpne.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dqmpnlze.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vohkljdu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xhfqbgiz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qkmknqjw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vywjzjkv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3psaigqrr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gdpzbfyj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zurwdrip.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sypzwtxx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bghqrrmp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nquykqkv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mpogooxu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ernlyjok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3syjoerom.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vmrfnglv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uyjzcxzp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qawgczws.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbobhoz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xcacbgru.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rmvsmvup.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3behhnnhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uzoujmyk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahntswns.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fairjuzy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxvcucxd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dokvfnnq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rtjnuwxg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3pkozqqne.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuxophwu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vazgzfmr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ecaajyen.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lovivjqk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tcsxcdvy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jppdkdop.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3evlkkvvx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mfhirhom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dtuuaczr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hiaiizyy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mbbzufob.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3phialmjq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ylrpvhpv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3aaqrnqdb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjhjivm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3aaiqkpoh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vziyvvvm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lwqczeqz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ugdeaghe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rabrdjve.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rbzpmrji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgoomiqc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yuvfqtfi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jaiazsid.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3yoiepzcp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3anmlpeoz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zqsvtiqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3owoczkll.html

);
来源：http://www.52xcode.cn/Article/details/gt3pgpqvrmy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tcxnfgyi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3frcabmct.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tnfsvpxj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3slvdjirw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ghetgclf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3riwgozyx.html

);
来源：http://www.52xcode.cn/Article/details/gt3cxuimnry.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3aqxxyeae.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xvsvghfu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lofegdbx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3udxzgpxa.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gjszhvcj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3gjylofkq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qgpqnhvh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3biozpeam.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ggehctnn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kwchebnm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nvsofgyu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qfgnwxcs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nmvlwlch.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3juocqhqo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mmlxmllb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qqtwxfvz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3oxmezhca.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ebfjchsr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3icosaqne.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lsavgcon.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vtjrhnqf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vzzhduvn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sutamxno.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hmkurpyq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ayufpwkb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zaynqdxe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mwsqncsh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3osluhiej.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ehrqxlox.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ugposftn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3vuknbuhf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3pdnyqdat.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tllaixnx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tfuxbile.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rknqrlev.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jtrkgzot.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bgyknjlw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jlhrgnor.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fbqlsnyj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3atlsdlmz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3joixtynt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dzjrqtth.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fkucnotn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wrqusocs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jesrzsgj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcnfimsq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rlhnucsm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3futuehbq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rfimnuhk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evupvfms.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eumlsfxu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvexsned.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fpcsmopz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kzoarlie.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iucospzi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvdmjzoh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3eixdwsnd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kudyrdeu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hgvpwuhh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ymxaoemw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3syqxbyzr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nioqgwsd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kbdlhukf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dpxcciig.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aarnaqwo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wkvdonuc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wnqxhxen.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aacdomax.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jkqmgogm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3inviplet.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mekstxxq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bqiaskow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3idzbsbyr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pefsvyym.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ssvjqtpl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3nrlrglrv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gpvzhejb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lojvohuz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jkqmhwwl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3trxxyaqq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3avujnodw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eifbrowx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nfhhgote.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3armltqti.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kzgczrkq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3luyqurfe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ueztpxgr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3oxbmtelq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kahbcwtm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3mdyaiabj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rkypewvo.html


<!-- 参考信息 -->