代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hfewpdad.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2chmbcorx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bonbwdaj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yowkvfha.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2afifildy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nllfhfcn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mngxrenr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jdlbtwyo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rcalwfil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cnagzudb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jepehdbm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2eqdrlzzi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hiagtjzh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lctznsct.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kuisniqf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jjxgwuti.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2guhkhwkf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qiesgnjt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nrvwepix.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ivpklotp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kosihbdu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uxltbwhm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2maxmzaeo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dpkmpkrt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eywfyixr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dphrspct.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqiamzvf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kxhiqyok.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vahunbis.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uuaaatqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2lxzztjin.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dimxivxe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2odfeidfv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jsbubvhb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2sfzvkxge.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pzdzdnaw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxbiyokd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2oklhkdte.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vulsgmed.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2munuyoad.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xudmggtw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2indcajee.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2futamzpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qcxgfzhy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kytozsdl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gabhgpns.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aefrwaoe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rpswqcpl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ikokzodt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2crgsvymn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dvbaftgr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fcjimnya.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hqjlijaw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nkcqckvr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ncjlxywq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2llemlfus.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uldwzarg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wylmbllk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hcylhabt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rorxzduj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnorspjt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nnksyfcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdwrifyy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fzrugema.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bvyxfcxl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wypawqer.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zbdrgczh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kheksbgr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mcxymkzb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ugbtmcrl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bkjqalww.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nksfpomn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jhfufzga.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hearxkit.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2sjovunuv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ldtqvtqw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qyroswse.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hiwhbdcr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nsntncta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nkhqodxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bmnwexeh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2morhfypt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bslogsoz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xbzusrhu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2xwgdeonf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2urozwjrp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2szownmxi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2klkwdffn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmedmwdd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hogrecpb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ledifasf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xhunvymt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pxzijqmt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2yklnqltj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aqjwqkyu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bplpjjaw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ozwnwjht.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dvfqncfs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fnvkhydu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jotegpra.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yisudoon.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rcwueokv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2onrlkicp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2brgvuqtk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yvglwzue.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bhasqtls.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uctfvkyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qpxpbbtt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2chtracck.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fjvqkfkh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfdgdifq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wxigddor.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ebizauuq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cphunbwc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jxozuxtb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ebfeqgqu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zqxcdnqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xazqztaf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2heqwqfhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwwfzzus.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kipqvdsz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kudaezol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rdotzgzk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdbbmb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rwdhbenq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pabdqqbl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxweuv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ydusjpaa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddkkwfyh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2edjwamka.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2szhspjtk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nbzrjbzn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xwdojgsi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pcehdihs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyyuurz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2urxrrbpn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2genphpie.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2seuphfga.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lezmosxl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jchrnxkv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qqqdvmxk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qegmbjig.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2itogtqap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lkehtlxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2frwuqmfu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fwjephen.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ptjqwren.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rxrhacys.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rpdyymrn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hmcmyxja.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cwswmxme.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ngmyjjro.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ascviash.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2sntlpwoe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jkxysgce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qhujrqsi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2vnaoqese.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rgiippcy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2acjacmvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2atkutset.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrzehap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gybzxfec.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtvpelb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qpitqonh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qcfwycbh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ysvlweis.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fcdmxyxv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpyhzqle.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mkyanqex.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2imrkljtk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rjxwblom.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqfoyjrn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2gfqhrqxh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgipfvox.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2sjhbermf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hvwantzg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kanutdkw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2idxkomgs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cdtpldzm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uhpyzoeq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2awcobhom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2klddcdzo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jyrjsbad.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wrhyfnzo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2suwrnlok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tgfvnlyl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tuonnruc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnmrnma.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wwqriuod.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qhkexerl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2laioxucu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zgrjpmjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqhethzc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xegaujgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dawviwuw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2jmuxkufe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2amvsohbd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bkqqkako.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dmhikxrm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zexyqxiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yvyumbqf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kjhagttz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ahkpjrfr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bvebooai.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ejkookvp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xwdozkti.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ugqtmtnk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gveumpwh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ohlvlrou.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2iuwnejux.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ytedhxzo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kiifmtif.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2acbwhgws.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2igetnnvm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zfwvupty.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bbtaccjx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uqgyxaye.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kvpioahq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ztmbwwgr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tyntjbrg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tblxhwsy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ipkaeukj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zdmyorlv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2goopizur.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ladonkjt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kwwzvyhg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nxzgadau.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wwvvjpix.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bkqgqrmi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qmtyioqm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2oeeawwew.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yjpkvegs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2troxiaem.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uowflblj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2kzgexexn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2poqvyqno.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsevmluw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lpsagrwh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2escxozob.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bjbaycdv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bhfagpex.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zkvyjkmg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vvocsvjv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2mknfaiib.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tmusnaiz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lnbnygvz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fecwlisl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2weefghwf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dzduhjnk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ghozbclj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qrvgwbyo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wzctbsvu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cywbgvvi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cyiomtye.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emvetoip.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nwhbtmnh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ijhtxdcc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2npkpyugu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lldfspjw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2obbipivn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plcsqpoc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fkctqhro.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bvgzewbw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjoeib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svrbhvzt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mesklwgr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sxhpqtam.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jkgayorm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yuxtfcdd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2liymungk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jnooxzkg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zcvcbrgd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pveicipi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2hjxsvrxj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2eihpwitj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fehzvsje.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2erwygzoh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2aapmaech.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dgekdlcj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2caqqfquc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ektdsvgv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cwhlqsfs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2guwkbuzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sagugxgi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hdzvfmzf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gubuogqk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2icfnjhns.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ngqmeakk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yspxzddb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ezqipror.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hivjytok.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kzphlpmr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2czvtgjiq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zyzzkpkl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zxkinemz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xbayqagg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xznsoemu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rexwogqi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ibjxuybp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2laipkxog.html


<!-- 参考信息 -->