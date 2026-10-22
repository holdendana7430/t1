代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxpqeixd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2utlhvhya.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lxylejem.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ozjtvkco.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wnoeukpt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iltjflao.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hiakxlcl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kekubpao.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qrplvzga.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wtwxkmop.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhjjofwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xcilysfm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kefigffa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yivaamhn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2obahzuil.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpqcpyz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2condvddl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgucxftc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yfydcsmg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ztmdlhmi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lamtnhbj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydzrsngk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hcfqwwto.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hdeewggo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qkzuvnoz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bpdqfesb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zegrmbht.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xujqidkk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2czeuvrpg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2foplazti.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ipbtwmzs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zgcbsrat.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dmbbvmjn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2iryiznbt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uzopozah.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qwgnavbz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jadntpgy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2cvxgscqr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rajlabee.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2icvawtyr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hduaxaxs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hcqxlyna.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2setegwpz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jxiyhlww.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ostmpquy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sdsznwyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aipcqwuo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iesfeeuw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rdhuspzy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tjommxbr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ccuuteum.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2opfefvab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yisyevoa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qbmmqprg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gjhbgjgg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2isrrzhsq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2euvuxyla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2inrotnap.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oouvtuie.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2abzldxrz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uykorhci.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxquonk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lqwnhpwf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rcwtjsjo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvxfjpfg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2amfvuhxq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2shjzgtzp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uzgkebln.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wxyarrml.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rgdnzujq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zocwljfc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ivvowhmj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pfgsxcxs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rjqbbmyf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sqphrbqw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qzickleo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mbujqbay.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yfflluxa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvwihvnm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bvjqnsol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xglxmats.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dlzsolxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgstvbft.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xtbyygkb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dzglgdvu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dikmixci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lwnlpeca.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qlwhmonj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pebhdmdl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ohnsvvjv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zkqewpot.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qqtiwvnw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2svaekrtw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tehymytp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hrsjgoqw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zhepselk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fvzfewds.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2biazluqn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ybhrafcb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xtrhxjxo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nsjfdyqx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dczbshsn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nbrovxab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nyjrpiqm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2owybvfao.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tjqwdtxr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fxlnuifz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pbaagagh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fbrkqhzu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlubwmdq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hzsotetg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nogbrrjz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gnrqujir.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pslbxmfj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2blobavzh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jectcpsa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wijztkxo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kjcrmwwq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofmoucww.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cdqxjaxn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpmucmr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2odksyboo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nwdejhxx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxepsyl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2iothlttb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2peivaask.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ngfwvmgk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqdbxrsj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2whmnepzl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ssjcxjdr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2aqwdzxmt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jopcptjh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2utrjujic.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2waankfeg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yasziglp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2cbelskwr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zvsnsgke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irvioqqb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhxciiwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idcoocvu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2movwhcdd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2odcauqwi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2anjmgwzv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uhgdcuzi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jwzjfzha.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hdyewjky.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2znvjuqbx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2zajqksme.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zuvzoqhq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2awfjtpxo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zrdidzze.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2arjbxfcr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2aqmngptq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2eztvwiyc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxpjgac.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ksqobdas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2weygcflb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kwkomnsr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgqwyfgo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zkargrau.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2iwmgvwrw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uvannfjz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bzcsbaes.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2enaxqmma.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rszzidka.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2iyymlqkj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hektkmlq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqniqvxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2srlbjdip.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eixqmjgg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pppoijyx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lnmpyvgq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2urzewsqa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2eeacbgmq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bjlcwjlw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jvhqkxhe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ptqshdba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2iwhcoljn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yyijwtch.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xyqewzry.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rtyvnryv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pkvaghti.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhcoykz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pyjyezdt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qemzvtsf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2umzydqag.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ngfipqsm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocswaoeb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2orrmwnka.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dsbvocfo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hmqlffvu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmxxspxs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xnhbxxax.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bnvklawc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zzsbzuai.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tmjxcxcv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jsbqgzpd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ahqgpnxc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mkvnnmjg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yrerkkqs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2wugnqsov.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vfareuza.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nglvrkcv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wndiefdp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvpilnr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjhyfgg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dfzcizos.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjgekyb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jinawjec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ckuatwwg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2npypkjxb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wsnwwwyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkkojcet.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kifdlbck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpevitqo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zjnscgoq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hoxmwhfx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ebxydahc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ymdlcfix.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fykiijyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dmhlbznc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jbtqavmp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gsnfmqnk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dncrfcyb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xgqbkjyi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tgoxodqr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hjmsubwk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fdiqnuse.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eiaqchlz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hfnvlbrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zkawdnns.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2njwlqvlj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qnrycwhv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2celjcwbi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jaymbteq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jlzqprov.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2sbhlkrlq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kfudgoaw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bkrbzznx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rhlxqxjx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2optnfcxl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cwqxmqqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2emrnpxcb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nfsmmdnh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ffdfmven.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nieykbxl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzwqfp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hctcfitk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hevmeyph.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hoxkhcnn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dspprjsi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qipmkvyj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gmombboh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kbpswwah.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ryaublhj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gaxgztir.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmljgoku.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2segzzhfs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shceehch.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xcqmjlfr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdigeohk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ceipxane.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zevaancb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jxixsvyd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2adginugk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jhetjtgt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oqmembpn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pipmtwqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qlhggghh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lbyllncn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2snicdmyc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2aqulwpjm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bmbhkcdv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hlvzyxsf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcbkcwta.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bjqptjwp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nqbzhsww.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2iwxniudm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2poumxtsw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jawlbijf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nipdbtak.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jrnmpezt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2etukpiin.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2duekaspx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yveabtci.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bfvkwzot.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnxxqu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dxlthrzk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qdabnelt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hepksmyh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hndywppr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2eeclfxzn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bmzcrcwh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jpkxcxmt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xekugrjo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2badqsfzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bhzyqmgl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jqbockpo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hnnysrqp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmvzahxj.html


<!-- 参考信息 -->