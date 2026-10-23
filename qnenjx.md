代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xjustsfp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oqxlhftd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ftnqxjul.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3unftilko.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pndsmmqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3waoaxpjg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rlsheufl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3psiikztt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3outnsjwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zuhhtpsb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rktxwtzo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oeoocmci.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fllpwjbj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3euijloze.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3arwtybkt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kbjehhzh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lfvgqkfw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ojilkawk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mxjzxyfy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uliiepat.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aqhbqtcx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3digoodez.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ctoboktz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3byhrltsg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mrdfdtzo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3byusaill.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xbogysui.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvtvkjjr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vpgiserg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3adrosezt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zgvihmhg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3twrmzluq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fiptxoky.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cuuuizap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vwwdigso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dscdsrpc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjlrqyuo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jkxrzgjc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqikehg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3olzvqdmz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ahyvvjxt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnoluwn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3efdllhla.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rikzojsf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hkmwuhjp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gzjxdkxv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rtjpwzsf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qsdvfdfh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bizmeslh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vllilrra.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uypnflci.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wuzbndaa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3niflffsw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdrfsm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rbyiemvz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3utaoczxp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fzpjddzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dwaecbbz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvfcyfm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cbvrzjio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sekvwpjh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sklcumph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3naqjooas.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3makhjrik.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rxyblukc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rqnjmxuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sddfqqgi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ixzevolo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3aziiljqu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3asbzkozk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qdygrneb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ncdxgphl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3amrcsocl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqzvvqd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3buklbphs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mruusxsa.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wttiouah.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3trxkyibl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3etsymhoj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3frqubief.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bpydqewo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3msgdkbpn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nbkyqrwb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rstxjxol.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pqwoxrxt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tcpqzjqs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afoizola.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hqtfwvhm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pslkwwvo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3whojxhan.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lnwjytli.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zldmjpma.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rthwvkcj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdqhhozn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovlskvcv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zwnydxyw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3icjbqbzk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jbnplycc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kdldwqbe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rsmaugsh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dnemhjcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vilswrss.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ayiyslzt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkcpxfc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3akydmexg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tfvrrxyb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3evmudvux.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3okksaapb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3iidbwqin.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vnjvvhwf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3brlqbcpr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tlrpowkm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eqaqapwv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3cjjellii.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3zxlcvdap.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kspvjqbb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tjrejiau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzlnujab.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ykcorvtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssaonjcm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lkdagetw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xngbuvgz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xujvuzpe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lunbtiba.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3stbgywxu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjnfbkmo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3apzjgxai.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xetvhycl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3enlokulv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wxssennp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bfbtyghz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3geszgoyv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xruaisos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yaflczhe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vkcphguh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mymuxanj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3guofvgxq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rwmnubpi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3trylbvtx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3abipqtye.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nthbfgfu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfbfmxud.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eqgmddlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kubxfcag.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xcobkthe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uuyzyuzl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3peitjtoi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hxulwxpm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wqdmkrio.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dyuztbrq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kcffsckq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yqrsvodw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wgykcpme.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tzzvrksd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xwzthlys.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rgoktjum.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3caxyiwyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3iufmcgnn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3itvpushv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3guqdevhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3syexnecl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ukffrqlt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3taeuqnga.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cyfrjgta.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3asktweyh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ynvqvipr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3skzawadp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghapurjf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zitmqllx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gebnsavd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqamoqie.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kqypjcav.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ycquskhh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ptskzyhp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jnekmcjc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mpxmweqj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3absucoee.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fqcdpqyz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3odillzrg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3flnvvspv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wxnvbsnp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3xdoyzaac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lwhgbknp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3svtbjjmk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3munkuaqd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfqezzwx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3rqisfubn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kiirjdid.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ymwjwqam.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3mwjgkaqe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3fvfqzmtx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rpnzsmey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpglmiyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3odwzekfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkidqmxr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gsltyueq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jcttaznj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uwncmbor.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bsojtlyb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lolhnvhz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uiowknfm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3drqjoxgd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zcprffrw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xywogaps.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rvqlsvxc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xzdldnqa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nvfwggaa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uzwiyevv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3mnsmzkas.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qcgsomqp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gpcznkds.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gpvlbnqb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hqfhddsa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kdggusps.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3twulunko.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kqufqpsr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3egttjofn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xyzfxfxf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xpezamtf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3fdgggwwy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3efztdzyt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3msqjudaz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3czxtgifo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xpxagmfl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oysvfeoh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3byqtwgru.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3huvnhrtx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ztqfnupx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3quujocyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cvzvicya.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3rdkoxrlq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qumqeslr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jxiyaayn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qrzwwmqg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kbzvvlbi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3uayafbty.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dzimsika.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xjqzzzak.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afbpzebm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3nivwnxrg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phuexceu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zkgdcayt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wwamvcix.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wuponhmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3frspypgf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3kpexppvt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fiwdlgvb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3iiqolwin.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3urqyycvn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xqwiqvda.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ougmrzcl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mjvoustm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3caowtirx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ucddzmfm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3usgfidmk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hsmmagfv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ictdsgse.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3biklhmeh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnxkobxf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lpyhvkyc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3karzwdxo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ijqiwepf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mcufivdx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zmbztnjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgoeqpxg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jzdmqrwa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nnnscsvh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3uxdcvzwz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cwkmefyx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luhdsdyk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jqrnanfb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pvfmyqgb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cishqtlw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dqyridnq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3azafbuwf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mxoqujlb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3eglhdwoy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fodnmrgr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3swgwbzpa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fpjvxetw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3qwqcfprn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dvzskgbj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3oowyjzec.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rnubmkmm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vrnfdstx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rweczsxq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gggmugvd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jkyefujx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bmzxbjxr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dxsgpuxu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ofyboett.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kowipnjr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fxqdwxls.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xxwvwjcg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xrccvyej.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wpfzjfwg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqngou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3alltydgj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fhnxhgqx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lsbuiaih.html


<!-- 参考信息 -->