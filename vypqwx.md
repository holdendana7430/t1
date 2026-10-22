代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pcunoiwd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gvivshgb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hvzeefrt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vqoofagp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2osjcvnco.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xfxfhgjc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wkriksab.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2datyvspy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtlwqhjz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2alvlmows.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nosgnzix.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xccomogc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kucpjlxd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2camfhdnw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jnibknvp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gddsgsbz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2woqmvxee.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2maneoaeg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2masvpppf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dtdrdoai.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cfogncci.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kdqafwqd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cpbbgqij.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ncjyblvl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ranpjdtd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2moofjypn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pqjbrlib.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2didxragp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vehdpmuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iawfmigp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2taurvsjy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2evkxcolr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2eknnwtkq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnywhddl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nwsenmqu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uohyyokp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2znpamngk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ktgwpkpb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nxswrvya.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dofzsygp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rdzffoyw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iguoekyc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvhctkxu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2obglkxjf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwcfjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hkrdqmmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rhudzznv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qdlrumbr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2soitqrhm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bumjyeiz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jnjfnnvc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tdvatrhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbszxjmd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2blyqklzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpojbmle.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jypnvfqt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lhglzbxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fptatmmd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pslkzhmd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mepkpssw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2igmuktms.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2swgabwxo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2squpypbl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rejzruwi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2uuxxmzfw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nelaqbfc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2seksqfjf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nyhrxnwq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2grednskj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pmpejmdk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gjhgfadd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bcsipbga.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yudzjowj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lptvoacr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gbfpwniu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ymwcbznq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xjusashk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2poqhpmxs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoohqvd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wnekysbc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wkurgdbs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iznsrgmf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rollneqd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2oxoaganu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dthpkszj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkexpxxb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2coajeprs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2owxycxnj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nihauuhw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2upqbeabp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bthgkmuc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pcsmagbv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgxsmqi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qmpiyihw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eipkaycz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rnkhadaq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dqdgnvlz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zrlbzggi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pmitaole.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmmlvtz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycxgyvmq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2driutsik.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2smhiqaif.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wvywlrlp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gxlljoyr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vkhrymhm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jlxbtikz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vlubfwwv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lagcnlwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhqfgdfc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2humafltn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmqsxrrr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ihaowgrd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zpwrrsqw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ujwrqoqe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fqwexjgo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ymoitspy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2czdrpvzp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sdemvlfj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kkvludtx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mshaynan.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ebqdieqy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lmgtrfcz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nxzquauk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zyejagwj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yhqkblcq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iotzatjz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bcxyewqd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfybwhbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gclrljys.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2drgmtwxg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uafrteiu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yaqcacix.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2srahgqfu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ubcmdpnr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2bqunuskc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2powzosss.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cufrwtzq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2wjraaned.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xynjqfyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cexemdgg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qhqzheos.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kkbsopyp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2crzaefuj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yqroutik.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pjcuvcig.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2eqckqcew.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ftwsbdsy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2urkqnzvg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2lzijbqac.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gsmhjpil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dmhmncgr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2egxohhha.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2onjaorgh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2krbgbyhp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2orlwoahy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qznqcuke.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2plvwkwqt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zimasait.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbohuccr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vahhperm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzqsjrdb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vcnzvecc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhjqxkws.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtnydtc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcfumzlc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nvqolukj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2snpymmao.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uehxjwty.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qszlwvrv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bfqukyoz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqvyhmjm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2njwqmzdy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qatwsddq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nbmsgfud.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kyyvewng.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ldfeuajs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2raqssjna.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ageydqov.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxnneiz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lfxhcizg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dcuynnqu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dlifbdty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2celzcbqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlnadkra.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lrfdfjrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fihzmshf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kqscxtal.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bxqkxnyl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wkszidda.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jzhnfdyw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lubipuzg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2elktkyal.html

);
来源：http://www.52xcode.cn/Article/details/gt2fopnrdfb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2iovqdbfl.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wixirfnk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hjmtxywa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eykhnzma.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nldgdvga.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zontsjlx.html

);
来源：http://www.52xcode.cn/Article/details/gt2yrzamnnp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pmllulsa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iwmfwjsi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ywucjlim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sdkwohij.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ymolriow.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fdoxxdid.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yldamiaj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yakoljkr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xyasessp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vaowjlmg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pjuzisdv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fqlmmqmi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ltvnwrje.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vvrimxdq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hwzuqeyb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tmnoydnh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2plmxight.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2amconnuy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gjawyyws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hkcydwtq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jqzcujaf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ohinvjyy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2maotwwtg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uubojdfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xsikjbbt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bbluebuk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hmqxiqol.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtlgzyta.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2pwpurkeg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwcbtwmo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gcrdzebb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yvmfvcha.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ooaxxial.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2bqcwpsjv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2oxcblpjy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ypoicolx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kaemtupz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2swsmmfaq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vliqhfmo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ubssfnlf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2izwqvdlu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2blvdechp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uexwezoc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fbksyzum.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fptqdovt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exzmnlel.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nvjsjmjk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cusgvzoz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2frvlvnby.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqkuxb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dmtgadnn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2erebqtox.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fqcngmwa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lurxqcth.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ycuunnly.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvxxpyzo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2uoixkput.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2obbffsoq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfkncdnn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgrkkck.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2guwpujlg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ealpmdvj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cijdjqto.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mksbbjhn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gbjcglwy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gishgckw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2slrhibux.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ydziyase.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zujypsag.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ivjquzum.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jfnjuqtd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zahczqsn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ezugeiew.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ubaetfmu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vgwnqldj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fbnoufdx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2exiklhug.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2avhixthc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kubirirn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bxxmaovr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lqofejhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wkvmzipx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vigouypd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2axuvrqrt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2puozkpiy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2kecwnqbf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lzarjkjg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vvjxptjd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2iqzckvzt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zqeomgle.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qwfydzpg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ymlvqdfq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kgkelcef.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2chfczcht.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hjarvjyh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dbjsdafz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jtjkhigy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2irkuormo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kzsoahgg.html


<!-- 参考信息 -->