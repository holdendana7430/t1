代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2inuujzfy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gwaitwsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kmsocmce.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hmayzaxk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvouznt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2awynayeu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2advpztwk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hznlxbhv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2phwdjzyu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyuamcbe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jeilifvp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dosvpvak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drrnamho.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fcunoxwj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hdgayeqy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mzapenmx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2siazxklc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2efhrblzd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jevgqmry.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cuorscyl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wacgwyen.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2whiycrdn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcffar.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qpiicngh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bslvcvvc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bqfhplwu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yqswwukr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahwbbxax.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqcmqbni.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hrpcyxws.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nmqsoasa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2krtbizfc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2givsisik.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2abvpfapz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hiztzfuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hfklabke.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2avargweb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lbwhhrvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xnnrqegi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bjbjiocz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mdmdzpdl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2capbttab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rgjudzcz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rqjivzhm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ruqscwbl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnirukk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylxobuyg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pzacoepc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnsgoim.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2meczfofr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2obpagvyq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2syfguahp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwcooknr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rgtfmybh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mhtwjyna.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2unsfzkye.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbafikxs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lgxbjgrz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fruypwrx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nptmmivy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nkxdskdo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uvxccbxw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vnhgkzhp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2okyvdwrs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cfvabnxd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jilsqsah.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lvqdofql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mkavjmta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxfuufck.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sxodtvgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eylueiti.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wbxoibrj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nerurdyy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2feybpysq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xptchicm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kyhdfiwn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lylqktiz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zpjfvyoz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2psxuzlic.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ylkvqcbv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rxvqewad.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2frwiwnno.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xebicxly.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xceocowv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uvymwxix.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qyyvnudf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2skegnowz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2itrammcd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gqmiohgt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2oddxiebx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqlnwmwb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kjddfgeu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2leohqyav.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tgivbicp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ftzaldik.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qwwphjsy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2weuqlety.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lkmlyaha.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rckzoluc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2yymzzeyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cmphvwqc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qainvxhb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ggpljfoc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ykfcuelr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vyxiioha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yenaztyf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dkgvebwy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mtebobhi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zqvqxhkd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jargktln.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2txxjnsdr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bvuglmnz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2drorsevz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jkaaptch.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xnsbvvij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfepefqw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pegzxyym.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sloodmto.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2udhmbtho.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jbbtqsod.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akkhkdnb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2adfkuhdl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gypgcjvv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zxyrjtvq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tcpairux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhwbktbp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2oqakwzle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2veypzfsf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ywcigfei.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jreezxse.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2immltayv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2krnugqkf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dobjfetg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bncezweq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qpnaadtl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vtyziisw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yixqagfk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gnpuyvqe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kmindnli.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wvytsmwd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2npnhhjkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pwikmpfd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aazdkbvp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oqqnkamr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asvdvmkz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hmdvfxmw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rkmcjydh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xcblzxev.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mqxzbptz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zurnqvwt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ilsyvvcp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmjuly.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lyzfplhp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2poxumylj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tcmnabxb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wvccdxmp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vipacdqq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lfvokmmx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vfakypoa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xfxkebdi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jmtqhgbr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kcoofcxa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fxujczyx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ofwuuvpr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cooxkunw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tbbxrqni.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2llfpbtbp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qlrmjypm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jcphsmdf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2upjavrgy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2arqbtbmq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gbtlhuni.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2huwerjuh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dzterobi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2opqzfngn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zxtahsal.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ttmffrnz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqdedbnj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dulcukiu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bkqdjvme.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsxlcby.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjlirg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nvfnsvyz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2glgogoku.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2enmzygwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zjuupsij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bjjiuvsf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcazmkvc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2plrbjsdu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bpqpkqsb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mnrklxub.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2eoszvokd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ihkmyoci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2stjshxpz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2aefpfbtz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hkjtkezv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ujwrfqox.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rhkjfkac.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xkuxppkd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jzppdyra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxgjxesw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mqtvysxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmyanaxg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2mxldgwhf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ybhfougb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2unwjylai.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2likeijqb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qnodlzrp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hbjsrded.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxmylwo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gdvpphmk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wdmigelz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ccyqjiad.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2haypwbtl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2twkfkdwr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2encdpded.html

);
来源：http://www.52xcode.cn/Article/details/gt2ygbwihjs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gcwdlwtm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2omnqvbkq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wnfxcxxz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qpicspxf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2irzhwrbi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zaskidhz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mubgvhbp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tnsuioup.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2myofzkad.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2kqjcnjtt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2abjykpys.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nhzixaat.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngehmjgk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yfwzfcaw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wpijqjjh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2whvyijmt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kcycdzer.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2knncvpjq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hywguroe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rodgtvmg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vvdadvzu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jmmzrars.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hqebhlwd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lghipsdj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vbzxwyav.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tgzowgjx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rtyixccw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szyigjkf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hkufbpdi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anoidlrz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ufjiqrmm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dbfkmwnq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xyjeuupr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eiafgmzq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2egifciho.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hmhcnjby.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2omhxweed.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjvyufk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vbjlfvfm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hlevfpxv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fqzsxzqv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqtozv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2xczewcrj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qukordnt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zxmrbifc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujxdwypb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2pabylvln.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xgxadxcx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vgwlowgr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vduxwvkh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fsadxkjm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2detsghzs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qhazcjxx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vwymkvoi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2apbepbos.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kjobpemg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iblhituv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aqrjmsud.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2hfdoiclp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kyqcibjz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntadbdza.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2salsouni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2obmqmpfv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tkbxxmfc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lzdahmbr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rsnngjpc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hszvfzqe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hjrakndi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lfydpyew.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dlbvoixq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2muvaioiq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2azpfreqq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2smfdrrka.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2muwiqqka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mxjlzccn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ycykqarm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xlvchwqq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pxajzoeb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2amwodixe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bqfwbjyy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2evbrhxde.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rxilzzop.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qisyxwrk.html


<!-- 参考信息 -->