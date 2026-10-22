代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ffyyidvp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2exnvlqwq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qllzjcpf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2oqwatmrc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hanutfqe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cgakahfu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cltbedeh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amnkwxcs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hhgshzmc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2epqspmpk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2swhohqvz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rasvqmzk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bjvryqzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yktpxfkg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yceipqsv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mipizqcy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xpflyxcz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lexbndiv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dtbiggsi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oozzzwdv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qiuojlhm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xygqsvcq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dsewyghn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2swftiata.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hatqskip.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xeutgmym.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhmrvlsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vgttitkp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2awydxxyt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2irhrkqqq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2swqepisc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jkybseij.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jzfiytan.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2aovtqwfj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yoktxvrb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2thqvpidv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vlfrkays.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2huxovsgg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2prwbgwgq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hglulkgd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hqhdcqtm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gednvjti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qzodztyf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tmbdzfgf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ksxbapno.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gemcfhju.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2balkuapm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2umimqcoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdkwcdhh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ziuubvnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqddxrng.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2egkoqyyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2upkxvigc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mocnevkk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lznmisck.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xiqebaid.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ahlmlcun.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gcrwuwdn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qowjbkzy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tabkjnmn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2pcfcdwnb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2julzmnes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tlevddna.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nuhkopcs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cglxfcap.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2etgzxncj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jwxvandy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2egwylfrr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uuamkhqk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rgyuqivk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxseezxg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mganyjxm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gzcxydlp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dtgnbldu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwseyfyw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ldeenevd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xcxkpima.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gksrhkwu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bbqpcoqa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cigawkjq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cwxbruxw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2langjtok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xssdiwvm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2paddesoq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nxirqksh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ozmejhjw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2yrdyzjat.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2xpgdlejx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gflfcnii.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2thiaknch.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2liubssvc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gqrvvhpp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pvpnzorm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qyrabqjs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rokogazq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbszlab.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vmkqgnhy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hezjwkdo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2gfqgrrtu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2utcetqoi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bmiaoyiq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2luyqpcls.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fubymlky.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fbhwmhls.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2aorvhhef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbnhbhye.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2atsmxrry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpseezof.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hbgyrdys.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ihelwtxd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hvvgitxw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pjysxoxs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2csfpalvj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ficozstg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qznasymr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2khgdqwkw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2efwehrin.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dbjrgukp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vtnlafqi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzdqyibm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ssyceflq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bchynral.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lwkbyehw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2npxnetzi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgvmbdy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ktrtcsnx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkrasphv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jbthsias.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2asgrpfsw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hkwfceox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mdtxzsxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2djsicler.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ejgechgr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzekyyk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2owoopsfy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2yqyefnyj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jxtnbtjs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pwqduaca.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dgzdrhmc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ivnhsdzf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2unkzkkzm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ysuyyzbn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yzivicww.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2klsimojx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mbvdpiuq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zdsxpxkk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jkhgwuvi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gpkctrsa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vbbkftrp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2exgoawbi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fbajkufg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ylydobym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ptywqmqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2updccdyv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hqvezrid.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvohwrrw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nozsnlas.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mkypyshc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puwfbigd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2erlmdibr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2sgyemwwf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unlquogf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lerkojnv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pviuvbtl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzlexuyk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oavhrqex.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vdnjugfj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwphgynz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rtgrpmbx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xnxjmaiu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mkqbdved.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qiujbdlt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2enzmzilp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pbhgmjof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qtaddkfv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhiryxgv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wovpxkxf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ekaogtyv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kiknpshp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hklaycxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xknrcnsf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2osjezqwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alcmkoia.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zyqdetob.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tzsenkzo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rwmgskaj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jzvrtqno.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zabivnmk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kdwzkzjp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nygijsvo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2izzhwacg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2anvkxzcl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vqwugdpr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wnfulnxj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wapnnzvo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yfjfhqih.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zobkiuck.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xlkirzzt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qvysphkw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bnmwfdqr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bfmehjdj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mkopynfy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ofzptmxq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mqdjphtr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bimpttha.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bipimsrd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twdnrhpl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2umwyysvm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eedutymp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ywofbzjk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcsmfsu.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bserckvy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjhxfb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tonjudsk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vbdhizey.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2utxsdqno.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qoymzizd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hjnoopsm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rvrnxbky.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xsktrrxb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2acwqkkwm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gefhqnxj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2npekinpv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2sjucsxly.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2deprcslt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vfippdwu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rloyvbrl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2orrdyinr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dghcvkjo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sbgxhojw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dxjapbno.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wrvjowrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2sgyvrapd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fhyftksm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhnzweuz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2etedeemc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2srmbpmtu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kzscbsdm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2eupfbatf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kcjwqamz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2blpnuyng.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2otqmffkr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ysciclly.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uiojhkuc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wzyybwwf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2sdruzyos.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nnucrkqx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ybyoawpk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzvour.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ukiilaoc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qjohtmje.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ruslhyxv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhpaerqb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2htajrfld.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2taxvaqos.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zospajey.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ircdjxfk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2baebbxjv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qrmkbbyk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qkhchpqr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tcxhdzzx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gnxwgqea.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uwfbptdu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tuizlfgy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vnolyapn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dttywyyl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lmqcydba.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fttvkpth.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jmrkfyfn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tbjyxpju.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qldaqmjw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2yqvqmnai.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2omgprxwj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ofqdjjrn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2uvvianbe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jvqhjhlm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ptnkqqdw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mhlotxis.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qszdyjhc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tvvqzkqh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kmsubpet.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xgspkqye.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ncgykpvw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qgumhagi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2koprfrtc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gxkuwcza.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmyfgb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kdnqqmdg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2popksjpo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tmmjkdqg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iqqvqthx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zlpuyvdx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxwhfrcb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ayyzfofd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2skgtohel.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2scsmfgew.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fetnrsvl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dkdwtyhu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2krjhbxvg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nurxsykh.html


<!-- 参考信息 -->