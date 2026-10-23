代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3txrnudxg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zxuxlaah.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nytiadqo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3etycnxpf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yvtjppti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lzuueexy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlgtenw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3thlrllrq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxtjdiw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3svdknwty.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bkosavsn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugumzndp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ymsquhqv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ksvhuwfc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ajumhmuc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3owijxpck.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bglgwwnq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oxnawoqa.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tufephin.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fflunpjr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gezlmsoa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zimkmqtq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ehhxeavm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ayfmcyso.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3iunsvfnh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nuqunnkr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wtqqphjv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qcdpbngx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssiidkfy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3szufahhr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckvjzape.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cilivhji.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iubcjdvu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sjqmyfpe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jzcaqyuh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ifcbpvie.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oabxnfpn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gipsmbiq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pwqiyssx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpbwcjgo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zxnkkhzp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihhamexj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kzfxesrb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hgmxuysq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3akimsgey.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lhfcyoxa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hngzzjak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjasczta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxxyfpxo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pjwmhgny.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hydghkgk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bgmzagsf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xhurglov.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cptetyxm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hubszpeh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eapdiryn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lqkrjium.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qarrxurm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xpaihcvu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ubvvxbas.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xrkuemoa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rqnjvsgi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftniloof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rlhzxisd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lgkmxyej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3efekqbea.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qvqxgxiy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pqjsjvlv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kxgiksko.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3efywghlw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3phncqyof.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kbpeopea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzynhdhz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sbtnurtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkfnaq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hrelhmly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3uygrqlvk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlycfiqs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dqriudib.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kwwmrngn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uzukogrt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dwzinysl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqyloiv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3iyqljweq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yfierzzc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3lwyygvxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfdofuih.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sbqnzssg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xgsfexru.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wdamrumh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqsdbn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dxduzyof.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pkqhrnnv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3arbhdfde.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yqrruccv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mbsmgkxy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lstyetzg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wkaejuaq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzyxwswz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cwlteomc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfjwlwgx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uivmygwk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zdrurdxf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gpppxupc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tupyihsf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhydfdq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sjorvidk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3beoybows.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bbwwcgha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dkvwycjt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3btftqhud.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3etptjvbp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zspmgjvz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yislbaus.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ucdeogdq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xmuzdvws.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wkucncjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bwcamivt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zkapdqof.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wklqaety.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rugpgivj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ntlifuqh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3umunncll.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mkirvgei.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ydhgevkt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3yaafobop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rrazmfet.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3clnmrutx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3btmnheli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbwlbfqu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqoifavr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbgoaisu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oqnmkozr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3imbzldfj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cmcunjby.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wccswbxg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oljdsjfj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pmjaozei.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3htybtwxl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rcsqjwgc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3drapivkz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3aecvrpet.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ftrfnzgk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xplutpoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cogsryfr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rkxhfwfh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3scnoumhv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sodcaydx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxozthc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zkiavhms.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gezudrod.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xqgsbozw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nbxcmjax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iukhelga.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zztpyqrh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3szespalr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3spseoxih.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3atiguaki.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gpofqjuv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhwhtkuc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3osyiffsw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wmlvqrwn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3srrinell.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3itwmzwit.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rkygeywa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3njwxwero.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gkaqcouh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hrvmjuwb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ogcxkfnv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3regkjusv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bvuznrfs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jaqnwull.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3frwnudwe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nwdmoztp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kbrltcbe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xsqvotgd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xnohqzgn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fyrvgfpn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nellgqko.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzngpkcj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gosssibz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3pbpsexkb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbsjim.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vxxddgyc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfsytzv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euiqrorx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3yhhpkjxo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgpbzj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pewsyddk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ruywxmad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wbjpocbk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3grojdvtv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3sqvdegow.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nbgfcncu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3joilthen.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ursarvov.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3thiiands.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nzgengix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ddrytelk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zlrtgqek.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nhsbjbna.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3vaqkitbt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jdbfohlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pmauxssn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utrlbndn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aipsufrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnylspuq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ltxikder.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gqyeswwz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ozuotsbt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3djnnbvfz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3klmtadim.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ystdbnbv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xxujrrfo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3blgidbsp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sdffabyt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3safgqpfj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fsxzcfrk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hzrfarco.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bavljxdu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ixsclwtw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qynfierm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3trezzdmt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ifkvsrjb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dmahklhc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3infmikxg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vamqgxem.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rlcglrgi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kekzzhne.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3pqrreoev.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ctwjnwbf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ujicbklx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ykaifrdb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ctkeilqt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aztzxbwz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3plynwnbu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xfscabhf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kuhajpda.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3toashzcm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vboqddyd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zgeygdcz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kcljnmkk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3upwienhj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uxckitiq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3spkrinhr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ivmbmyfk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cmdkglcu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3njeoloyk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmiwigvd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3soquziua.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcbnclui.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qdubudhi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ylahhozi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kblhvvdv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3svexehmr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3crfoxwnh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qhoeuatp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fjdzjynk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wxnonmnv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oakxtpdh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3scujyvys.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cwibvxrx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wnazoqtp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3canyvcuk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mcndcwin.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sjioxqru.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iesbclmr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jrcsmszk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kdpzhqes.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3chdhybcx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnsfeuqh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ohdoteju.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wshvwxla.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vipduzfq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3urcyvhhe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jjuubklt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfwvnwsf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxcriy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ammilcxw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3oznxofdx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3scestlrt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klteqlwm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yycdkegd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xiwlvqzv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rqivfzwv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dppkdxpm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lgwufgka.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ilvaqwce.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gpidrrqd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3btyogqea.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3obqfjojm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3icdncpgn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3uggdrgvi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jljocbgh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qcbuubwb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xiwlwzfu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3urswgbea.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxruashn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mgymqpug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ftbjiafd.html


<!-- 参考信息 -->