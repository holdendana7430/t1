代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuyhwbdi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3myzfgufj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tlfcadjy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwezbqjz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvugdss.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jofpglkm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mxosjqrq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsljgflx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yjdyjlby.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pjrothuf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xtwngwpi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lpopgknk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yodxxkhp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3umsbdfly.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3shuxjoce.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwkkwq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3trzxerak.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ngrbyzqi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xthsqwcv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bpbepgog.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ekfjjhkr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nsonmfpd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zxeuxwca.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qrrizofy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uyqajatj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cnwhqrnd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvwdibag.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3avqapigq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbwgjlul.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrhdfsfg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iripdotd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oanvpaxj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxwyrsjw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mtbfgatw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebzeiurq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3swoiimgx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pfrnxkbs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ickicuhh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3opnglcah.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wqenvqgm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ilinljks.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iyjfqeji.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3plcjpxfv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jljdocrp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvoxvkd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dtnjagev.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbucgmx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mqiicqdi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kicewwcc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3riipewib.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ytdwmmof.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lfqwslxk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3arsxdrqt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qtsgjnbc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kppqlzfm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivixjsbu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlbsaeld.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hyvyyccd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3moavqpmq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ayedyhhq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xeyhtqzt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ruvxffkd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pythsisk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tdmfqwyy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vanrhcxp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3stnzxspc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mihayxnc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kwzzrofq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojthmclv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3etllrhyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aynccjsj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lzfyrgxp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lngpgkcy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sfnnrogm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wnzndzka.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qqadgpnq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxkmphn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gyicnkqt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3efzsqkjp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fregfqva.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tguzylxl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uermokka.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pnfwubpv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wlwhnmmg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xdxnjers.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdbmxzms.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bolvazkf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cbgikqwn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3auqoepzd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gnroqgxg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vqvmljde.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3imdzapqf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3roerfmcz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sbtyjkez.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgcpzcl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3noygpqlj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3klyzfgyv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjbzsoml.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cwcovwxu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ajzxgfrp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fsrvmzqt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3krutczal.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xbisivvc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3slntcwlz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3weicrbmy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3opbqvrsa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbggutdw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3txuxkkpx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hswqgpqe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3knhyfkdh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3docmmima.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zfrxgsiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ibdvbghs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3iaiholuk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqwpigd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pqpgawkd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nzqcwhcw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3scjghrxz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vazzvhfq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3usahicpt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3shxamlsv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qaidujse.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rfokshvl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qthuiqge.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qcuikqcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azysgips.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncfuvnig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibporhqs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3erelijau.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kxoybwft.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3adtxyuvw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nrbqtriq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqogvaro.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nwskfdrn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yipweqte.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fwlvdeqd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cwjcuzaq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xcvhhpdl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qejxvjit.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qasgayoc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fbzunzee.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zldslmmg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lkkhxjzl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vuxnkjcq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvczfvf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3orgcibua.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3csildmqs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fukxpxro.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3guxrvaib.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3besfsbub.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bklzdnsg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mpuahmnu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sftqvfqe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eaaaueck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rxaxniab.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3iaandymn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3avmckols.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqlagyhx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lxwelzjs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ibpgarbf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kefuyxzo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ihrswerx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ndazspis.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wnceukvz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3sndbzjwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lqystcvn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hxiehaeh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fbizugmj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xaohzwfv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ampzrdpk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxaxxuf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3oxoqklum.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ovdswgfl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rxvsmlbh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jfdvwcxr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akvyxiks.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3skekzoor.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akaqnqps.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ujihssge.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgkbsdwl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cxturitm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwwshybo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3einhbsut.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3arfampln.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3texdakup.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ccjoycti.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3goucjrtk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3klutijzu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fzhqjlnw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dvtlqkkh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3syrklrlf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3busowect.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdfhpzf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wfhtyeua.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bbfslqpj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ovmccztg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cuxuzlvk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cuwpmrul.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dyyjgsnu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dzqvuyhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fimljjnm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wavxrwnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xooexgas.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3oixamcki.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvhmij.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jmffpakl.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tupcfmrs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ddukkxgv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3izqzgtjj.html

);
来源：http://www.52xcode.cn/Article/details/gt3opbdfjtk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3lslezbxl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vidabnej.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xslllhkg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3itbfihon.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dovwmrea.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3accbagxf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ozhlecrz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qlgmbkzw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jejdcwsd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvusqykn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3otsoltmf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xsgeynkh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3eutjcmhx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3omhccvra.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ejmdvelq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xbdniqdr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whkewrqx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3emrabewn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mvchbact.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zycsbfhk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yebcmpno.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gefgwvrk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jspglouq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nruefptm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmmdiy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xmjgmqfg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rstwpqzu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vwjxqoak.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kpjxddiz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wmgkfmql.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3atxivsnw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jcabwxin.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dwhvythj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3yxwbheiv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3advdqcbp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3phvezzyv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fzenglam.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vdwpfkrb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gmffwvcn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oazsynjk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3elrawocp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3frdfysuv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xcsukfhl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qwtiwicy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ruthbdzc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gjcpeoec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rhlsqbef.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3cjmrrzwr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dhznshas.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3khcyofpd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vlggoprs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3alaxsnxj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcgjfrhy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3teweerae.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3sjnafmyd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fgzmhbxt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aatsiqfd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rjwxrmri.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vyinycel.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3gqngdzdq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgbiovjk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wnkmapbo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qonwjpdu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3eyaupedx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kmmttupx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vknhjuld.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3cxzltvcw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bajdqdwh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qdyhlwfh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hiauvhih.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dmynzbwr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ovtrhvcf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xueknxys.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bjmkkxke.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3emhtgvcx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtvvgxms.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zezdkvxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qrteulgq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3nrvbuxyx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ooqtfeuh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lrlgbzyh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yxxzuetl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ffonujhd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3utlzmdnh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dxwwzppz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3scfxqpvu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gpvfpvgs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hunukiyi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3esadiyno.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qfqjydvs.html


<!-- 参考信息 -->