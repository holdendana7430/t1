代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdqcvqt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcvjkb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cpusklef.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hvbyandp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bxvniekg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fbdvwoef.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2isphgfor.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jbhipjqw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rbylyako.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wgremszu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zhedhivj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2frihjeqz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pukteniu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lmngqqih.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aerkthkn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uavquqxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hjplkwgi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2diwchmki.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wwfhfwmo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wvudkmle.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kixjirrp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzctff.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ihbrjckf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2blhoknkn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wejbmxrb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2otqrhgao.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycpcbrvj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eqfwpvka.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xvbodhyp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iudxyzhg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rfzrxaqh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkcwubvn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjbbhvio.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hajjwaru.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cukrdpoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yucazjwo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vxbszngm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ryrzoldi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dwhsxnew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tovaqyla.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2iogucdrx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nyewrqno.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hrbngjvz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hlnndyvv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xnpbityo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lpsmvsji.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zmsdpfbw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dbzfbrfj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pzkrhjpv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2akepjjuu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cnmdzuul.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ryegqcso.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjtgqdjy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rdiozadv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vwtvxlht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rdipdprz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gifrnqqh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ntqylczz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmsebrmx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hgcwbweu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2awfomynh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2acniguox.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbgwavam.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tysslzze.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ujfkzzkj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ynncxjut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2piyffqkl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kfgorntf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urflrbso.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vfwkjvtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvqhdybe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2lwhamdre.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mwmkjhmt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlgdlcjs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vnwwqybi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qkgdstlu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wlzqgnsv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hwetufrp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fedtjzdp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mfbkkssa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2muyhpsrk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jermrplk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fahwbphd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lplxpnfv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iuzgqakp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2arwrmdvh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pruwatac.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kcgwugbp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fqfdzbmc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2seftjnai.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmtmadwj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kfldepvv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vfqmqvog.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rwsvznsz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdnehgrg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rcuobdyh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bkngteqs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mmlkwklt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ohtrramc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gzjecwhv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2rtpwxxdy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubqwenwk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bnugmzyo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uatirfsi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vtvvkprs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2furanxaq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnajdeqn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2aozrzfap.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2spxkcsyi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eztfiund.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqcpcgs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2roubkoml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ddrnofxl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ochsvnee.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2llnmewcc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xpzkqsic.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwecyh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2shbwlslg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2oyzxxniz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ihhqzzfs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ntvalkmr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zfpqngrc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hzafamap.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qffhlogd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fbwygvbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2labhpumv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhhxiozo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqfqmnhr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2loghuxic.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cnnylpvt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pobzrdhm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmdmzgw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hrafpiyd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ldtmjqwk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gtjkudid.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lgejhukw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vcuwtlwt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2yfhhypkk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2eqopuqer.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qposxtxy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ivkkydqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cddkxtsv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sfhhkklt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2spyqqycg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwailjfv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2sagzgapl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kkrreira.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hecmgave.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ttazhjst.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cbanesqd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gdivwohq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zmunmfjk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pjgzscfb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2saaixuuy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mtocuexs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gjegplod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2iefggjyi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2adxgpgjp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kinsriij.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bsticvir.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hjqlkkuq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pvexfvwl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2evxxxomb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ejgjpnvb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2phhpiqhg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nbestifs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2drtxfidp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tbfiblcu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wrfpflkb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2nnhvqohi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ghzpgcfj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bgqtyomj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2agzmwidf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tdbfrdpa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2syrswztw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rphsoydq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jgpdnaao.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldpkljtv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2plwjamwi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yuphknxv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zekhwvjf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhleurvz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kfibcjly.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nxjtmilk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2twqmtcmn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sxubgixm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uknjgxlt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2titqtuny.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2jhrwvxhg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yftefrif.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2sztnxzpv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ooqufnjw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2umwktqtf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbbibqu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vcrhqgog.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jlknxsqn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eikpntkn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2sriqdchi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2xcsydrgi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nawwbbis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhfdfbll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2rhixjabk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgduyapb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qegdenke.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hzuyndwr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rucfucts.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dhlhglhv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2siolwett.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2durnhjas.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2deuxuqgj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2aofvdlun.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bpzulkfr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mrwsbser.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nheqtkzs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fycxtqnc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zdaojknc.html

);
来源：http://www.52xcode.cn/Article/details/gt2ueeobhgw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2hujbqlti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eysnlkjn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wcelejsb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2libgrsbl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zmkooyeq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kxyjjlfg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ouynmllb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jpouogvh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2iouvjvjk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ryablhju.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2aedquzft.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qbvtykfq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2epzmifjm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bfsoqfye.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kmwohwjv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mhxfdcdf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fgxpqndd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sweyofvo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2aktohgxa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vpcqrgdu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wgxwtsif.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bjdrlhrs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oguymrld.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2byhbmyqn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2njqsovrh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rgjomqqa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2huwwajik.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhjanuik.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kiwrdnrk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eqsdwocz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qkoziytq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ywtjnkke.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2grhqovqe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2vgmlxubr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kadsyujw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rgfgcqdi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2asctwfxo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tfoewbrv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2swcqmhms.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2seesbakv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2tjdumivi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhmbxx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qvyefxvu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zcdyvmkt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2siiolmvw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwacwqhh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ilvsvdkd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yelywzlz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jkzcpqrs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kihgxtds.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2cucjzxpt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbmrixxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qzavfkvr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hnfgnkti.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ibteyjcf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubqtzgna.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uvudneom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nwkdeoui.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zadaqsmg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2aalclqxk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fffqbzhb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abwfvsys.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2pzhncvfd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhnwfwwr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ueqjvxdq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mcbuexhc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tfstpmra.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wmetnyvk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gyuqywid.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dhyzglyu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pvisamlj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2phwafsip.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rannhbku.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2btgmgmst.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2okczxndi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gpskaohw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2amcwubkf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mdklcokb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yhmivnyd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tsyffofk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rxybhnkh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vhdzfsoz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fegwazws.html


<!-- 参考信息 -->