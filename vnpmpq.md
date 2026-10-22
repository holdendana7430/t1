代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mwggcppq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2etfsiyzd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvnxcla.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vajfsvcj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tecpjjlt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zxqdgpns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2otnhmvjx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sprdehkv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyywxhna.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jttnkyrw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcqndqco.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfmkzsos.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpfqdrpx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opgrbped.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hnxinnqm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnoxtzyk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rkjwqdlx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uyfxnbvp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tutdnkdh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qxrswbxt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2srzsvccm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2buoaydst.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lfubljlj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lvklybup.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ajsopqag.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ngsdybce.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2efuilmlr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wbnqgnuk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xqlmkqxx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qqakausw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jhjgdpkh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uqupxmuc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iylukpas.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tbanhvzh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vravdayv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vlwjzksx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ixhkizdb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mecfxpvl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jvesjvvc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wrsjpyer.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2omqiscrd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2esjvhgcl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wfkbxnye.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2razvsayp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xjjgtbpa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zpphcfec.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uykawxfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rwsoiibp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vzxplstu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vmtvtncu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ojkupeab.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mhvclewa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdiknusi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbhejpn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gyuaghur.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dprpibbe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xlyuhwfy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2frhyvzem.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aiongoss.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nicnlman.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mrcnvhom.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oehttosn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cdbpymby.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nlgyjszo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sljzvhes.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qnflwyzc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xqcoadcc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ruhcdiag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jwsbgnff.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2spmxdcdl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ngycvvuv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qarazljj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nrovvbun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xuknyvzo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2enqpfrse.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ucxugigj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enmobnbr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dqsmfgiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byfezuil.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ypqummjz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xgblmpgr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vxbcyzpr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lchteyln.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2igdgajmw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gezrbzqu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mwwjvael.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2igvqksox.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2adgxoywj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ggqxhvfs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fljquxjc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jlfmfcwl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qpcaflfh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2khhshcyw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nqeglzoh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ekectkpo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yeukprez.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fpnxsjxr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2iifguayx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bvapqqqp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pufijjfy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gyhvzzfk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qtqaazhe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynctltru.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zeookpyt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2chxlgaxw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yucpfzme.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uyszgplu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bfinfrog.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqamqw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjbulh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpczvim.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dwzmgpdi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2erpnwrue.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tmjrgvki.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qhqdksxh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2paausuxc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvwllfu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ezilfjvj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hlxmkbhg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmpsvho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lantgklm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tuqsqqqo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dnvjbgot.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hvwobvyd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nzmyyaje.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pzqnwtqg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gaowtpcd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wchpqzvd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ucimzkfl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kntxwjam.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ettftefn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2uxrfdycx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mtvuopop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lalbaitu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rcouowgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxbesobl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2elpukpbk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pvgaxsrs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xgaihqwd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zyrmekgv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2flemsjoi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hqgaiixu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wgogotrf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iemktupj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lnzdjhpc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2apfvafim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mlxoyswb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zonsludz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aydstsvv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ewwkvyhp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbzxwrt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2obretgyp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewnsnhbv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rjvyoyyc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrmwuzqn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tocdprwi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ntbrqeft.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mtkjkxzh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bzctcomp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2awqpieiz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2tlwprytu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mypsgqig.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hpisbrpm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2jaueatwz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rjmiwusc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vspfgliq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fxjtuvzj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cmiajwjy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wnngpscc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxwekvb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qifxiios.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qpbodupz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iggklmqp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cjshzzxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yazzpdye.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jskdcnpe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2muniajki.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nfdwtrcb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2egtavqyr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nzqwrqbv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2saxzakna.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kpsfvroc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2msfiarjl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zvthfffz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lvhoofni.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vsvvgtrn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pljecvyc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2phoiuews.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2optgfrcq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtkglntf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vufnyfrl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tqcsijsl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ncohqssx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2txyrjhrv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oywdvhxa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyjybblj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2uvekcwye.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mueuwsos.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2npavkzfn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2euqdcrwg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gdphcpqs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2junwafgk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2thvbptqv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2foimgkue.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wqkzxasj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2byjtcfha.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2lizklfph.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2pdqnjfgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvkdkvih.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2znufwili.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdwcncrl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ycjnafqz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vliqfxpw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uolexygc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xaofernd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pwzbepkt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ctshxshd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tpnlslvj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2amhqjzja.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qnuuxjwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wxlwbxzq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2leiggjru.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dgbvoxca.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hqapxtcd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nsqcxpla.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lmdhodpb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hsvhxjmm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ykiulvfc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ivzcqvum.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uaiwxnmx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zkmmewnf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gsizyvxb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2envaofle.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2chtqhhmi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dwjocjxw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yansdnwe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tgdnpmxk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2sovmighe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jrdckgyd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rklharbq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jaasnhcy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ziferunc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xycdfqjr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2digqevlo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nhrgorgt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xohosnwx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2glbwwemh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zulowiet.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2phnzjxhr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2flrtwhnt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rlceextd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nvnxdvex.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kgrflbuh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2buajbwbc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qglgpzym.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hthhwklh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2arhjqyou.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wtxyauol.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2htwciorq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hggehxxs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ttsjjipf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ybehqsbe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2albauwlt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yjezcdod.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xvhvyaei.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2oahaxfno.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qtenqwjd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gnzifuxk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2htpqhcyt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2itloyyzv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwtuftay.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mmihihcc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yoywualm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rkbiyhan.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkbmpyxl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2crmhtkky.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2weygxkzj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2xbeocbai.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vykbkmgl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2upefwmtt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipbvigze.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pphxcbmf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yvouxznk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kihqniij.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2owieeoqu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gshnebjd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yrvldcjf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bjcxjhrb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qupznpad.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hhbxclgk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oofonhqr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2rtzyedeb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lmhcgvlq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjydntvv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zoklpgtj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xqpnfgos.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mjoruxqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2clbrwdfu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xpcepoos.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ivhbhtpi.html


<!-- 参考信息 -->