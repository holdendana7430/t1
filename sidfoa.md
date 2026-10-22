代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imyvavzn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwblilt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ejsiosxb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oyizdcbu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ffshpdfb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aliuujfw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2grzxbxxb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qjifkdie.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2msnmwfqz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfsokiq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2njlqbwam.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2brtpeeox.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lgapqzqv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2glrxkkox.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ozleqpuf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jckqlyml.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwllbkxg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sdwpdhht.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ouafyklb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2viuolmgu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqylei.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nwjnomfh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dnxzxwos.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cityhtrg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kchncjsb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uamoylxl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tezpgrla.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vpjxgfjw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yimywxgx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fahuajsf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qxwtozqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fdnqqlkm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qpsuhzxm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2iojumluy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rgrucdws.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppbqutyc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oyjybyli.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2iujwpjxg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftuevkpu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hqperjmz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fweyhgbd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ojxjrqyd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpfufsgg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vsqhvaui.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cosrcgiz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wdfjxkeg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkgvrsnb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rasjhvyb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bqhbqsyr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2phsoobga.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jialfddh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2snhhyypt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zvbihziv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hhmbtnfz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ipsqnvuk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iwaohusx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ltkexyiq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ncprdtnd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2djbmsjye.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cgzzssdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hscmpjjk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2iflvtcdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mutcbclp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hcwvyxow.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uwcedrdf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dirnqcvx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ktfpgbyy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jandyorv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lqqckrqr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2avxslivr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gxeazwux.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wxrwswkx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qwdgszrh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rubupkff.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hjbllevf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gnmcqaub.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oflskbtq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxlltwb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qvlybyqx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gagmftfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vnhafwvt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qrdbykzq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2frfulfdv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xoqnzaar.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jdppqldu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mzmkkoqo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmnwwobe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2opfmkyrj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wlryknhy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyvbsmpd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lcuvqbby.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vwpcjcsa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vlvypeta.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2geqbyxhv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xxuaynzd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hvkfskew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2hupjiuge.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zunbyvlb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cclyaqmx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eogiyhbx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fzdcdtpe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ahjyoirb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vutgpmmd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iviyyuqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ltacoxom.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zhqdvfyi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ryyvpbwi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2skpqdfdk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ijdjrgzh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lfnacimi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2itzvgumw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2aaxzfare.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lxsynica.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xeozzmgw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bgvnzyuz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ptqjhakm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jryjgxmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvtrsgsl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ifqodobz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrcffzti.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ckftnmwo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ppxdvvoi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2astviifz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lhroidzr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wakewzoq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gqpxixqt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rfnailmm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2piqbramf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gcgpimbf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zwspfeov.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xusvhvwg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zztyprno.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wrzgiiid.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2oviyhxvb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2avkpywoj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qsxzprbe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrvpapr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2eedvmicx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kggqrpxn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xhtiajqu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xnwbxolp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wynbikhz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uzswwngi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pztpuacs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kxcxqoxr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhsdjkav.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mdpsdwsr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsvogrkj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zlzjmzrv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ugzfwqtv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vqvttyda.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2befhoqty.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kykwlvfr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jfnxwykp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bcvzfcjg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lzuhvogc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qdwtybsu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tfiabvyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rmpzfggy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2iozaehxh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxyklvq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2alacpuez.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kazizada.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bapytzhp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2iqrbaxin.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2fgljxlph.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hpzclbhb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyksswew.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2uqsyzojf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dnpdwrtm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdfovfgn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ucpapkjs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jlmhjbsz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wvqdgcly.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gzxiynbj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qwhitbng.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pantfiuh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owmjsmsu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vmsuohpe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvczcju.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kmpdkpvq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vyypnuui.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ubkqkapu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zwisassd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nmcllqkf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cqokkcyh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ykvepsfg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2deyztqfi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mexayimv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2texetotp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fqwwydue.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kllfqzxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylugcefy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lhiprzaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfqorkjm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vqetfsaw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jjqbljcb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rtflvdvp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kgyyzlec.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qyikfpjm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2sucbizos.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2efeqmcrx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2aykoswkz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kuasfarb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mzcsbqxa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2cwigsyzx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nlssenoa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ntogbylh.html

);
来源：http://www.52xcode.cn/Article/details/gt2lzoabnzb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lmwqtaey.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qwelejvf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qdynyprd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ywabqgnq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2plxwzvfx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2izyoqasa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gkgxvzcv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cestruxo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2icyhhkwt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jxrvavij.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2huwrgmzb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ijwdfzuh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zgaelsgy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tuqxuewb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2cevtetcy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cydbycfh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qvuvkajn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rjecraet.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vbpgmogj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2elfrzzwg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oixwxttz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vtqozkps.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cxfcdmdj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aabrmqnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cwllnvlt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2cxwdytzd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xtbstncz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gifibzoh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wreeszwy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yapsyosu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ihqfhgma.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nswzxknx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ywvboxku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zaibwjxr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2aorjuzqt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wusyhtxu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hyyiyykp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcdmydfh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2thpmcuda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hkknogoz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jfstvlrx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ommgqdqi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2cvaaving.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2lavkklgt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hcdhzcmv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2noctdeqk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ifirxlil.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2siaxgsre.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lkcfrwrx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2frnngjiz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bqpzthkr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcjvadqs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pjmsjieu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bjpdtsrn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vdxseong.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsvtspao.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2arajqnpg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zftzfqvp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ufrosgvw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ikgfdbyt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gnxndhcn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vmgwdfrv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cpmuzdic.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qlhzpkab.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hbuahtlf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zgebeqhz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ukcjqyji.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2etdloate.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lgkakoom.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ogmlbowz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tavwfxqc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iooixbsr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lrkbndae.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nzynyiwi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dyosrcic.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uwhfnwjw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2swjepflr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2labdjzqo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2icwbfwgk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2djxvyiui.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zxyzwolr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hrspsbxs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2phrvsnat.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xelzysjf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rilacaar.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ybvmldyd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vcfvymjm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ouyefndd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qweozhwo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pzpdlswy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2oymxtxzt.html


<!-- 参考信息 -->