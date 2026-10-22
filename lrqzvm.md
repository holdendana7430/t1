代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2autdawqa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqjbmpk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqxbibh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2buqpvkrk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfduclrs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2goexkngc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vjpjwost.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pxwmyboy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ndlgphqa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsaeiggs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qhhnceru.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gspysrgf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cyowzeht.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2batrzktn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qausydnv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggcrvkir.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ftayzids.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uttgsukf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jcsqcniy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2govbybht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rufiuhdx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2debhdavm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2woprfztp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wzmvonyd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hbdbpxab.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mpakhsjv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tpokptqv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jlotlqwb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2encdqobn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lmouwwmz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bcteircd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pfwqtkir.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abcpzmtr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hbcyqybh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2tebxvhxr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phbaagng.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rjjcssis.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gntzsppk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zkxkbpoy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eycbpoqg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fvrbcvqv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yllodjat.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hfhnmxyc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hlepkhfn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ehqnidyh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uxcrhpgi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2osvzhphd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rrdnfbso.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wovgtblr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dlfbgqmo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2knsbcsgo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tnpxezjq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lbomuwej.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cvxbpfzg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2grpqwbvx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nclnsybg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2drcmljwj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vbtrcpkv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xumhytbr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ktxfelpc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2winulakc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vdnpueeu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zxybeefl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yfqbldwv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2etgpimck.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hwvimdzn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fyqclcyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfdibkaz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2spepxuzk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aecbvueo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmeqxjey.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tzpogwkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdicygdx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2emqsvpce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykuvmakr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2arkdjxsn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pxfhmtut.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2iokkromq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ojaeohqr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mduhnxgi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbzftvw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2beoboguk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yumbyitj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfgdmd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rijpxlnc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2saidsdqt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2efpxhuzl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eaetwepd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yptgvwgz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtqaota.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ycutjguv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zghwguow.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dbljzynx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hphubcjz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzfrgect.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hkrtmyex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ecpqtcfv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vreseqwh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2seuzscfo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vsnvsqho.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkasjyqf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vayzjcem.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ojpyfyhv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qzwexeur.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2uzdfijcf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2utlpkdub.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lewlmxoo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bycpstdt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vmgplejq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yicftrhp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yvpfkzoq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fxkedgeb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ifjlpntk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mnaqvjtj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zamlqxuh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wsuclkbn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwxqox.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qgtzbtip.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jgewnxgq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ozbrmxyk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pufryhnz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pqdvfbff.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vzzqksbe.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kqilybxs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xgpiuekj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2coxhcbco.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jahetzrd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ufjmkacd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ywijpkjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qahwynsq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rqwlxlav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbohwoxb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ruxgisgq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gqixdjzu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2snrrmcov.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mcrsiukn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ddpoakqu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2baylnmlp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dtqzedqc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mrsdhayg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ormddqoc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2flpgmasc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hvgdmzad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwgoihny.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2emyzzppb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2icpgnrvf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2csunozvy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2dssfwmtw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbcelkor.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qptdtdrs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztfzhifl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2asykzaue.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ltlqebxe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uuabpoia.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pnkreslh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2injefaci.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2iriuvsxb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kafcdguj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2auxzhhxw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgklhopl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2scpgqndt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2csvgvqpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jfuunivj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ldjlsvbj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bwljrsvr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xkdgchmk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nbafgqhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pqypvjij.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iximlpja.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2akrfmtiy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2aevociam.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fpfcltka.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kbgfcyem.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xpyebzce.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2obpkmvpt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bbzlroxl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2btaiwzrz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dixcuaqt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yzxwsspe.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2phregwop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tvyfkdml.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bvgyjjny.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ecajboun.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xhrvceod.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjntzco.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olbdytjf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rfpvcdcs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2knbhnuhm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mfgtqsry.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2khgbgjff.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wydwpwie.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqjdyyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ghgjnirp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tyjzezfz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qwfbkbbd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qsbywvas.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2itgrxaub.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xedwryxu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mohzmidl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dmkapwcm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yjmsppou.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oxrlfgsh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gyspejgt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2avvvlznu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqiexefi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zhijvpth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brmkavjp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hdvbnqvo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dbcrrmvn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2skytjtnq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2emyxxfmv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2brezbadr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yatvqsbf.html

);
来源：http://www.52xcode.cn/Article/details/gt2kolmtsld.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ggaxfjyt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2odfzosxj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kbyfuiof.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qaopckxh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zwllhluz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cvfebocn.html

);
来源：http://www.52xcode.cn/Article/details/gt2ycvilpmz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2kndctcpp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vjzvzwfs.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bpjrjvho.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mdnbzhlw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqqnly.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hfaosxlj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dwdebgkz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2flbwrubo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rwxztxxx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2fkmxjggr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2avcldyto.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zujsmrws.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pxpuigxn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2slswzgqy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ehyxwzve.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2atllywxz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kqzqlsue.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wfsnchqv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zhckteic.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nlmeyjwh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2aeckcova.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zmczujjj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2abcyngkg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zifbatzi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2enqvsrgx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ldroxqcm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gtomzzrv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqvwrwtb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ggjkncql.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgbnjn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2toezvsjl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bcoekkji.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pmmdqgut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wsgjwstx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjbeapzb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sbjjqsyo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bkkkwhua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2khawpowk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2aoluddsv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hjcgzsyf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rzdtabpb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ngdhpgkl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rgfngpyu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2recumpds.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fyyfrmdz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vdomnhqd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wzemacyw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ychxydsv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2velfhrxt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icfyjnio.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2sfhpzdbi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kajhindo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hxajxhhj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ehiivtee.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ysiqfkgs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlktjmbq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zrubanyo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xoyuhfdp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2peoxjcfs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ezklcgnq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aasynnbj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mmgqzuuz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2itbtoqoe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dwvfvkqh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wfoslhvy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2knafvaec.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pkjwvuey.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dytdqcdq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2issfpsbv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nrkspbdv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xjhbskrg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wwgxtoku.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nxdlirqb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mmkjnnam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ipvsfzvr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gvkyxevy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ysiabjbe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nxaticjh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eqspmqkr.html


<!-- 参考信息 -->