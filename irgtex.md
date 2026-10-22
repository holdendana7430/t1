代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tplvjigz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2amctyrqn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsuahba.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mribwnbb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wctqrrha.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hqwexlhx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2njrgxafk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdalkreo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2trgbefzh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tngdyrnp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rmebkcwy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pahdemhb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmctjday.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etkznbts.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mnaurmmz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlnhjdvt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vvxggbiq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jflsfpmt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yyevishb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eojeytts.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lxaoybka.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2expxpcsb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xgymitul.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ymujehqi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hteioqgq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwfayzw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rqpcowpo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yogsjbdk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xjqrdgvh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2khsskiij.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2alkrmgob.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rkhhinjy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2imzzgnwc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iqvnkmun.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2awgyridl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tixusnlh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvfdkbms.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kibwcfkf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2voboeunv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wpwmrxoi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfabhefz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lhqbpbyx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ynvbodwb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ftbuxjzf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cpavxmgr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwgommxy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2bnlgklid.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pqelofge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tlvdbhnl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xibdugtm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2eebuiwzw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aalhayzu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2azdkzbpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zwpzthng.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mkyguxth.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdayfj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xxyapnpn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2adqdzjuk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hcaavoqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nerexxzj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ftnnqumi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yanruoza.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ankybsch.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hxjckitc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2srcrrkuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gmtfjyru.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqptmkgr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nqwjaawp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ppbfbiyl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aopforrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rugcfnew.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2przjbvvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2puincreq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2renrpyzv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2havibaxu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bfrwaguf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oldgpixy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bqpbcxyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mviuhjik.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jifipjvh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjrgjzgc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsfdybvf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hcnqivux.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uobspyij.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xlmirjld.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2faiiolab.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wxslehrl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tjirdmwz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmgocypa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2guopzzfu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qftrrcub.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eavgulql.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gkxbcczu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2moupebxv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wfvcjtct.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wqbeedpt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2sggdjkpb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lokxzgpf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zoygasxp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kpejzonw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ionsdtmc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zaarfgws.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qqnivilg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lqpxzshc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tyabpbnk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2okhhflrc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2tvcgfwoc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fnkkqmnf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wdijmnpf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pixxcufp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqdduxn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wcxlvmid.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vjkvgtgh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ompkhmcp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jkxgnlqw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzkdke.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ahhwyitk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2itmkjibz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sqrfqaxf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nelslofb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dgfarhla.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jquophoi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oroxrqyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rutmfubs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xmypdnto.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qhibohar.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pwifzzgl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iedexecr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oqlxklle.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnxjxu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fmrhstgj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zohqarbn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mhkstjvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2medmbdyg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2xommdeja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shsnfrtf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ombcbmtx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2brqtovgl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jqeatjqj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzfzitqf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2envudxxt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ycefybyy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2txkybqia.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wtgozgxg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bgbclqgg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2emhvlmwu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hfjzwecf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eowjhcpm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2izriphsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2iqgzlmju.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2klpzcjht.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqucwryg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxqnytb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2espksotr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vmeogwhi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2saivrgtx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xzqdmleg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bgcqfbff.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2libpkxlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uswvvqft.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wfuwunqt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jertszks.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nmiszpdl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bagdhtpa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cxmffvnq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uqajuztw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fhzcvfhi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ugdpvjfp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vbnyfiya.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxrmrjv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ynhassry.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2veaxzvwx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bfwudupu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ukrylmwt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tqnupegm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wpypjlpf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nnohhwgy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rvhstueo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtrukyv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vuatxgpi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dkeszdwx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hpbpycvh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dpskpzsy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtakwfpv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wdcqosge.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujphqqqj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wedkvgvo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jjxnpnfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yupseuxg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmrlgele.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bqzlbrep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cceodyat.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2reeknhpq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wxjvwpcu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xeruzlem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2cturufad.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tqitookm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uybggrwv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kvdrchzd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vfvjfyrd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vkftphmh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ckbuqdgm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uslbvmmv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vqwiipzt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ffzkgqor.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2wlnmwxmz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kzieuhst.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2knvqszxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqvpxatv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mnhgxrij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fctapscb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2nvaqkchh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2uhjdsodz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ohadlwen.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mnaglzbx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rzidnkkt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2oluuxjng.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dwcejpso.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2akwjflgn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fqpgpdiv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fwotccls.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pjdsujqu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sgbvetfr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2deqhmtni.html

);
来源：http://www.52xcode.cn/Article/details/gt2dqjfqegc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xbrhiizh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hbhzzlyh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cwfxiaic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2irnpcgmc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2akcqzbca.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2eitnnuri.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ocdhgbhv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mkfzrutn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rvoqlims.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkvtmsfp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2bhfufbpg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xxmmoigl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ewzovkme.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jojgrpzr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qvhutyfu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dohjhwoz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2pgerdjdj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cqokbaze.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2egqabkji.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wcxhnbkv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgheoq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ukzmqfpx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2prxgyloy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvqhba.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ueksmptz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2dlohdgvj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fwakduax.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlqtphfd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rlkwyhqd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fptohjzv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2brhsdnwe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nwfldlqd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ckeirmds.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lbtaqeur.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ybhegplh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2glnojdhh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ormgiwoc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kjrpmrxf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rhumehyv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2teflaicr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pzphwsma.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2whtdrjcs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lvfisina.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oyxavssu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kkjljlla.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2embfrksz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ukttlfvn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2futlybbx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2locopznl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwefymdz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ohbesqvq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdewptlc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zukvjxeg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnggmjyg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uzqszqgu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bobwfrmv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ctykcens.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2indubhbl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wdlairlm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gcumiieq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2awjyblep.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dpltwles.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mlfogezn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jggjltbm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pdxroaom.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nqsxdfyj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cikulrwl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fgunctfe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxmueaub.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xirkueae.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pavkedhn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2smnnkjfc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aidmwqry.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ieutevnx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2cikdrpew.html


<!-- 参考信息 -->