代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ixiymphd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3docctrjs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsfcqfpf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhspixmx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jtvsxald.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kwabyzqp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kgpxtfvx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yybjtiwo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3osyefowg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrvftksc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3znwcmpam.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gpyccuhp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eojonipm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uiurqmhb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nkcpabla.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oqnnuyti.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qpqqyatb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uglzgcln.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jbwzfbod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ibvpubkn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xkmwzywx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3okzrntia.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rwfnqkph.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zpaiigqu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mbqocypr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mebcqlwz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3msgobclk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qmbuzlqf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfauwcyg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bosmplao.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mcimmznm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ojtncjyl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jadgdrmq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cmwqvlwd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gyleptiw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jrlconxq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rpipzauw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aphhkboy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iowrffid.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wwkibqvm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3peeueyqs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pclstdqs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jdbmvevz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3waucsjdk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fbezjliw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3eejuznzz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tcbuxuuf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ioavywmp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jyfbgpfn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tkzrxatv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cialufex.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbcyubq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3avmwjugi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3upafhtpm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mhmxuzou.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vrsbpjyj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxntokfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhcxkvbq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tdxnihpl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gddwqdzf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvraopyz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gofwiqdp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3utlzkdrl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bfabsecc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kqqibmra.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lixaacap.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dihlsmvk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mirqdqsu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xmnucaxl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bfyuaehv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rbxvuxzk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3paohoomi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovxuvovg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aqkseayo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtwzwyqn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lmhjbjvs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3afnouuqe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3djegcurl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uwowysfk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zwqvvdpp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mvqvqwqm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rsmbeebb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxazvvo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kizxwmbt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qpbyffzc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gikrfvzt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bmjzedrl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3frgbsygr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ydzldzli.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hiuesmtd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3sjrmyoik.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bcbucvco.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fsvcsukv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jcnnrmny.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3aberooen.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wurlejpl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yrqefpwh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3urrugzdq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kydczhbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yabfexoq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtbhetq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yiyqpscj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kuncxppw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rrfwqgsm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jpgguago.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3byknjbbn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyhjqwwb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3woohjdjl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3julnnvqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3gbumawmw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jssimlhm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dprsblig.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gfkbpned.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3djeyavnj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pjfdyvwu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3znhzzebn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wfbpffnz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yjxzpfga.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vpneodrd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hjeaqjjo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3llgwlqsw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3isvpgisq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gkrnvhym.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3butragwg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qwntxlmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rseoxfop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cdcotxrh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tbmqnzyn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3uplidzhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kisbqpsb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dvkhxaih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fghlurcw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3faezwpei.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lyvkvguz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bhdtmgvc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hilbhtya.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3exlfooqi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nbpfpius.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3puvhxcjf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3liyflkkg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bphhfzof.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jmtqborn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3flfbyinx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dcyhqayj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dbadxpob.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vdkjdowc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hkaaljzn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ndsdmqox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geamslhd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xpvhgvso.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jvwaffha.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3edrddpga.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qveryluk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptxkcmvp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rflfenms.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djwzazcd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ijwmcvkz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvbbibve.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyjozz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3jwtvysji.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tgqktuet.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vtpvgejj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3urvmledt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yxlvljsw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aqnppjsu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbzxgpq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3lwaaswnn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hzncdxil.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3utxqpavq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jsrverbt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dqcenhiy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tphmeesr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3crjoqorn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mwrzavjb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3thinocub.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3beotovsh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gfioueta.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3sopdblyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jojxqafz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dsvcmuou.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3izdfppce.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tqymkpvj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tolvujvo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gngdcalq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3aobbqdee.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puummjjg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ayanjdqf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hfuhlzmf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3utmcmlgy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3frjapmro.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gngyhrdm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3whphersw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mlqcdkma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jurtmgsf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wdbjebhj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iihpkvtd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnnchih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zmrpqanb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qvfvulsz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjeogkzu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ufifpjtg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wxmnfhgv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3xvfriuqk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3sxyyrglg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iflzbwah.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pkkpafpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upyjggvr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dvgdxnsk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rperuepn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hubwyoin.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mrxfnnol.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kqnnqhqf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3itgjvkyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qpyssfro.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ujtckqzo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3wejcfnlb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ykmrfijz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3odzoxbtj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qgdqkuni.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cwkhkjxf.html

);
来源：http://www.52xcode.cn/Article/details/gt3ftuipnpw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ymypdlfi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kaylcvdb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrnxqzlj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kitudtfq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ourdehsf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3edoanumg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hzdsevpv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3azunkzou.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hjzuqllq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xkhtjkko.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ksoeglkd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ekstdehc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pmayiqyi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xedasxew.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lvicmoxm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3didgbqgh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ieotdqcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gqqgwuzv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3nxahoayr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xjdazewy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tgjczuwe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3afipduef.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3djhilktp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3urwklpye.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jfligchc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ekprdjhi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3fqqrlmph.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxnunbvj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3psxrmjrq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivcofhkz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3iaicntgu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wyaxhfbn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vykxjgfh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3oeppvqiy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yuekukfm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sqvxvmoj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3gzowpkkk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cubfjidr.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vsknmqly.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xdfpqnyt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gcpmpqnz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3oxltfxvo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ichtddkx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fcnqjkek.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vnopwbln.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybvpesaz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3skqktupp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nghxdaje.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lzrfzpov.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skoaalfq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sljtdxsl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxvstdz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gjphizyo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3scdtosnl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cprxgnjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmqslvxw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wcijgvxu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aiyqdmcw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ndgriqmy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ubyexlqa.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3foppvxiz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3znkniuto.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dyoffvok.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3clxwlvuf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qcujjoaj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wkjludjb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ejtnbuqk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3slpagobd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jbeummij.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wlgtgtzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vaiebems.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3eddyklqg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gzlvmych.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mxqytret.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yhmtghpo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3sxxrgsbl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vigdousn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mjjiesck.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lgxpdgnb.html


<!-- 参考信息 -->