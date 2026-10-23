代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jimfxuuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3flkkjohh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lgksqavk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rhzuaapm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3trovcfxw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jfatytgl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nguswcfm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3juxkkpfs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3duspxqtu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnjdnqm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3larjbkam.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vnlsmezp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ejnrwqbd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lwvbvjih.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wlirsupb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3huvxfmfm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtwkbrt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ohbkamgt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvvpmcjp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3soiraxei.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdebgbyd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3regrlfev.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kbmizeth.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3guaikmau.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3amwbyopa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjfggrme.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oldnbdhm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zzqbcodt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ngwnboyd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3litemnwu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3txryugxj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqpygqhb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dowbnrgc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qitbhmzc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iltwsydq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vitggaim.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yetxwaki.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjprtu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dovhujju.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fwahvbpp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jhrpybll.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ubijurdn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3reoprwet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sqcryiwg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3smirmavs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mgfmikxy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qnstgtxj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yqpshuld.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eplzgfhq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jpzjutak.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioebbobu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qkfyqmev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ykhwznhh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tmeimncs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tbjsktxs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nefirsft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qindjzvx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvkhuzk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3daalwuna.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zxeovuug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvrnznqy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hbtjyalw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrbylavv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3emqjkjnk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vseapvxs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mideggbo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zhcgfstv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3eygyxrgw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yxfiqhvm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3eamakssg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xwzfpoji.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pgtqsgqo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kpjyrcdy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3weaadvlg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ohrtkhfs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3usjriend.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lexuiths.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqijpbdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jpsocvls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kadncvig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3htxmwxbg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fccxmxlf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bkwoaldv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3svcwsmcv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ysccbdkn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qwlpjsvj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zseeskgj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wwflbygj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hezqgbsi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pbasxpzz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3viahbeev.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tnzicvci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fdzqvnky.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bxpdyceo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zxgxoaua.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3caasatov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3puqbqxuk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3cyoyzdgm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yalxodeo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3drmvdepv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkwfykq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dskeiuzr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fljiwzwn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tdrxmacr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zxlcsene.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xuhqffmd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjmnelz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pxqtsfto.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wlnssazw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mgepawbn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvtvtfwi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3viyynote.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3foihmfmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3aidlnmvx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vwcwicsj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nobccczl.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mlwnjcgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieflyipb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vdsfkdtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktxquyyq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3conqnldy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jyvhrjgj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3svgnhlsl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wrwzeisv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lquipdxb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3knqmkjhp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bxzvxrwk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dfuyqwge.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ughhoiyt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xaqowwgm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wjoqoqpn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3atqvvhhe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qwcyonpr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tjzfjkzs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vbyfllrd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wpfxwcjr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aenpipbj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3kqkfrevc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tusyjdtf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qyfbsxss.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tdsaapxo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxnhljf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yltibvnh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxpghfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hobylfji.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3aauxvyzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ookyuwnc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xzemkzxv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cmdpvcvi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3skxnhaab.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nwbomldb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ahobwfxs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3syjtpwoo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwsnqfv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wqlgirep.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3adyfsfim.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pdtnucyr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoimla.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yyvbexkb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3grualxfv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxxsxwa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jlxinler.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkpqfok.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jsrhtazf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hjzkvtxe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3soqpbxpq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vnnaqzmh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3alboovtn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3iyuikovp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihdxuops.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3viuxmmon.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pzxsbutm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3atazggsq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdueqjed.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ywxfqdyi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kqkfvmpj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nhujlsky.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ivwnrucv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jgekpxdk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3pldqyyta.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yscmrsgj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dpvfwanw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3eeqvdqnl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xazoqccn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtrxaox.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wugsuplz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yulgiuza.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jpztnxqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pweujbnx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kyqrkdgg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3otmgqdyo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oaeiczgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gchytvpo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lnhlxvnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vewqczdb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ilrllbcr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bzwjhjmf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qjjtmeab.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3axfdjgjt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yqtdbtfy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ujnqecgi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wfospmfu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yxfmlbwo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xsflrknu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fiphdtvb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3iofhdlxo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3exhquqls.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hyptapux.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3phoozzdr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ojpyqpmg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3vvepxvpp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfounkpf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3uhnmphfg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3avpvpicm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fogytqbo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hfvifndh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3liqukaux.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wfmfcqcz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbdfphsv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3vmrundbw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ukrnmght.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3czbqgaab.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rzgmhnxf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zhquafpi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rprqmvtn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cuiaylao.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cpeaaolc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tngxhtez.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3uybimbak.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xasgeumf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vbikcddi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zlkaijli.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bmunihpf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rzjuohta.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3cdpkryzq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3poglxjba.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfrgsvoc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3clfaoers.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrekzhc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3livwxmhm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fjvxotva.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xojcqmed.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ubodvjoc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3wuhuqvqb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uwaoqazh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lnfaromd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3riygxfzm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3okdmsdsg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3achrszat.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3egpzyxrr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hywqhzid.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nkewsgjz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lnslkwtq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nmxxyusc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdrmtnhs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tuvqaqmp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vqhgecpm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3guguakja.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylhmqesm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bavvfdki.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gwzawkro.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nyakmcff.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqaltrug.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uimoqkrb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zetzrbeo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ydrhuinc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxcgsm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mmwvcjfq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3raucuddj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sexbmqbg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ohnolzhx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mscpiqoz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zglfnxvt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3japztque.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3fchgucjy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ulphortg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3emrgowqa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozcnnxhr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lzyxhqpp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rjwfqrsm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tmqwlpul.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3attojrds.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhyvcz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yywneobt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jdebjltn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qwprbghn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ihvpwxwc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jjlljlkb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lornnifr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rcwcrnqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tdunpody.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xiotxnyl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jcciwahm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3joaxrunb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zksgfkkx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gbxuzlpy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ezhdbogn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gwaykyyk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ttcaaxbf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ztgwiopl.html


<!-- 参考信息 -->