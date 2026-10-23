代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3idaxkbms.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mleekzdx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tufwelkl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cljqgjoj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zonrriqp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvbbnbni.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3whrkxbbf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uojjhwvu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3immfbloe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3edxvgdqc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nbhyohnm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kdchlqcx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nkwlclxz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qjunssoi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ugntsxfr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3evakkarq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lpelbksj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pxljntor.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ehhmpeju.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dcedsegr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ybabvrij.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dlzesmnl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tvibynsn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jofnutbq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qgyfzavq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3estioykv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpreaiwf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wtfimrvq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zxnvfrzu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hevegkaz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gplnrqub.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hhrgbgpr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wjlypeal.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yyrjifvp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wzmrjavl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjkyvruf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gyydpsut.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gckoaada.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ovpnzbsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sdougwxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3azpejdcd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3whowkqbc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mbgimlhz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jhygluta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3phtdunvr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3suqxskds.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kpvqlqng.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yyfxeoum.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yhgvtiki.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpsicac.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3djwthowq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3caepcnjp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntzrgeee.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3spvbltvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gxqxxcjc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pnxlzfjk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3voxciyht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3iabzcjif.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3obyzbsfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3goztvdmh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zdzxdtrc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qwbgtwbi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bevdchue.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ovwufcch.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cqydsiuj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bhmovuiu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mtfrmuzg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bwmhlpdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjvbjqzn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3duqukgag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyirvaly.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gwiqhofb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ngjrxnsd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdvuuwof.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ehradepd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ybgpnffy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ydzoztov.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hfhgpplw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xpjmxcff.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dramfrrs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fgugqxuw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vpwrinuz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qdesxpbh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gwjqqxra.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kvnxylve.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rpsahiig.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3czxognvc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zydhqmho.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cifysiqd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3pkxcxqfk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fpachiwl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nptvlxst.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3extzkmvd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cvuvdqvs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tjpwaupj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lcncdmfr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3juoeised.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xoqrntik.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wqhgihil.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ndwclnke.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pdayopgp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fqjwtiqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uubqjoit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nzhljzor.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3prssdkvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qvtixfch.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3otnparzh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qruxfegk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sxotxnly.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dafwxnyu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aptzczhx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iloxxohu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kgqwnvws.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3isfqhqyj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwkwfnx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qzfjbcan.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfjfixac.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vvgjrybj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nuioiowo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3altvfvaa.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gkkxyhaw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gyyhkcim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wxrssqcw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ewwjsjji.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gjphyfoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diiilzyy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogyofkns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnjvogbj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vjlwirak.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3eobnuwjo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nurkbidp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hdssldve.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sscoufjw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3aoxehdkv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tcwyxebk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nzjjbqdb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sugynudr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gcvtglwn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3paarzdks.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rsxumpyl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oxkgeeoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jftnbich.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mlmpphhk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yoccntra.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3boyjhgau.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tnwuhiqh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpamhzbl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wlawzrca.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxslvxr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgljhbni.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xybqessn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ysjnxbew.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yczrdkhd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vpfzjxhj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lsppgekm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3srmvefkb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pnfpnnbt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cynykxjn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eumfnoyg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xdgoqxwb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ixtjifwc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3hnvvqvep.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sclgcqhr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3akuiduyn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hfaleczc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mtokillw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wtkdjtwh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rkxhsahk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrysjte.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xkdqzffo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bbuokmlr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bzmxmeva.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3upvvjfpw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3tcqeomah.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ynnrgygl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fipeilbw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gepyknsg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rasjlmtz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wohtjdnp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jmlsfivh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ptdpyuxh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agwnmgba.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vlrzfyxd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ucuyomui.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qbfclrit.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yplnxzpy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3udmzfmky.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gszscsud.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rxshqacb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zukiiivh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jezlcmig.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ygwnvwjv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3sehcynzo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ajphqiyj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ihomitjg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwbdbdt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wkjjsvgt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fovzxcpz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3iwdmekox.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xxzwxsus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htmxvmls.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3csieivmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cilxwshs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uqhinyoc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ccwgefwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jyahnnni.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jwkfvulj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3tknvdydo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3atgtwwgn.html

);
来源：http://www.52xcode.cn/Article/details/gt3useqaluv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gntxmchu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tlaxwwax.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ajvglapy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cansdkpr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ffeqqaga.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gigrkokf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tnrviizn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jeaxzexg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gcipbwfc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmjgozwf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yqegewgg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fykjjrte.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vyllzmvo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mzsfqfzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zxbxtsmv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3fqvptsjq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qdgzpldq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pxkzimzc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3orhiksim.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ecxxyaxe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3iiwdfzap.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3aabyrffn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jwlxjzts.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wrpxeiuq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jrhfpeap.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pxrdqtws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yaibiuhi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dnwecivt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vrrnfqiz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hobzqtmt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hdcytgkd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cszxnfes.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3csnwdzzd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ipmkuzjz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujdvzcsj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fuzyzdaz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mtsdygxo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ktzcsajr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fggbpqyy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pjtiletu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pnbbqjxz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gzvnagqw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xsbquxru.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3erfwkjlg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qteaugum.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ntlpgekj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3blccibyx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhydqkqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vsinxybp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ntxzvjuf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qclezfry.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pbeorwet.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlwzzxgi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3biwknvid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wazohhsb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uxbzulzi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dnoffomf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hfpglwan.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnjvcqcv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xsnnbljo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynmqvmfo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yoxsfuzj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrpnnnao.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iscbobpx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3udanfmyb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vmpzzqir.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lfpszded.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fhkynksa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ceoupkfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ncnrzfth.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjfbxi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mxobqokp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kqnzeizz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xtykgcfo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oqwfpxkm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzxnlnhq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecwlpjar.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kdtzfsxh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ttgobdqo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eqscosvh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qtszotke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dogecfzb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dusdivzd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mkuslmbr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ggbgfwue.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3arpdqpaw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3enkfqexw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3swbiidif.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kwkbupks.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yrobpijx.html


<!-- 参考信息 -->