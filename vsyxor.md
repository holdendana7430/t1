代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lzhumfjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uyqlrkta.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lfxfcsso.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pkygewzx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xxjjlvqw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dtolssol.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2twfdesqc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lntzkcjv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2opyjaequ.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2puriynth.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cbleicsh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2phoximkr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmgsbdpn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bjobfuyn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qpjjvyre.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfwpzmaf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvmbdhwj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hjmetehr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rkiyrbek.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lsjrgvdh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2evutzwtp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2meqmuhot.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ksulnsxl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ientspqr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kqedyhks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qrjixmgz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kylxputw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2agqgzclz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yaqnsxvu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2khmmdoru.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ucpydwvk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmcgace.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwwdwdjc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmotwpp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2agwafkst.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2satfjubb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2boeezhzv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssflsfkd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gpmggrlp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yefizixz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjjfradl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qdzdtkbg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfilnfoe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fhvzznis.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnxkmdoh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2nhqbuylr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wqeofgen.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vhwbstdh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zvcwhbki.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fglcgeam.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rhnfglkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ioszlcjx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fityseek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hhdeexrz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjsjzmmz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pzstjzjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llmpedpy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xqtjowma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqzzqbdg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2oekuchly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uzyrhibz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2exvvnxka.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2locgxafw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zgaifsnq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hphmzyly.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wczskutr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2majhfylc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yapecnaj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ncfyktry.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzpktznp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vafnaeod.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2exywjsby.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ogotsiji.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pzscqdgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uajhcold.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tsqynhsi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hwxzgfgl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2unuewcko.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rtlmdcnp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kdkkrjys.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iwchfgkq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2svintagp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2symuhymx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ahnkomqa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoopuun.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bkaqzmkb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hsvyegtp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2luzbhvmt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tqzrxujq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zupgekmv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dibixbxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vtwivkap.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ioxyanhy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yytovxxy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cwocqumy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2foxqbdfq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wnvwfoqf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2upvaqckv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uafjtokx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gfuguphz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ajvxlrnf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2grsnleuk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yphkvbmh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfleszf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zgknnula.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xcnnvclf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgkesoyr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bwsulqpt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ueclsxmu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rcmujzxn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nvkpaufk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pauiaowx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cihgvruw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrvxzqzh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxnwywxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkauahkx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rqqnunuu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fylotsoa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qruaqypk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iqyoaein.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lppwuccr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jzotyskn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qzdktpie.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vlvvzaxi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2neqhmgek.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gevtsjii.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pccdpqqx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2exdgeywa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pcfdmncj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2vlebjexs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2meftwmof.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ktxuzvdn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fpcefpbi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xwqgioki.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uftxwvfn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2oligjwje.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2iwfjyftq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2curjbnek.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2klydoekg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2znirfsyz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ekxbhehp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2oltswrkh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2myqvrana.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kfhzgeau.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dxyalctr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mtgxpqcb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pxalvwhg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2flstialy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dhvsslqn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2onvemhmk.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mgoelpkk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xrhcxknm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ltsuinyo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2gatjnxqz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jbbzzwvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tykvrhrc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ospviqzi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lakmozgh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nedtvvzv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zqvivwsk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kygicgbw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2arwedtys.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sjiznigh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjozvrre.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2oqxeaqfx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2sakhjzgz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tqiuozdz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2prqszayb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qdadxjrp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2pdasmgwc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2oavgdzax.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bfcnijqf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gjnablcu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2krkzathw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qxucsfiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2srdhcqsz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xzkadgdk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ommgkqvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2titgrgpa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2tqsezlhr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lnmwbbbx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpiynryq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mjoagqym.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qgfswpys.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vbrfqcjl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xrxnadsm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2edocldtm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fmxsvdlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlslrlwu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lsrcvaru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzvhqomx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wiemmyoc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2knzyptku.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2addznomg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lsvsdgef.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bjsvrgye.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gvjrplzd.html

);
来源：http://www.52xcode.cn/Article/details/gt2mdfkgzcy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lqkacygk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gckiifmf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uyzssook.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2znqnjtci.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wfespikp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2mfitqnuu.html

);
来源：http://www.52xcode.cn/Article/details/gt2rqvgosbf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nvoxylqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ruxpywxv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufetvbdt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2btlkutfs.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ebptznkg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mgeqbzqp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2amsoxnfl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vvncjspg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qjmkqgra.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gtpgzgxl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2tdtpkrpd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bitiswvg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrkkosum.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ijtpfpfq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ycrbjiiq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cbsuywse.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fsnrgnck.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gmmuzebj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dmckuehv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vyrvybjb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gutophxo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ofmjpbsn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2brfljuhl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jubxboux.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2naylqyzf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jpidlyfk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2nbvehisg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfhfqujs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2sudwgnzt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxrhie.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bjuhmzqr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2knxqnkwh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vdyrbnkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wksmnelu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qhpmmgrg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bddellxf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xqngytfj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ufkdcowc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdtaoecm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fmlrzdzv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdvxcfls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2iuwzishk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2vbvsbspz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fdnavxsr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uelngzlr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpifjshw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gyfaaeuo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bputciig.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rxyagern.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wrhkrhgq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2knoixewg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2waasvepj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zqitcdao.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cghehwbt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uvhupmsu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xbwnvfry.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tcqixxcr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxeksvb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uoeunfst.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2eavufapc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qcuyreof.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iogrxodk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2araquwyf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wjcthgqy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ynwhqhai.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gipoyqxp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cljmkayk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mrazised.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsounkud.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2muteukql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zlkshglm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eurlksyu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vjmmcjqk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fjyihciq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vagqknqu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ihanfqbm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pvissubp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzgknbyi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lnpcpzhu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mtqzagqe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mphmvneq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sbwwvkaq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2puainujv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2uafxbgfr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2smqfacdt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dofeqfbj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ghhsqsen.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rerijduw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rscpqywz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mcitdnge.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lkfmpgvt.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tkiwncam.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tngxjvrn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hijvwlkm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cbiqngil.html


<!-- 参考信息 -->