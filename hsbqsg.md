代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ltwozodb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wliqnrjb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jwheaijb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ucanlqmh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3phaklgqh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wgutkmzi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mgwhusas.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3irekmzdr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pngmvrgq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3onpwcuds.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qaihckne.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jfnicdzx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmviophe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jajlyoty.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ybkzajsl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qeaouvhj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbpbywqq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iswbnfgb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mcvxrnzl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cztemizz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zsuntxpw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lsdunawu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mwokcplq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdmyayoc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mjnbbxmt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vpyeoudg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tegbzvov.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3medggkiy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ohvtmgad.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xsajguzk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lxerimbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hflodxlw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gskygtzb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3opwdbzjm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oldkfpvr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ddoodjyf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mhxzzxgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3empgojkx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dotlbwky.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fmkfmccj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hyppifth.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rbqpdagq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvpixizn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aacapbhs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3crcxdlre.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tuvxtssq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yhfmajvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3obsojfdl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kcieefcu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfkdzfo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ghnpvjrs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mhbgmttn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzhufoij.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hqwkwglb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywmptwhd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vkukjkii.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sjgocwnk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nptnprqe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lsnnafuf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kloyapok.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3moazhewx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cgvzywsn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zmihpdue.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wwrcqllt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cuyvszwv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pywhbsvc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3iigenlyy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zowyiefi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xohouyaq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qsxfxsha.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bebpfdfw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qsdibhxk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3amwmmgvt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ztbxxqcu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gcedwfev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nnjbmugf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ththpqfl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vdcshylb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hbumkqth.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ijsscyqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yncrjsex.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icfatqzi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3giqwbdee.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xiakzcmf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pgrynldo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmbsgwg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjwvuu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ybroxqhw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xlyenlan.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lllnouag.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igqmsofj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3eheelngf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvrypuix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3pffshrqr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rhxhlzvr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3frmvulbq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ggkgtsnu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zoydgvuy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3btmqlpdb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yytsgvia.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jxoxxugj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ketaptqz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qspyskeu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fnodvsgl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tufefjvw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3isbhmaac.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3llwyjjuo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zuyxfsry.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bzixhedo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyrtdxdf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xkoafjfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoiehfrz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bjyxobfj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gxogxzfy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfzoir.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qdqyqydi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ansmxbno.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ugobcrws.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tpplqdwj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3pbtlbjqd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3obbgiafp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lzqiiulf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kuweqoug.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3udajduof.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3owiewejd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nqfxcqhw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xicujczv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lsvgjgiu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dmgzvfbu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3evewzuop.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lgxodiln.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qzynihtl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtpcoyx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vpuvkvfs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ghoxolxm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cisxlslb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ykfiddkx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvckjnm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3itraioez.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rzkxyxyy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3onqcdypg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yhxltqes.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cuoltjqo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3neencbmi.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mosuvpcd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ijharfju.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fzomgjpt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3frtznhlu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3svvrhadq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jmzxngxk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sogkhfgm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kvoplciw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbztkuv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gfbpfkzo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lvsbfwhk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3aruykijf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3huqknufg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ivjppesq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ogeeokox.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vrtvuxjn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3erxzqtel.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ldxrsxbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvrucskj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zotglmlw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ldmxedgx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwkuiciv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3urltnxyv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pseyypmc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ywbwvpan.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rcphhlql.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dzovyfem.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tuwkzehm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3owewwvrp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3mrfejznj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bctrsvxv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3irswlkng.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vvefrwqj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkbbedz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qgofjiiz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zoguelnn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kzgtsvsg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3umxteaey.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3oivtdnxu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hzsuaxyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roorbzrs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wlppfejb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etzsxaej.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mxkarckg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nbcgbran.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ctwmdqfm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nbylfdoz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zmtzgtwl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3eeswdvid.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yuvxacjz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hgdmpjgp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kywwzgwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vousivxt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rsulqppc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lujvwkbv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgjzcfq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3orxofdpj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uvnuqvrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fqypqphe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qqevpjpa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fauzjbim.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mfvtidyh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3yfuixjjo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3cmahiyqm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ctkisvoc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xwlquzaz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ixllyxwp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ewuqvjde.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lmkhbbtr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3egkguile.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nsihptqr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3riluwhwk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cintftld.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3dhxopull.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mkdqxwxx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qcksmyaz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jlhxbsow.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gerkmapr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dsveafun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aawprjgu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3uvvrvvet.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3barvzsjd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfwhzvd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3izckyggz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irafevwh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3eyymbcpa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3muhylzfi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpmchfbr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ueydhyaf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwrzyaxt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ndlosdla.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zdzuzohe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zhgvyksn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rddznswb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxzawgao.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ymgmtcua.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kmlsyoqm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rhaigwgy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3tgxdzlbb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qvyrepug.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nixajxjq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vwgowjon.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3latjvvgu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ugcfynre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jeqzpjwu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3minhmvkw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sioabbiw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3frporyep.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wftwoxlz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3viqlfbjo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3idgzuglj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pibmiypn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3riwanqxd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kuieucgz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jweqdwil.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3onxrlldt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nvthvhdb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vzpggtvj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rcanqtuc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uydxgysb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjexkf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3basacasv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3njjtycmm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3gwelbbjm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qaezggfv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mnrbcrdg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hqffdbnz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sqkevfmi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pmrjrews.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3crngfkla.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3llwszorz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fxqtdwjh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3smlgedvd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hjoyfrfq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3viunxnlx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jpvannlo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qmxkhmaa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hcqzxdjp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xfgslzrh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dxsztihp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bpdrpyqb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rvxmjeow.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dpkzryrf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3arrulzwc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mqlrhpba.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kjbysxlh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtlxlhzx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3iyaksvhx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sddfcgxh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ecfyzahk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cmshvotb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ccndwydm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3abyjtrgh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wagqcnbv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jvkchbum.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3wgwvbcvj.html


<!-- 参考信息 -->