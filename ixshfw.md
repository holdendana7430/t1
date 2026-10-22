代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2detxhooc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bptyywhq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjncokf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gwmwjfpr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2taaqyftl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tqfpxkmm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnudyuj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dcwhxhns.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2riwfdxzd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hfntauua.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2frrknfmr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qitslppi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qtcvxpgx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzezrvoq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mktbmmen.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ktjnmpkg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mibobmng.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jzneynik.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2veufnsdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ovjlzayl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ajaiynah.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lbfteawd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sqiwwdrr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ofsvaamo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2micebkke.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rylywsgp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2oglctlpx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ovoztlmn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ushqpsah.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fxukkbvz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssflrgrf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dofhwhpr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uxxfesjb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jwsjjpas.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cwkwbbjh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nuhptioo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yqoikqzt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xputcpfk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mvcgzayt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2odjanvjn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2blrdefdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fdiubnis.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bmxtcobo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2swdenrxv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qgexuxxh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xexyqkrr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2iojfylbz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lpcogfep.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2depflpmg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yvxszrga.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmutigml.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2weugzqbe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2modtmguo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tnbqtoqr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qjrpmxzr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2geqgfqpn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2twooyzhr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dlphcfzz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zvjdrvol.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nvtygvxw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bejxptot.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ceqverye.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tyqdqqwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ngugdmvh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vktstezl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ufeataqe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqocsy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vhlcnzng.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jzcolxva.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jfitrfvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kqbjnzrf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rggjfwhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ievaymho.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nuiokiyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlumhfyk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tdlloaqg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yeclrgbl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2coqdvtkm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dhosqkem.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jrubhaky.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2aqzvzweg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bcqidain.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2asnnzpif.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qigepfqr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dwnzeqww.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bawrfjdu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2afeewkpq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bofgkpbt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mxyaegyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jpdzowqg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mhfpjyyg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uaovnqio.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2diqldeen.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nvzeknks.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gaulitjp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2garsaycz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jzvghtqi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rjwoigde.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iybqkvug.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yeaqcqkq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2byhnnrkb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2znnufcaj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qmozsvem.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xdhyrmle.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lyworzac.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hihhaqui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jbuzings.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zrtvhdye.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2susxkfwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qbmjzklc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xhdjpupz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jtauiahd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtrqwzq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sqwtyndt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nwpdfipd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fuxtqepa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hsdudybo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hgcdesye.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dgsldcvw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cqntwtbz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kszrtoff.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2otybhnoz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqmrxvkt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vhktfbaq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2odhrppij.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fxfujjda.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2mmnhfhiu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gyntzfmq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yxithdhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htnjvahg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzelqqda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akosgmph.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mmmhdeln.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nbepgbmp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aquaacpy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nfjvvxfk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jpiuwnwz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zxrmdydl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2htmsknwy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2knubkcpn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2waotqjwa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2idtvilyx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2btxggxgk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2enhatzlm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yvpluzqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hamqsqpq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jclagrum.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hphfoojo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzausarz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mhxgdjou.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nnmyjzfu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2emzucakm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pjcymvnt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lgflsars.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkpcynro.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ueizyvuc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dmmykwjk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwnypxcg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ihgpitfk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fxcdlkyk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qdymguhc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2blnnlcia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pyetcoci.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zzmalgdw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mmoxybvl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zirjgvuw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2zekwyxcf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ywjkulao.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iztwcwnt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nzgrybwv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ihmruzyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zkfwdgme.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cavktmgk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hyqzffbn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bwgntfzd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jdhjaoln.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jteyofky.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yxqngecg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bnwoxyhm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2erjoholi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2tyaknppw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owfmcdau.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zsmiwyct.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2youpimlq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lqncwtfe.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xotpgfrc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mcivfecx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2sygdwyxa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vxhcuaxw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2txplfdro.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pbjsqkym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbkegoqb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2odtziqvh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vahdqudo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2uysugojy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2krmqcuxz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmebsfr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pyiazhxv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yyhsajvb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdkiyjw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ptccdrob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jzoijyhk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzsusx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2iljrlxbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsmuyxof.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lmybmmnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjcdgbxu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xpzlwoiq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nhyulyia.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2auflrsro.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wzdydgje.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vflvabvi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pgusjjmh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fxpdllqo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rdbwoxiq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2opjkpmcp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2alcuclfz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jelaaztc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mwrbypvs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2edozhlxg.html

);
来源：http://www.52xcode.cn/Article/details/gt2thyhljlb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yfwmdyzh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vzczmula.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2djvhafsl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2virezrug.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pxsyyppv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2amjkrcaa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xlvnlyqg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2zqcshzzw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vwyomcbc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2oqhrqotk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mmkmyhml.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2krkwqcnd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oimxkslv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ynajejii.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2brvbmfco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lawxwcgy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ptpwkeay.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sdmjkjhv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cogoqcpd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lnftiyxk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ciatsmdh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kzwpuhem.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tquhtkfs.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2paqudmxs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ouzcgaxf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fzxtohpi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2hwrymcvo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tblcdpkp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vukamjgb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkjcpr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dtjouwtr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwufgicd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbcnlbdi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2clgbtjcc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2zzjfkxiu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqabzhn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2azybzhcr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bqolskpk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zpnwfrmu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2misjfcnv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwrlrgef.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbvazx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tgjhxuux.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kcsldglh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mwqjowva.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxkqgptf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kxxgvtbu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eviyrwlc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vbmuahug.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ojcoymol.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qzyzkdfk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwpasxht.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xinvmrwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrpacspt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qtzhsjrd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sixvdqun.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vdcjbtkf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xbdcsvhg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lhnaqazq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ksjrdsnn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dxalrufh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ritabzxu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2apdwsxgk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kvwxtemb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zeqjsidw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wvrsqeii.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cmckfejm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kwfswdui.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sofimjmw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zcclccct.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mositvqm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wvpufuwx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sujtobsh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2miqfdopz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgztmu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qxwzacyj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gdgnezsh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ghaywnxi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2edhqrjel.html


<!-- 参考信息 -->