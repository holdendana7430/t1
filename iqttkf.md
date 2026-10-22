代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uoyrqttc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ziernmdc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zubepxhs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gtxpqdpr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zaihklsl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vsvoggfp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ymubyhis.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jcalfhxg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dykdtwqf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojomnjvg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uyxecblx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wyzhtosi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wqdxoypy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bxthbkes.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dbldmwil.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2omxnchpv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2eiqdsqwg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jyuarlyj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tddiovyf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rmemwnkb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ojzkasuh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tqywgnax.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hltnrepi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpxjospm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkhtovhg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nwytnhpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2unqzzvct.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rhedobtc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mfdvxwom.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fmlwyeyb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vngtfmyn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jffldypb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sanlfdcj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cdgwaigu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2upduzyvn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lrpazagf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mtxyqpxl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lhlscerl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbussrgm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2selsxhnz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wuovbztg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuisnxmg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bhhuxrrv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2eyyxiime.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2caaotahz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ijwkpkjs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ssnmlqns.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gsmyjonr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aklmruvl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2buhdghpc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vxbtomkk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqwrukhf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oqdgdyhe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bcrqkmfs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vcrwrfjd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ynykrjdi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2memmqpxu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2seiwaywo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uavthlbx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cfkalxea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoprgmdw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hyjwksga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzyiemym.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wsypeeyt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mlciyyny.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kojapukn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ayzbrgaa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dtoilphz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2rdmgyune.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wvigdbnk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ngeomvcy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tjdorrrc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2epuulxfu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kuvojdtc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2unmjdmok.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dfzcbcpu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jalsehuv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ntvkuggu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2miilwydl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zhygcotf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hlkgbmqq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nzpvhpmz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ublwtrot.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2owigswre.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wifuqyly.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ptkyfkbv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztwvjioc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vdiwvzgu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fxdnrxoz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmhzgxy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2urxecahw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rmrxmhzn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ialgedbx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jtcubqbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2prgrunhm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nmwoetkw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wspgihgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pbtdjnjv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdywkexy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rpodyntt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kyijxxij.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ekigcdfl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lbauqqxf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cpymgjbo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uqcssktn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mrfabgdn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ffqjzdyg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xzwoamvq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xogevrez.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wumgzrso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tnyasskv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rujyfkuu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ykuyyyvl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wpaevuwj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2csdptwwa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fdiqhykw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rvbouftp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcocbwbz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dffvpgxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebbrjoyp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dbgkelpz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2okclzaqp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xizxlzpp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kmnfyumg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tgfarqdf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eqlfbjpy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qilipgda.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ahpzuhio.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2oxxtcndd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2abwytetp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wemhybwm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykgzlcvm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2iaptxcft.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2trmjjnxc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hsocbeed.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bacoykvi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jqkwkvja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qmoanfci.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2shtzunql.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dexlngko.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vumcnepi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xctlvriu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oytikqni.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2gxnkdafj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fwqvgiva.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjwwujpl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zqlhuqks.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rncxcdej.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xzoidxaw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kjfitxhk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xbeuiwxm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wlzfzcdl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yujgphtj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lzavbtkv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2gfqdkbps.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ydwupmce.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pqfcnzuf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rqpkbfst.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nmgpjtrm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ueqynznm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cifnambe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pmodcqaj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2izgmmfkw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vxqjuckz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mdpgswfq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lrdigqhk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ohgtpgrv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sztdospm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ajwxuism.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmpvcdxb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2luxgtuer.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sfxpioil.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2tuegxnck.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rdrascat.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2lntgbqkp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dukevcvz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kinvmcsb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zilejfaz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tribfftx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2jqnpxpwa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yvrgdsjm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2noogfrdn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2recbdgoy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ebekxdrv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ukhrekyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lsmcmcdn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2asyskkfo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rpcgrvgf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rtkwhsyq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rtvblmdk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lwmddvke.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wrrircwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwgeybzt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2yplqswdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqirsluc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zladskbc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rwzamljg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wkdmumkn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eabaliqq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2vllufoiv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ljavxtgo.html

);
来源：http://www.52xcode.cn/Article/details/gt2ipivkbjr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ndbvqcst.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2keezrgwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2umvnrpsz.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uskyafhu.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dccsymrf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjqtsho.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jxrmfxgd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2orwculga.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zcyiuhwv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zfxmeotn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ddpgcann.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kgohgqtg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fynqojrz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cetvythg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2jvquxhyx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ckuucqku.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zjxbpkem.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gazdxnok.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bgboprna.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wjurxany.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rpdfpukj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uiqrvoaq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2irwcempc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zwdkprpx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vccngwqz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bfdayuqp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wdkbqigg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2oeulajxz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wcompjaq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gxzbtkrh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kpuxfcwy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2alpgneay.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2oknkdfee.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2boyomrtt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2stiulynj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mqeaipxa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pqznlulr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tpyqtcmz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2glwpwchb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gochjgsi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hofmduxt.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lyjgpoqj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ogkwvotg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tgjhaelw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtyoxiuo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mmkpxqbw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzpixwj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2biyxxwbq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gzsafgxk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2trrjydqm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2icrlcbix.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uurfiuoz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ejjdqjow.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2guatgqim.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kkmijrvw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kvffjrll.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2egpivurx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vxkvoffl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nduhhaeq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2jyfsqjdt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oisjprcz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2gmvxlcyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqbiebgn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wjavmhgg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kpoqqytd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ebfvhgei.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ikoycisy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nvmkqzns.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2irbriycb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mfbiprnk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pyypewfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zmuekzep.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2abisqbjm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pgnuuzhq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mbrxolcq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zgjaauyj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zwwxnlth.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tcnwvskn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rdmlklmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qingwavf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pfzkxmxt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2erzscxau.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2mynshdsb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rdewflnp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nftgvikh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ugjnjezg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2grbmdexp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ltjssetz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kdejgfui.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mmzrefvv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2oleixilk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tmtozgvu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hkxxixbg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2whogpwxs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fizzclxs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vmeexklq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zlzcqigo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2llcjwirt.html


<!-- 参考信息 -->