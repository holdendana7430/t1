代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ivsnjlft.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yfwphgob.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zneuylis.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2eputqupk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qboekxqf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzdlysii.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cnzlpksm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aatycfwz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ebqoqtsi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dluqizev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2srkpqzjy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2feptoupi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2asplmuld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iuprrusg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hfyoevel.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ewosorxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fzsgkral.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lbbikpxu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pfdcrnpn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jzdhrwxt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rzahlsrz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ejesfxsi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qicnxdzd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2crjxbbhf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkslful.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2odyvsqdl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2slgjyevr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yxibnwxd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2heudnlsn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftxxlyol.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xgvwuwym.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yasiyhai.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lrgziamb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pyexovri.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mxtrfyuh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uveoyjtk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2faiogqgf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hjjxtceo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tekbdncn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjztxybl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2geutlvlr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xpdiktai.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jznaggqw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwxvjjee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvpqosj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tuivmqyt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jsdkmwbx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vjykadkj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wwewukxk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewotxxzi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mmhzltpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lmkuxpxp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrxnpnnk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uncjicyu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mrzvmqrx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2phgzqvjw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2swnhteyc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wqufomex.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2elozjdsx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2uxvktkzv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bhjypggc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wydumxxs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kozexqsr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xbgpzbgf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zrkpferz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2devxnpfu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lwerqacm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pflccaqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlixjdlk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rkyilzva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgsjqfzx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wwsnrocw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yjfnlgzf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cghnfdrb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nscgmrzu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eflprrsb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ddjfokro.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zshgkngq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2eooiusyd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rnmrxowu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vmzeiqwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsmzjch.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tctrcpwf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2joalycul.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xhaeoccd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mwjiokik.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pkllbgtl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ftnvvwgv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxalqd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aynfzaql.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2suwadjrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ejmwsqfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dbzfwwzh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fucrsxbg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmuslgdh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2csvkjrul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvsfvqh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvylqkz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xfgqvwmr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zirdsbwu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2imhpshzg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsiendxa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jotqaayd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dduzljmo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lladfojs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rxjxpxxz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnellyrc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cnqrbpgv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gvxapidi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zkgncbld.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jaoutuen.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jcspygek.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2siewhgoe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zifoecjk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqudkmi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwujkmoi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wwbdaxil.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2iqtaxidw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2npokkkvf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oszvjuhr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aflyhghv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yquqynur.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2keotkmbp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xxndxwah.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vkgbxgln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipsbmddv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpqwspvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjfqwevf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2arazftvx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rfckrggv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2zdzzhvtk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ikgvlxmy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pghksixd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2evyqmues.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rxcajjwx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dsfmwkhh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2najbxhkd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hjxykcyb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ulkwnfjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omhpmbmv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mqbmuskl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dfeslpva.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qlwqqolh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mvrkktli.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egzjchtx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rrktuomn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czpkcigs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wphniqnc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uvfqokhe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkisprbh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kvjitdlo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kajlsqhi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rchlomvi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2byzewsue.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fscmhxcw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rvksnlnu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2yfuvukdo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ylqiaasm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ctmcjnqp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yuufaxzu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2euqpwlja.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dykfonua.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hygnmckh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2styrvycr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2bgzgfqmf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wzgazphf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gugbsaue.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eofprzlc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxmlsgq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mimxtdsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vbcqiukv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lnesqqwj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pgyodxqq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2tcgszbhd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lyfdxpuz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2iapynypk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qplwkvgs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfpowsxq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbohyak.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlyaafvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jpjnvihc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxpjplbi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rqobeebk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kvkzthpk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nninbezw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rapjgwaw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owthdzuj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bwbthqbm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dvjaizjm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cytvukjo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ywilrnmc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bxzzatdn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lrzkmuwd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2htfoccpu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rbnbilpa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2doeuodlj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dzowaryp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tqjrblwx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bpapsfte.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2arltnaec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rldfzgav.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dcimirke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkeyephy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2htzfmxfn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tcsiygon.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2epgopbuo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vtskswrc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uhqbgdbt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qjvinvmc.html

);
来源：http://www.52xcode.cn/Article/details/gt2utzorraf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2drpzmesj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jkurvsaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kvueuvnr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bvouuptt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kgsyyppk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2thitolzy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ktqsooon.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2atscttac.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fppaouzq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cokbahes.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ovhslymj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2osckamnr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2imftabml.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xqherepe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ygolsfqp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2feofofww.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfaiaclz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dczqhdwl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gqoclnlf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2lrlzgghu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ahqlmqvl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hozzjlmk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vchearfr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xormopih.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gvpmhrnl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ilpfbfeu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2syjfynxb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2oyeezhux.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ndtstkrl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xkagjiiu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2oojhseey.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bopwbyoi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2afvgcstg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2crrxnrxk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frsvfsym.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rfuqnxwa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwrfznfv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2thfrhdlp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbobrtih.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iywvwhfz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2upqwlayn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2btyqxqlo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mibfumuj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zplussdh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdqwujn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bafabvdw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zgnvywyz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qudzvkty.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ibohfbko.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2beutcfpf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pnfzmrde.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2glycvamy.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqtvrhsn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rkercndf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2klphclhm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ipomzdei.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2naagpzwx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2uazblyla.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psdauryk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oveyrkhf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nohlaaps.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iaylppbv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wdhcxwhv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gsarbupy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2awyaoxsh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gngljgci.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ccxjztvr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zijbsqlm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vujttrah.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qpuyinuk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2laxaofjg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cemsmvea.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gesjskeu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2heibmwdz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uzheijch.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vfiasdfu.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sfcfxeug.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vrstdojq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uininwhe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2svluapoi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nipicliv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2becjnefe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2edioqess.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2otgmmuun.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qidjywwt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gpdilihv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hnsdopuc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dhhfswuk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ckbepjpm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lzpulzan.html


<!-- 参考信息 -->