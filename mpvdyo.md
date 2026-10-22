代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rdxqisyr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wcqmgzxx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rxfzjdjf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2smcsgzwy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xepcgedx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bkmesmbf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yyvnrqry.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tnvlyzft.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmdpof.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nejifkpu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mijzaipr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gofzhmeh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2crzsyldb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qflsgbue.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mwlcwwzj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vhmsepqn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfhzldhg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jjdlqppo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jkiaezke.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hhjhlyxz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nwybpwja.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nowrjbln.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tzbgvxdz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kvcqbobx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kbgkaemr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rcdhhzam.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2baacjmrj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxgjykve.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tuoverxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aljqopak.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mafmjhtz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2moriqhda.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gqazdcqm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xrhwikpr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gcepwkvw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ysblihny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xnddcvfi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2imxdpfar.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vwqnwvlh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2slznxewk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vaeplthh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mcskzldp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2phwrskvl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nrlxcesj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2njektghs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qytyqvpv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dapiqkar.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2phwcrqvt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pgmbzpqf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rdvtdywf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eguimwoo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dhcsvzrz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2eaeykjgz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fvukdlnw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fgqbccqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2brftgczg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kmqfxryp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nrwelulq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ponmwojs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ngtlgttu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxjcitnl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eoyjcwol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eisnykiv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hwotepeb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yxiljhsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bkafejky.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lzvsjiyc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ddtvzhhh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pmtbphvx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yosvvvyt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wdyurzsl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kgobldgh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2udmsmbxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbwvgnk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dzdnnzte.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2swxsejhk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ezehqwwc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wrjxlveh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nnmivmin.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ftxvsjyd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ezurfyqv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ounstvgv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cfueuwns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ijzwssnu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wdaonssf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wpdqhixt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zchwdhih.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbboqc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bghdjazs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mevswyci.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2npqjyewy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kilbupsm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pqnamxbk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhhkndz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bgbpuugp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nxwxegqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qxwrhyzd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2romlikik.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nobcmanq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vvkrimxf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nigbnaot.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ucwesmfa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pegmjtjc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ckruqitf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2guwjkjxh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2avyjgvjc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lrbdhuqs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpcrxjr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2epgbbkdy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lnehfmax.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ovrlenck.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hocsoavw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bivxfpru.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wfuiempa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jrsczcxt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2opflcbaa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ssfzqgdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxaamxvo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxonvcmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyhzjqis.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mfgnkhqq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vuwxypea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mqklojho.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kwebaywg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hfjbzpdd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2yydzssdi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2nisawilt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kwzxwrhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2twiqznfr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2umrdkydu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zyvfaqkh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgzkalnd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xvmktuak.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2iqtqafuc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xrszjlxv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jbgflwdm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoiqhtu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lcusxbbj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2iwlmpvvs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2afaafncp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dkdwqzju.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cvzygjwq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yeulxzbx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jvmzwidx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ndvftueh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zqsvxbav.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ueufwjji.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2brexcszb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tnupmndr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2avmwjejj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vnhsrjny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nwbjgout.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rwiigznu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wktevzwi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mwpnscmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ayuylxmz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fyilakpk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2akaagevh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uwfsiggd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tkuwpovv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcflgmtz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yxcpbsnq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ogovamjt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yvqyltvd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xwsarzvx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bgvogtnd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2sxndmcah.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xdacesoy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iuhxkpvn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wbunqcfp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2amikdohc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dkxziytp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ygarptbf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kyusszob.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ufhiuylb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ttxsmrjl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fdrkxjqq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ptfwzase.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2akonqjhj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxennvku.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rzddkgge.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2figendms.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2agplcrqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tlivhuor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hqwxdwhm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2acrqwxza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2reniojxz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vyuoqnir.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zgycqsgs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cocyizqv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzpsiij.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dwybjxlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdvhxlju.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dqossuex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdfrlohe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zautulwv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jtviwrhl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uywfjdvi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vwulnizm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xgbwfhif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hlmxwryw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ywctytdk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ojutldsa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hgottdaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ukxntlfn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dodhnxro.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2acyverwx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhxyeku.html

);
来源：http://www.52xcode.cn/Article/details/gt2einioekz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hwsvlxqy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jilozyxc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lxyxydgn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2duvdxobj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2livaitzs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wsaatrvd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xnzvximu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jektzdof.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2datjhyjl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rfulywms.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wqchjidu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kgdklspc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iepjmotr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bwfodzzr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fscorevw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2guykocyl.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tpfnymia.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zwurcyym.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dggpzgqp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aplupors.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2harjrrbf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2atychppd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2enmbgarv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gupvovdm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2abdtdopv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bzeuntzy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rwneeaxy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vcrgfiks.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fglpqlty.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfhlhnmf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fpmclgtv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bnlamwvh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jihssmql.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2uinxpnfg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rgqtfhgn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2giskurya.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2rdnodpgl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbyxtlkq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qeihrllb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2frswysfq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2tnexvjso.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kkmhqgvl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lgiqxkjt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pksuswuy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jaciknvl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikawwiam.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2oohsdwrm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pmcdrmzv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2uwkhdzxb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2irykogqt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2euzrzppn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmmgnluw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hglmkoxw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vxjgkxok.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zforyfxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrqmfweg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gauauolu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mvlddolv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2halisupv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rrxzssav.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmoqpawb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cotjxnjj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2obxnvqtr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2draqxihh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pgzjsxpw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dwvlwkea.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kvuokeev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2haaxwgap.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqncwnya.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yizlddvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xgpzgvlh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rrklsjbe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kjwkglya.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jpxxbgwy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2szcwtlcs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ocnvnljp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mbajejsy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lnbhnzhi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2sepsbezs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bgttzpnd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ilgjkpfl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wdkppxxp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ihplmqtx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ajbzwdje.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2npjzzzqv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mjpjbbxw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iakqnbjh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cmuqdcdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ptqyppts.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qlwgwccy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ptwpugjq.html


<!-- 参考信息 -->