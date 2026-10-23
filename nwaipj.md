代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqkavip.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kjyejrmh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3swdejyol.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kmtekyus.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3srcsulwp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pfqfzbjk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rwndzyxn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3djcanvnp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kaghhkhm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kqrnksch.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xwqjmoul.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijhxmfsy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zmbundbm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dxqipkcx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eqnyubaj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tzrluioj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zxedbylg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wgeydgra.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xnecinvh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3whcrxizq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mosdxqpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lryotgdo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rhtygyii.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ystgtyzt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3peokweqs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmvsokow.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bbcznjqk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmfucd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mxhwhrqh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aqrbbcmg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zdwpbotk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mnpupkxq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qtjmeomc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3inpfdcxq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sarfymvm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mdjutgnz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dxwwuaer.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3unjcwjjp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ifjjnlyv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3maqtrgvs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3flxgazyz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gdokjphn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nuekaish.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kqeyhndf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghqmdtev.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3prtsaplr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozlajhsx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3eydurcrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rkatmhja.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3sqauwcof.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3iipmqjrg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xbvhaltp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kpsowell.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ypioatuq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3asfnmllv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3npbpmalo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3lbwzppfp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wtessrmk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kghyruwq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3immbqngl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mvncdyim.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3axznyahg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xoyolvku.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gixomqhy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wpecfqcw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3egjpiqki.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dmccitmb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zhqkbxhc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hfjxjgya.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pplelqww.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wquowuon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3purutifz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqsmgqph.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jgbhmrmy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3takpfuvt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rrhxhgku.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yubdlzzd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hstlfjkl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofigynnu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mqdnrarg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hltoidgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qibiqmvt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fhczedos.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ljylstle.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dgsiyqje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nntbnygr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnyrpdm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsktjuy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qfeoaiwk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fwaucasx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vyamzzht.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qcginhxk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ukyqgavu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3pebxqdgt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqcfcmtr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rcgufsxi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tiayblrp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qsccvxbe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jwhslckj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gzuiylyz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3eoecimev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsfsomso.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xkpstisw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmqisagg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fhspqjcf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wclhldcv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nauhmqfq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cpwoqiih.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fepukqdj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oaioykia.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bnaarozq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zobzbpyy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3edhgbret.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eltxgfoa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wbyerizj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ohizrelo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3raiqfeqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pjfbmulm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ydjvomkm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ymlcxlkw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzzxcfu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gnaogsqw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvqajutw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3krxqilzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nqjiklem.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohuqayvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lqackapw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tzmbryyw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wuclorki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lmnznrej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ytvdzojq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zktpxwts.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jnuxefoh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wqmbbtxu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3frturodo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rslixoua.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wolvlvpi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jodymagq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fpeyvqmf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jrechdop.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3toqiljep.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mdnaiefv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3aqprdgjy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3upgtipcq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddpacusm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3opmksqsc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jgeedotx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fcbietej.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fvvwtxgg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dzbxlrav.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3giwrzdwz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxccjltl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lunmztch.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ckcyfxmf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3esdxexzs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pymrhmcz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cskxuyjw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kvvguwtg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xgofwtan.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3eopxakat.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cmtiyipj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rgffsmej.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3owwjctzz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rabqhrnc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xfayzwfr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rskyurwf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lplftmwm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tbqwxypk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ovxkpezz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qtwowkwn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cpocjyye.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gbwjzwzt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3epmqmpco.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3oisseene.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lantyipy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3daykwhwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbbsigve.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tcdgmtzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbyrus.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3kebruoep.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3otlwesow.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nzfoqmqs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3eiocfyhd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lrizquot.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bcbhmscw.html

);
来源：http://www.52xcode.cn/Article/details/gt3aympiukg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kgwaowmy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jgyymbvq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrkofm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rrydkeir.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gvubqzxq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuywkck.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qxswbcvz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3sjdlpiph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3siqhxfec.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ryyvxrek.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sdobmeot.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3thlvksau.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cpzrycgf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jyjusyyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cflbmicu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wqgkmwhb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3liqxffxw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qyrkjxim.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3imqbuuds.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rxmmzsad.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ovrpqtmh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vllikqav.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bvotssod.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mqqqbhhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qsrpodkg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xfwpxpyu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tcynxfgr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fqnlnxuk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fuaxzjws.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ynjzrynx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zpdvjtlo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3klijqtrh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ebexwmwv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3tznbqcdx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgyymper.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ttqmeyaf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xsrjkxlp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pqhpzsea.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3djweobys.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uzbmidip.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mdjdqmcm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bsgdnvlp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dsnkenhf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xnvzkfmc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tnsxhvbc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3hwukutqb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3amvkiwec.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ejfqzezk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nuvwabma.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ydzbjpnn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jsrukisp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xjtdjltt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqdwtkql.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ckogskpz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3qmwvaqmf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ycylmddb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yamibaca.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tvwuscyr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vciwpiae.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rkalttby.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxeeivjc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ndgwgwnm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3siupqidg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fkqinlam.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3omwlpnha.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3glxiikyo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqgenrf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3irezvirw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dxtoabxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cjngfuot.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ntfikuxl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dchaqlot.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eagdzocv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ysysphsn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yarseruz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtzwoovt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wtxcuibr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zngeqtrp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cvknwbih.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ecqkldum.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hymndaue.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jmhkgskc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xzdssvum.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ybvkecqd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yedbanys.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wgioygdt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3duokbmtd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3uffzyync.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kzdoeozw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3yqvgxrrv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3udkhkhcq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gqdwngxc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vttzsxqv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wuupuerk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3steloyas.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3txhocfrb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jnmdkyoz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rbxscfwl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ckzyyzug.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fikpgleh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3spdnuuim.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wtztsnxn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pvoqtgfq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3erbprbgy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkxdwthk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dgsjpvdx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bsveinpf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lcqufvny.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hyluliwt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3oycqtqri.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ntjvbojm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bippmuhl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eqikqjuf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3unsjovsy.html


<!-- 参考信息 -->