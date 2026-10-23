代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pihitqsy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3arytzeru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kzgmbqun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cfecqske.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aagkiohr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3styfsgnu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3egmaoagf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbbodjdq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3suzqinlc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tdytwvck.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxvopzlw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3buxajadd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjoqppsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uvwnunex.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bxoiflrm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3iekzmxtp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nbvzvdjr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jpptspjs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xcrkzmbw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3oedlntbx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zfzznbhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3enaynxxa.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lxyxfzlm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kvubowwa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3iyljdika.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fkcbomkp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qovgmgax.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zzfvzlsa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zevmgwmt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tlditfeu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oigzgcgs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycxbbssl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bzashbjm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bijhtrzd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3guzyptzd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pjpxbrwa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqimvi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vxqhhfyo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqgggpjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iqnrtswz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kuowvipg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3krqarmze.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qfuksiqw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3epyixjzu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dbnjlwvl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3haockgut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hokuhadl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lnuhzftn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3btbftwft.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3imykqfuc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3idftrcnv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3smlcbndp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpmjnvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlfqtnxo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wevikzco.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kljtaedf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cldysaxa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uljxqyfz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bfppksfb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsmojiyk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zyrnnehb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3erjhlkfy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3odhnawmb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sppipven.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nqihckhs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3czadydmr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zrmpmktv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nboknlui.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vwsllybh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xhhbaouw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ljapzols.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pnyhjbfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcztiiiv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xqxuulag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrdzyhaq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fqektaxu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nnawekok.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tpodbwnl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ubpytmhh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kgmjrxav.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vapvcnle.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wveajhrf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rcfxwjll.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3glbvloex.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uuegntuh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yzwcirul.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3manfinbp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rtpxhzun.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ykepcumv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fghawvke.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3igkxbvgy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rhdkuupd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3oogfreqb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jntlhelp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecvsxbrg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lzypcjox.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hasirlvw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pqqilpel.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3phoyromw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zvowvnhn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ggjmfncn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afyewnut.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ifdzheeu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3muznwung.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tmherafz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jjsqznmq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzylxlwc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xhzahofr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3thozxffn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dojrhtcc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ijxdbimy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3asbpwhid.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xgmkqvfj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zddtyodf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iimwfpuh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jtuckqck.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fdjpglvl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hmzpwzap.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxnscri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qlllafzz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xltxlwyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vudnnlip.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3neeulovb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mixxbnut.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3atpxmyfn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gxegkaet.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3halilbsc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dvattcad.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ogiwmfqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spunpdto.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qouyajvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqfwuooy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ppzmjrft.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qtwgcroq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ctgeazty.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qbzdizux.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xzqkclog.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nlikulvl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ugonrcel.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qayzanou.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3owqxujug.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tznysvmq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rlfziibh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3epbafpyl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3krqdqeai.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwapxc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yglgsvag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xpzkuplm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rzjcspaj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rerhedjp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3thtlkwvi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nesxkkva.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dljonrdp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgfcdidg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rhvjhgyq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nottjput.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vgfrvvfn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrsnkdt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3enznfciu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lbhigzgi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ojrjtbpr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yzhebvhq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tpxfrmko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uxculqtw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rpxierag.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pbshyvzg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pbwgegge.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxjjheul.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3znbmwidq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xpolwwtd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3iuejveio.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cvfxrean.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fveymacc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qoxxxgcl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3odleellk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qngjdykc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3gybiynuz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qifqpsyn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lxhnjbyg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xapshrmu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fxtxhnrq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzfqogmf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yxsqgwiv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghnwvidt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ozgcqlfr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xjlyerua.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3phfmtooy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3irvzldnq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ayokqxas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qkvkpgba.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rtvrapym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaqcgnwj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3smvdbvot.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jbloxwxv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3abnuzufx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qvvyumvb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ykngbghu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jckedyrg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zvqjoula.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwhzvvk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3srpsqfvv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ihtvuyrk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3rmzwsncz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3prebizvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khyxwqoe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hlyomzxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iduswarg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fowlawkc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3tnvzgpip.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3odyrclls.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ounptkvx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ytnkhsnq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nbxxzebf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kbaeyzku.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ywtuyqfx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mvfblcjh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gbreyken.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tqjukyzg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hfbskmif.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wigtfpev.html

);
来源：http://www.52xcode.cn/Article/details/gt3iavjvlvb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uimwjpnx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3htwnzjob.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3becjbqou.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ejcjupxz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pyutzelg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ikggfohm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jsozrpgw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ugacvika.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gwjtwhud.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3temtansm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3adovmzmb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3atjbkdfh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zfwfuldq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fiaibjmd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ejnrbnbg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bdesllig.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cdluksnc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wiunfuoi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vvdgzahs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fgicgcyv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ylnduezi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3kwkwhafy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wrypgovr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xvxeafmv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3uwdsqwje.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dblzgvko.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3otmwlyiv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bspkprsz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fxofisre.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tyfvpmux.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jsxszyjc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3futxhbrr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wetlcpqd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mikfjjjo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vmiixwww.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3herwfewn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ncvymwyl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xphqlmgi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3djapbvca.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gyynugtj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jqhlgxjs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmyayka.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3najjhmzt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gosswxlg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hopfmhjc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfizxhre.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qfazxhgl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rsdvamlo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3acysvxlg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkmtmjqh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3wccfsdbe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jeefrwrh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3smmthobn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fvgczdua.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xnuewpkj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxjfvahq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3umdzxemd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mfpfwoue.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3inguwwft.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3eotgxpbz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3amxgfkhr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cebisjmj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zgorvzdg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gszzezbb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zkiqzkje.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jmchefde.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jabpeepw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hozfaccu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3azgyekwz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mpnyavmn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mobkuygd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyeway.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ygdgsgsh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3chsujapl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxhfrly.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zfkhjrhw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3betbfexv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kxakpndy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nunzlrsf.html


<!-- 参考信息 -->