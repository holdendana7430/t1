代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3orzdbisi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hktxzopx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xupobvrj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3eglufubk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkootfmj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dyjdqabl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eykxpwlf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mewpzxto.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hobhxzst.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iwbbgyyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nhyhbceh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3laeuwqyh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lrdtxkdd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3obccqhis.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dtqixwdv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ihhwgmpc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rugghlfp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3otaohxod.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uwamlmev.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dfldudpc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bzajwgqd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bewrfqvd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rglerdha.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jnzrgboa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sylhvzgi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xponueut.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3foezxwah.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxukfqmk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mlbvpgpn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3adsmjcmf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hizntlcg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbiafmna.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rfwngvbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3akgzedcs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sggsqxdn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tuoijxjm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hmjfjvhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wcxxsphp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3cnzcethu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3buqglmjc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3coghaxqu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lnhqavkq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ingtbhwj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3swmszygv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vnejgptw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3doxcnfqj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3htcuaavy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3elkyafhf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bbywypga.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjscltg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wdjgxvik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zxnjjstf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qaudwkcp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3znurvgho.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ghojhprg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gyparzqe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pkykobkk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gantyact.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jdewwcpe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hndigaqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wdzatsaq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mbmzvmen.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dfhjyixm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kjkyeszb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wygrrtnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bqtqpuiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3agjiffvy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zaatlnnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrszqdbt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bnjhifzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzvkzoft.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qvshqyax.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gdkkcecl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gsfdogbd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mrgbwwcb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xlazllkv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uyysanqm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ofnzfmqo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dxkdecvk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hurizrrb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mvrftgwq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dotcktmv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fbvvmufi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eunntwjk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jrhidxht.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ciklcwki.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qkvrsvse.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ffcpyils.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nrcrlhmm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpkcxk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rhdjwhks.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3racdeadn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ahisofob.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kxqkcmpe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lxvrnkkl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vzspqxqi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfrrnzli.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fdppxpsz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ziqzloxl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3isxugiyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3iqygfykv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3reakygjn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdvmawej.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rrvtjveu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yxpniyuu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dbsncxti.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ambtqwzp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cmnyhaam.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ckpcxobv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tmtvwjds.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kymgrbxs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfxgrkg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3piiwzyqx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3essdxnah.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uzidcoyn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wteudodl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ivurmkes.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3mshsoswp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gedgcxrl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yqwjuykh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ijbqhmjh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tbvbfggl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xtynklhr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mlqybave.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iddadhxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckqpieyz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pdxplovd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfmcnmqq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eylisptk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nkqueone.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3roerysoz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3twuecjpd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pmkjifqb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hepddfau.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wvsryyui.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sbvwecxy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tcqulphx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3tmayasrj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hhoobems.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uwiimrtl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldbhsrqx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rsgyxrmg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfjrcxw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uxzycqid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogkmkpoc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ujhtvvwj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3flmjkbgy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cahujfva.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vzbkxgih.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zdwwsoqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zbuuzrzt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fdmtvvqn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3aqtprgqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3klpzqcjr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rvqayvuw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3cnvcfgoz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zzekzpet.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zbgzvure.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3urxfrpjq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cgrigtbf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdqmlg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvvjgda.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ztikgeme.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ifulduvy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gfdbwbpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nlfkllry.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3anmckhyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gmkcodcl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3njvworrm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3zhsdjbaz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqhcoery.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3edbzzael.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cikiobaq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dutgidem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3adhutemw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wfrutjuj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qrvrwdpb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmyknjrx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqeglxdr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3siybzgqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dyqbrrbv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sslynehz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jnmidbsx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3irrsxzku.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3epadnmya.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qxtuopte.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ilnhwlqa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mqaewgno.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wbmrmvdq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hkbweuzy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3mjttjoan.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3aamwzdyc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wmlkfkuj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvevtr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fbwrieps.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyrnbvmx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ynybivxy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jqftvzuv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3moxqdery.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tpgujgkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvqmmthg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3udrzzfnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehmusdjq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dgtiafhu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kcatxwkl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mhnsrbjn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kbdagqbc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dahrompj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uxjapliy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ztnbvrsp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tljflpia.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3egelqrvr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ncroygys.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yfuemojf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dgiwwpig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tnwghtib.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rejrqpvz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kmfsbtgb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gnfyahvv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxttpmnj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qupimplm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qjllchxm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kiasnjar.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ftayedpq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lvyqrqcz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zptnnake.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycagizef.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tmtvzbdo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxypvy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jlojwxsf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gocerbnz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rwixxvsz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3imfpzfgf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ahuvwzlc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ranuxrsn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tegytdvs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lnwfroab.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dmnrvifr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dqnozuif.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmkpsz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xocmpchv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qzrvwurr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3aopzujrx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mwppchrg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiqyxvib.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3szgwrkth.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dgfhpeoo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xbnmqgcz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3omzoezze.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hrmvlefa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ngguiloa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3spjaemjg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tlnjnwjs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xvwtvpqc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dzleyvhl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ighbwqsc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ygdvfskh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3opdpdgme.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jdctmalh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jriprmox.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3bplzoskd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zjpjqtnh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3srcejbfo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3whxujomw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zndodzsz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uuztgwzi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eairbrsk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mzkfosgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zexqjxtw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ehssytes.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xkvgczyo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jwcyufsw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nimwybcp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bvenzxaq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kxcadomo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kkdxmwam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lygnseop.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ucnlycjt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrlxdvw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wtdlngzy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dtcmlzcu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xrpssqls.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tzvefyoz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hwaooerr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vkassanr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qadmbbeh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lpeyophw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uhxoyako.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ckgvxnrl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vpdjqtwl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3etddewoy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zgqvymkm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3yxorycjm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gfncpgyv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gmdxquyt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wsfewboh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3utuitina.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ozzsdvwz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wmaztxys.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jlvodqmc.html


<!-- 参考信息 -->