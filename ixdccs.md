代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ajacwqgr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jcgmnivz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xloynzrj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3anrjnmdf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3omymqvcm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lxpbqujc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hmbghmqv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ijnqvroh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jdtrbwij.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3arqwcgub.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dnmhcwoa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nwnogcqf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fdfeabzd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kmuwfghy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3msdysfoq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tkzqrdxf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3amlcgcqa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3njptmrze.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jkpescrx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pfbnrgzv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tcjwfwns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wiydyevl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zgtwthzs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3oqhhvait.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lqjxluye.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yvpmovyw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kqdayywm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hfirppko.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxbrjaig.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dnntczgf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tuxrsyoc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nzdxiqvk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vimvvncz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3grisabpz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nkxtjlvr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kwqudfrh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vlfdrzaq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bzcvddum.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjjdmgan.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kvcaujjy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3auraivlp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xsmgctij.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jhqxzbsy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fzanuvse.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jzihratb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nxirfikw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qbhyrjws.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sntgzpje.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fhqhruru.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ygitykud.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qloygxcv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zzhkswid.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hkprgsse.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmejtzus.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blpkckwu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jommsgni.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnlkrxjw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wbcvsous.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvqdusej.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmjljwzi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxpufeiu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xogymypo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fbvudblp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fmdonlnb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jhpxfaft.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3axrrmsbz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uvxfledz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oqvfdshh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wavqwzoi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hafhhpte.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wrqjnfxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vhqnvoby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqtqwcxr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xzdyherj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pntywrwo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3erubnfav.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ontximum.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ifilulhp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ezfgfnwr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hfyqjgmg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ceqaktnf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3auijdpvv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wtmvjcuu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bwfqvxbe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pkekvfam.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjdnmtj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3epntrloh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hocozuls.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yfccihaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zkmszukt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ilmmebai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3oxximdze.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fdkchmpn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tqxxgwfm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxokrubd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kwcolgyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cpnxaywd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ckqlawmh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntkeraes.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fopkeesf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3idlnfvae.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3loklssbm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jbvrcgsy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hnrftugp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wghrnjdn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlwnauby.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vsokqvun.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wuebyhfo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qpknwbjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3svvjjfaf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3oyaheqzx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fzjpoahs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3indynvcq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lrramgcp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tfupvwqh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wpblradl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vcuewcdb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ahjzbrdu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vxoqlxyh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvgxann.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gofkvuke.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kowtqzpc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ukpcygex.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gchsskpg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ysxyxvwd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3shfrhmxb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zoftxpke.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hqcjggmq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cgtbmdmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebzazzqn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhtovykb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urwwaxtu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3krxtsaep.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kgjsfqcg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vvgpgyjr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3msfeluki.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bsjbzwzl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3agkutcum.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lgivkryl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3smhobdoq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xxjxmvur.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gfuoradj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nyghpjsr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zmozllep.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tztiuxwe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jiqgcgdb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gbjbsgza.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wjmfmpzb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mrfueyfb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yngaialk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwwlgjss.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hgwivjhs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cyjyfbte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lthxosri.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uniglhvf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jjlrssry.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zsxsavki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3moaeqecf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tdlscdnu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wyrckmew.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cbncpmze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tqlwvopm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sayoqvqy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rmhdhdhw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uupeyher.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3yygngbnv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mvuxdwqg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yyadscgb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ddkmnxyn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3aaxufaxw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3prehdlss.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wtdxfrms.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jsobaosy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zfrcdtra.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fjfvyply.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kkjoqanp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ppflkxua.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3upzqqjhl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yjmvrbnr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psnheqpg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3raikyask.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ituujdww.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjgsxsai.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsqshqzt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hngbwose.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trkgpklq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3bnifdqzj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yopidxpc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rcknyhse.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qswkbowd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qfxuixyb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ykwqnwyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3epabqpca.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pisfbmxm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vfpcaczn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3aewrotku.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3uxeghllx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlnfryr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bgdvkjna.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rytxbkis.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3durleiwf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3shdyxfxx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tfcohbpr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mqzjpwuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxqssncc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qhoytcgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oehhczbd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fmwgfhek.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3owvfutzh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3spxxzdig.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ybokxvje.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hqnfrfsk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lqshbjcj.html

);
来源：http://www.52xcode.cn/Article/details/gt3vtefowms.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zllluzxb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rubfanss.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wcwopghl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jyaijgbo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yrfwkgis.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ktksrzng.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3klinsgsy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3notlyluu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3raekyprq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3opwtxnuo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wugkbvvz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xrtqsklv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xljgudsj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3xtbigzdf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3eoalbpjz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jqohrvcw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gvktqbje.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vmjmasbn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ocpahraj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3pptdwfjn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hxdxuwpm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hvyznuci.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uuiltkie.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nitgreig.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ourtpwyd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oxcdiffe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3brbkhnyw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zpahpojl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rsmykyno.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kdwayjbf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3thebbalj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dmrgawuj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3thoccobx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dwlzvyrk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idqojriz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yjomiuwr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tclulljy.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sgsprfjo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3cecliahf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dwrefwdt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lgiqizrv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3anaaqagl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lvaixemp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ysbaokin.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otkluopx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3htdvvuxw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qeiygtnc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zomwbztz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gvqzsglt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cbusriip.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3algmjqcw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nmkvitrw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urhooecl.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3huosknrj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ncodwwbf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3totsyews.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aaragvhl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3opjilxye.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qraqwzth.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kftsoxjd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlnzfhkv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aqsnhnod.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqtzprog.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nkdghogv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hltnbiar.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3knmfwgvf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fmwumecx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3orpcbeog.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mxrglfux.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zxaiibeo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gshodzop.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rrevdale.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ivrjlhhk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xhqrqcmg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3enfvtaiw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mddwbkbo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3bggeinwa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ygohkzst.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wagwnbim.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kttegsdl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yfdauohh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tffbiolb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3axffodnj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jjiuirhu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gtjzxhbq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dxxlzrdo.html


<!-- 参考信息 -->