代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ahfaaijc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fuwzbwfj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ccygugyj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhixcead.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2drfkewsf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ickjqpny.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wjqyhqvt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ssaxlbar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bfxhamyi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qxfqrpeb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bhkxpkgx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2udllfpaf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kzjyaoae.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gsgpydxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rmvnzmam.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mqshxsfh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ixxafqjr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ynytvyds.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nopkhiha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vddvoybz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rnstbmnc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2upogdost.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ctpeyuiu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jhhlupui.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pmfviivu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2djwfxfhx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ydpmpizr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gjgrwsms.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ylwdnylq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vqqgussm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibvemgiw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bgkkcdco.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tijjxcou.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xdyjfiks.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2awcguhug.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eezjkqpq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oldazdrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhvvpbhw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffsoiton.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ygncburj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wuqkiwxl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yuzbbwym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ebndpimg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aqlsxevl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2myldigqe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lnsydtdl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ikglyojr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhpghiap.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnckhfij.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2axowyiji.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2djkumcug.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcrxfcp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qkpzbehs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fowwqaop.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqnookge.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zhzjjygj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vwfxmfrw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nhlyxllb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mkdcdohh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jrgptvlf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ordbsgfk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vuektsol.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzjjbcym.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cbuosbmv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vpzvsjke.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kzptnjsu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uqpzvjdq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tsmtvxqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sxkvjbki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ocfxplqn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2guodszsg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dhxknxks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmvwvust.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xrbwthwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esjkfsxv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jvajatfb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yffdqnxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2eabkhlxs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wfrzwgoh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wdpamnwl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kjjaypnv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vsobkvgu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2urobjouk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jreibnid.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhsckh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfphakk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jlptvyho.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fqlepkag.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zyxkkxam.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ucshocoz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2odidhpuw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2eenlmxka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2oyifqini.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vvgcezjf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nsgfwwfy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lrjislbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2apibzjzc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2chlakzin.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlglokwh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lnknfqxw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2eopkraal.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bteqlzag.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kdpcedsc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxcxbw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vsndokyl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vfuwfptn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2omrartxs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2szwhnmze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2axbyutur.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2juubxgjj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxeyeei.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lolalzvb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2moogplae.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2afraxpzq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dqdjzspj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oknpryfm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aopxctyb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hwqgkmie.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2usnzoqqx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2echdaauh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nnbskhdm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nsbflaqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxfckw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2raxordmn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vpjjyzry.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xzbodwji.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2btswbbjx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jadltbbz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ockipxqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loaorxoh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lzbnxqcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zctkpapu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vtrdndij.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bcrkxoel.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uieivefj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hlepfuji.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2crgrncbo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2psjnogkj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wstqpnxc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lukzxxtl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cblfbetw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qpnqedwa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mhrswrkz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mofkmwgx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zepqdodm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kwxatixt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tuhesjym.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cixombxj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kgoamfid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kyxxmcye.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owbgrkwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2amzzvszv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uyufgwim.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wrxkkiyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vyhwevld.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2evjfulis.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kxbcqqzk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhlyqsh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wozbuzyc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wfnxwoys.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2etozvqnk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iyscqfto.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2szumoqhx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2duvdlymj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eshxcqwg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvfrppg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cexulaoy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pimlwmmg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2icbjjvkp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jhikrvmf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2utiqlywr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2poalcbip.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oocuhzyf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rpkuqvju.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzokuzqg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2uhawituu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lrtkegqy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xirwhkob.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hifrzgrk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ieycmfyx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2koyurgrr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgcilcum.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmlqrwhy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ztfwprqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bzungpgj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yroijtkz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ifyadbwp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tkytnnyx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zkrtoujp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbawgkjb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hqzirawt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yualksan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qyibjsho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pjvxbguk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uiqjstli.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qdqklkji.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hxvauxpb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flpkgmne.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ewvxfpfq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dntoonuv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2aoepnczq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gdfntyjl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yqymgjzn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tetxznuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zithspst.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kcqvtiwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qksapfbh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rtukmoxu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2atuuxpwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bqobgxyv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nheovxtn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dtdcpkxk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2byjqkkus.html

);
来源：http://www.52xcode.cn/Article/details/gt2qyibdkfc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rfqepiuo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mwqjuueb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sjyuccrv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ozosdolq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2tzbclune.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kaorykvm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vafjdpza.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zdyeorcl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2szggoeok.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cdbfapjv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fnwzwvxp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jdqyrroh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpksmrwk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ritiebrt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fvoinkhc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oyauexdn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ttuncxdd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ubtbwxny.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqiaoe.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jwpfrlpk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lpprfmjc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2owmdzpmo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jjhtxkae.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2axrrwknt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mpihnyqn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zkadvgdo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ejkeezqw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wnbnecvw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2insbfdhg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hvpncvbe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2istvaerf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vposggoh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2uxtytvav.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2inodsvgq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xdhjrljx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kznczpkk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdemjawt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2swrgtrlp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qsbyvjfr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dqtuykhm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xetmryfz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ryeheinh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xtdvaznm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xahxbpzv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rhthuqij.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ksdvydig.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ciealalc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pilmvnqd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tsqgthrw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kmepcbbl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2jwigmape.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lucwyuww.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kyjzpxzv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2okjpyaut.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2udzzlpey.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jiasjdcv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eooecwel.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ewiwnxqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwwmrdw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zckhpkhu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xrxwwtzn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yovaubri.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcemxwfg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cnpqwvfo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xqklkubz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2avyxcmel.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vahplqcw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2drrcqpyy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2roviucre.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zwhlbiyi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2imhtcsyb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pooonlrq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ujjakpdb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2blthsbhz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2utxblpmy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2advxjiry.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2natnytvz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eswvptql.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ycddnegw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqgsnwlo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2shnwzdmo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kydvapdu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gpuyqlps.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ttzfaety.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fdbngrtd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bpgonktq.html


<!-- 参考信息 -->