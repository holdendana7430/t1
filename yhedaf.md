代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvrlftdx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2stesyeap.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nepvuzzn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tvolqnip.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zxphgrpj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkudfax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2spaufafw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hjknwllc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ctszkrxs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2agehcbaa.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ruxmnmlq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2sqwufxny.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hcekrpbf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jjsnlgsq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ceqdjbgl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2motknloc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zjlxstdh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xgjbabww.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2owsnopyr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kozquhus.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbopekfu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cgxsbuxb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pgeetnto.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yezcayii.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xebhdbsm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xfejsjql.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vgljoqws.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kcuuophn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjsrvknn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xtzmwljd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ghiyyxvy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oizkgjze.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lnzxvltj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oplrvfin.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2coqpanjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqnqsbkw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dcarsxfi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2eowwrbwp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2aygoiepk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyktsgtd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ntlyzxsw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2sboutxut.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwpoukg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwnydln.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ndiabbes.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nlawrzav.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sixtyshn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hpykiquh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2icpnnuwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hmiuhmxh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sppavdav.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwgnyhih.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iopdkbuk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vcmauwry.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yutcjpgv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pjkkcslc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ekwrkbcx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dsmmfloo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cddumysl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pjslbubf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zzglvorg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tycdtglq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2drhubost.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wcmcadvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxbqnwxt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xncxswax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eazcxykt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wiajempg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sjdgxtri.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ptesfkyi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yelyjhrk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bgsijugv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dhjtlbxq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2stjrbxqi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yfgaoozf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cmpaqstg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yyinulye.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcyxrfoo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dgwpxzof.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kwtrpleu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iellarls.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tkjuckpw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gwtfipjp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nqahtvsg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qrvyeiyf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zztihnwx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sflzuojl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dnfthkcp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xivfqxfn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qggfruhg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mtmufzpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yuyrpwhd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zfditxaa.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gsohheds.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ynsqkfpg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zjjkdnpw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hnspakuz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qesiufes.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snbeztkb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2prakmrro.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dbedwopy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hmfoeowj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2usobdlpj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tmpcqkvr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2schovaop.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yvqyzsaz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zisccjjt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bjdfwwds.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2baguztsm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zzpfqayt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbpwxbg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2whzhgvry.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ihignohh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xhfvpvdd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qplqnjec.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2milghilt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cgigvrzo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bbpcckqn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2llpkamnw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xtorglgl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2txqocsvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2makkbzqz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2addcsbki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdhqbudx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uigzoqnj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2spwzwkyp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dqwfvzhm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2exticgfw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hipfukqk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2brnbltxf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fddpfzvd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2uijivrjy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gsvfetdj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2yxvdqqrj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2widufizs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nndbqsjw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sfvpjuyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hgfbsjhe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fiemwzhp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2maqczuls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bnbywnkl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2poayhviy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czlebels.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2scskvtax.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xwexdkqp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xtqwxpqf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rckdqraj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwxwdqo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2swaaoieu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfrcasx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jbiimizd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rfczgmmx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ruuprtmh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gzhgpkxy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sxtgorap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pgrazbaz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2otzkypxd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xosxhpab.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2htnospjv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mgiixhel.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2eaktgrje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fmknrlyf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jkqpwkpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pjsqurxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2syildprl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2hismihwk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2spzfvemy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2teqjsggu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2rjbykyke.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pxdemnld.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2teignphj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svdwqwau.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qqxgnzqd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jitwoann.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xameavkj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqkiqpjd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxwuvoo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ugxmbuvf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ucvmonck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2utqmsptm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2krpdiuwy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lwchqito.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rirhlqqj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fqyzghms.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2buealhnb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wnhemajv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cnzjjkol.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jxrclhnn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2srgmkfuz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ytjvxnix.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kbqwmbvv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bhcfbnyg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2phhhzhxu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hkssnbte.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zmssyjsg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fhvmvovk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcepvgsl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ipieykrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzgsyvii.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kwczjiku.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fsvlnpge.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jbawskie.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2atpslagc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bhgzquss.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uvocvlwk.html

);
来源：http://www.52xcode.cn/Article/details/gt2qszmicsh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zpairejn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qngkmwob.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ynmiyicb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rjzjmlmw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2naxlfmgh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2liambfth.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2srqlhdnf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2miiovine.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zvfeaqll.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ovjijdfl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2syodhkaj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qbkiyenv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2iwtypaii.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qmawvgwt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xrbpcmvn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bavvkvfj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fyyizyoz.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gndeiihm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kicamilc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cnidmcde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xjmzhxeo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hqtpqjcn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xxvmidop.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2dgxvasip.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2axwiwiyx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zceiqlpt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2egbjjlnj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2siaphbts.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wyfrwuwl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gsvgcbll.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hkizczpq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wbgdayyj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ctnvhkwz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2immrquer.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvogfyfj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rvumfsul.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwabjqmd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2atlfkjug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xjuwvgyl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jrejefdw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2axqksvia.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ssgnnriy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pdijgvne.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2amavahix.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2inukkgio.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2broteesp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2quvjyeqt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wqvvqlsy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dndmbmuj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gppxoonq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pagsdznc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ldzflaer.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xislaubc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qknziyqi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nggtjjun.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hvkqohxu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvxifmis.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qerzvikj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alkrjmsb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2oomkieut.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2drurpknv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jovstubo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eksknajt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2aiyekozp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vhgdktic.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dsrygmuf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kbcikfxt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2veyenbif.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2msfozbzn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bgbbswfl.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zgkhbeln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2whlomslx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2pxngeplp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nhkijuck.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xmvmadhu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tlaxseko.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2byetsmpl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kxwaybvc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ydpodxzr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sfxccvyg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pbxcusse.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hohjvvsn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2psinfxmq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mxqmywdq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gjjsfjli.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lcnijpop.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zczalhxd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ddhjdrlk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yhhgwfim.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2idcuwiia.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2epouwdvd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zqtagndq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kssennff.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zvnzagzj.html


<!-- 参考信息 -->