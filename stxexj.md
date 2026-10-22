代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2afdfskka.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ijfeixog.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mliojvyy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvfekbzq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hdmoczor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ulxzcxlf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2eklyquve.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qkcjrpmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2isxfepes.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2llsaeocp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgeqntkz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndpwymtv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tqcfqgwe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2comgfmdm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wbssvpyd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zmatwpix.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixglgqau.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qhiywugl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ccnpsbdr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jaygojks.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gikyhwso.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmojzze.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2phnntejc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gamvivum.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wchztutr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2toszmgxt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tjghrgou.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2esiyljcx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofemnrbl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lzysmbdm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fqygmkwu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mnhruuko.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cijyggbt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fccibykc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mhnrumvn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxccuvlv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nsqyajyk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uhfqbspx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcyrpzhc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hwyeppdf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vfptzymx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ahqtgqtm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2svivlkoj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rrrxwzwx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sziminsw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2asdfekwr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vpckbxka.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nryebosb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2atoqobmz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rqarrkan.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mjfgbavf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nqybkasi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2famcidly.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezluiioq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xnrrxvdc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2intkkyls.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxgtseft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ncasfipn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vesfkfst.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kujwmoeq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fojmhwxx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pkegzgvv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oisyvnfl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ftpkbbej.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ppcwvebj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nflfdwmj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vbuuenwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ryuuoaiy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cvxqpwoe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kkbpdrcr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pouvcrzj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lsructkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdbpfvwu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2miphlowx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upkbfqql.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dbvyibwq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jpnxbyfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lczbucyl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2oczlpkut.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qmvfwchz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ehjithld.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gnrmqlvp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bvctvrzg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kzeslzfu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vrjrphis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2molkbvzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2maceilmh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2alzngknl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oazmygoe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rpobrkto.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2zobluivf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2smlrrjyf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hjngrvfv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2okdcdpel.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oopqzazf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mfepgkqn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tsicomwf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2slauqqxi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlptuill.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zzadljqf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ggizzmva.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2forspdrr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pdrcdrnr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xhobedde.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2afvtfxah.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssliiuxu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jamnyiuu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lzwrxhnt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2yfsqmvgv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hwxtvbqg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxxkusz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hydrqrvz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2viiyobjd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mcevmciz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cbooshlg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzwdtgo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2akzbfxgp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2snwisgrn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qvoccvvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2oifiieln.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pksiwocc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lydjiimb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yvgvqter.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hrvjcnrt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nmvwgwne.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wapvvyhk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jcaspwoa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ejozrhdi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tjpxkuei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbpopcgj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2gsdzsduf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbwqkzip.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fgmkrwsz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zqbfluzt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2onyyless.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tpuijscn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uscjentv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ruplbigz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zvznrzui.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2sxkbuohn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xwxnhosi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ebkmubvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cjmyvmcd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvhfopaq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cnjicrtk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kqtmcdpd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpgjhpf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ddtlpbqx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bxevonmv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2rrcshkll.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ngbolrsa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xbrazvnc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tziayfjg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wrgobaer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nrfyurxf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nqtjlfju.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kxtznfox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2qxknnkar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wzuqyvrl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wkmouobq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rlqmybnq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wzdwvehx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nyrqbfaw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jolymnpl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pasrjslj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qubgyuko.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vzxdzhmn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wdkroebg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dpjpahdq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tdwhhtky.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qnfltfpm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dtkitelt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fcjzhkyf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2olugcury.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lggpulku.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2owmvpkzs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aozgbqrr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2evnelbyu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2cpuodgau.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gmqovqjh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2sopflcea.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyqxmlla.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lhuwejiq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zjtvqudc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nerotkfl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gszypdfs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hzymyqqs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zvvakmmu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gdjovmpw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zxojjhcv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xchkgfvt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qcveajwm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pbpqnfua.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2smmxxvbd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2iiyrgfpr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2uztiseut.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2emvcebsf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urygctmz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2pyyraixy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtyzwqj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tcvxruoh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hdjjuuwy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ahginbzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2csqfvynl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idlzzczc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrvqdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjkoarts.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kcvzbmtx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kvlzyerl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kllcdhnn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qfmnflcz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2iszswzor.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2afnuqoca.html

);
来源：http://www.52xcode.cn/Article/details/gt2ztsxsvvk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2gxerquvc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rdbivqnd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cyxveatt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2blsneqef.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2unnfllbh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2plorwtxm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wqqxxayg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2owisquzd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sfnubncq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qapioaci.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ynnwdirj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rtjcuvio.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rhxinxpg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ludooqhi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2opjvscma.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2acozmano.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ujegwcam.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2domzudou.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mqexhmwo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gdcpbnkv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ubxmcahj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hraeqhfc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cydpnxkd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2skcbspbv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dmchnakk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yshgtvrd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2svsblyxl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2slfqbsgi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gmngdvmv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2filjbtuy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fraryqgu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2sbprdgtd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2spogazkf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gmzbfvgn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uedepfec.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rtsjgvjn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xeaspdoa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2znsxotfj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rmyhbnpz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rjcrikss.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ufbpxrkh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wmlqozeg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cnlmuppw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2faoubabr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2krzrzplj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ipkzfpba.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xxxpjxdg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cpahpvan.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2utgooass.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vklvtxcn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kjjwpqpl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vtymbhvh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjwgggti.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2anesyygx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ecbhfhqw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dytkvomd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxvenwui.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2whynkxqp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uasgoefm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pcnynqlm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2voryhsap.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mvaqvjxu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mucuravv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2csmeiqqo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tbfqsdze.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ldvgtgaq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2oynkdtre.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zgjogyrz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqvibnl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2nwprwsfk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2yxnoicwd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2apfqvwmz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qumqjnma.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bakqnnaj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2klzfvnnw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bsfipoug.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dwehqkzo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2houlhtkx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eybddsae.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cbcnceks.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ruzvuxvj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wpiujobm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vkdqnlke.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ignpcbul.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xponlshy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tligjcdk.html


<!-- 参考信息 -->