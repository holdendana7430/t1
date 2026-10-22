代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrxtqwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dcxhgmir.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2sdrjyrjo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxabwtg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yateppum.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lgqoqden.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tefksfva.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ndgboojm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ezuhoymt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ygeohbid.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2plvkcoex.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2huuyxpox.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2detqomvj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qwqrkwfd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hwzojlgs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pbdvucvz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zckyjjxa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tfvvdftu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2spxpvikz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mkyladoj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pcgltcbg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ieaandlp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tpgmbokm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ynvjmomj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmxiahow.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bymndvrb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aatjgpvz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mmflpgkt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kdbyksdy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2brqsdjhh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2axbyzfom.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vxtgmvhc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbphlrzj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ayzoibdq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xukcfdld.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uwjajldr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mrdwbmml.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsnnetbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2llfmqmeb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rrbklrqx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jzzngezp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bmxsaldz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xkktcijz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2txotnave.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gvmdlbhg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2oqpwuvib.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kinpguuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmjkvlt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqvjnhd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mougkfbz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njnpjlgx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nymlvtmd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2selwlmsm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yicznlar.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kfpngnkc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lavnzygz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ywvftoua.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2slhpqsqi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2guxmecqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2thujzrsb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pidvxgfd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2selhxhxx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vvyqanql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ketknwia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xboczavk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cvqlromy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqlftz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ktsccoqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfcmipwc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ftzyjijj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bditephb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtmtxp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2swekxtea.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ammrzffl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jnqocqjz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vqqjtaqc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2fpagjulu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jqauxshd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kabcxzdw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qdkpjzll.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2enxhxzms.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2egacwizf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2eslbritv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ygddzccm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fowpourq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2phlxsxmj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sidfvkhz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rsbciprr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2unjlaotx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pqopdmiy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sqlxljpv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2iahocxhw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cekyicta.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nodwdppz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qmwvkyup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yckmdbjz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qxepragq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdyiwu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2apefjmvm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2whtjwpjy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xwruuvii.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2torkrhxr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzscvck.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lzfdynoi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yoxeegbm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2otcnkqgd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kutcoaxd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xmkhmlom.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rnxysqok.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2banzxorh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ylsgelqd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fkopontj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xlnvybvu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pnuvtepc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2skpvhvvz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmruotme.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zzipjwta.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nfyqepyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kggfraca.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bbuwjhxi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sjtgjopo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qtfzqckt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tjtavegv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lywbljvk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2durmbzhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loeoumkb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tkdhcugj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbeenevi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kmjxwqea.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2sjuqujea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mfbllmzd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jzmpmlcu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zgpreiyi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ycuupiim.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xfjjmcde.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2gjvhdhhj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wjiitksv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bqkmxjrc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lndwbzsd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srnjcaok.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jbdjerlh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ohfdbwrl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xktmtxrb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ckigvwdt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tsxjhbxu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2upvifhiy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vgutxwal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cajocgbb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lepnusim.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svpksogg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ubgrkxwi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2evzkxlks.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lagjfolx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gotoklna.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2utcavcdz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2glspngcu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fsmnpmzh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xwcihmwm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dwdjhtfa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ojwdtamr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oameffkj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzjbzbt.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ntbpyvye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2avkbcusj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2uaqvhrvr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ywopzbem.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nihrrdxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2piyadmng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhjddrws.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jlkigeye.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wmbyiaof.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zyejitrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2waalsbad.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xcfxggmd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2egzchsoa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unblvntk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2yovxubov.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dhpphgkh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uxyqlkgu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2okthdrny.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2amdqetgg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gdpjrfgs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2whwbxtql.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hanrciqb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kwitlpwu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ezhgdicn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xzdnpqeu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oslgvsts.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dskvtlfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xdsbqxsp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2iwrgtpbv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zfordyfh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2beoghgfz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ujtirbjf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kywmvich.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgjugge.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2omlvrghn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lgcdxbra.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dmgctlwt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2btjozcec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yscuvsfu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yzsnjftq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oudtxegu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yeyyphwh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zjzvioam.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hxaejqgp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zofepzmt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qpepsbit.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2jionofbz.html

);
来源：http://www.52xcode.cn/Article/details/gt2amzqarho.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vktrohbj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xeqlwjin.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aopkicjd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zrftunwb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2zyualchr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdrpxbd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wksjdhgt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ntnmxmgf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wzgzdnzc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2chiwiddv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2idccmwjb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2lhgmsbic.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2frlidtxr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2veoxmnss.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fyqpzxek.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2loqbdeek.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pptchobn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yknkdzzu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2luumxciw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wiextqdh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2uyufkddz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hhtsmwjj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jjcfeqbb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lccagyrg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rmekhght.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2icozhrum.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tgsvtpzc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zonxlhdv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mypybskp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gxhlvduf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2slntdkrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vjxykwzv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2auyzryuy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2obrsgpcz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjifgunk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tdztrjfo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zevsjkwi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2niajezzc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2awpypbic.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2apzxoemj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2yjmvyjzm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qwyuocjo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jmdbspsl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2mfrbswdd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vhheadmf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2awxvsqix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ylbuwecd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rhddzcds.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jeabgfzg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nldfbulx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2iazqwnwn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jtyzeujz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqrzgpax.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iyvdzpen.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qsadnvut.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gghvxjbl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qceffqsp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vsvbyydm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2maopazmc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fliunnvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fdkgpavf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gfukeoeh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjkasasb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2eptntqrr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wcuvzqfr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nqpmmetj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bjqwcxcb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uxfwwjii.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vhbdcevs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hpywrpkn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dluknuha.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jtrpxdpa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2prjasvft.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nbeaojcq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jyevqukp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uljdjdim.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sxzvjqfd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2togkwgce.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqoyxlma.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rahrxgte.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qggfhasy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2euqirwga.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kvlfdvvd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhbgwagz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2suupnasp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nhksljat.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2btiojzoq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jynprnwc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wrtkisqs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wsuzegns.html


<!-- 参考信息 -->