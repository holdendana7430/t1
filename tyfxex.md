代发 wailian999

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2soyqfdmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rtqkfwvp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2efrfjklb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dihygqtd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zvpgaujx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kslvpuqj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xjepbyrk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xmwmdbsx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wwdhqgbs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yijbweel.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kcycnbof.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjlhonur.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmegxell.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rdbehnig.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2budyqdsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2djbyoysa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2aoitbbfz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2loqphzwh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2didtdaru.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lgnuvgcw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kywtdrle.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uzjbiqdf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dsxtczqc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eetimoow.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2unhbxrbc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aveckkyc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fueqioae.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gnypscev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jkmeohjq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dbkwnumx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gwcfpgrg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2puxxkmfz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bsuydfoq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yqsukarf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqpxvpa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ngngfofl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afnzvarj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cunuvehx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wteacvue.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vhwukhks.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rlosmjya.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hemurwkf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gokutxsl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hhobtuty.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kcstgxcw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jvuwjvwc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuupdtt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wzozzqoc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wjwyvuqo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtyyqngu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2orhpmyhg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kcaquoud.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lzdlqqck.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2plbubdrn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vrpfqdic.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2oojiqrxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qfurhjwd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bnsemldj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lnraoyzh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wabksqmk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zcvnuyaf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wqnfibsx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2befjhxln.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2afjdkocl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqxbxkk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhvekyf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2errrxftb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iiusksvk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vunwexti.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msvzrjvv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2izxjtnwr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2atahjdxq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zkdvndpe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2utbqxivy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqgernvv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dzzsocfo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qqftbhcd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2foiduwaj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oajjeinx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2obnwqzmf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vfnqswhb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iuztihqs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tagqwusd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2beryctmz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gifdrftc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vflweliu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xjogespt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kqpbhgcj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bryhdjbx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qmfduzea.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ahikfled.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ujqumdko.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fuwvfvzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyzvpueb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sovlgguw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbjzavhk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lbinrapg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dcnqkuri.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qyjgdurm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nontprgm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2idhzocop.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2coljzelo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2clupgstr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kcosiuhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljyzkvfu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2khakrxbv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ronedsdy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jyhnjeyl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2awmehoyf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nokbnvll.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2keqtglei.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wiezasdr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vbhobwgd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fdzxfete.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2byxwrmwt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wkpkpcac.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cnubhecx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2anevzptn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cztmwvjq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xaucuhmo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ervsotdu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pfywemwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dboysmel.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rxuahtjy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2okdjbgrj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nbzgeisd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nsydnrsi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fnxwqkiy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2grurcyuc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uydqdajy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2elqgxusi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hdmpgghr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kdizzeia.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2covqhhyn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kkzmmcmu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zxyrmoaq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qkmewcyy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mcfedmgu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2brmyznyu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xcboasrr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2byjvbbgo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ctidylxo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pmtuavom.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyepygwj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pvbahfzf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wvvrvpmd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfoucfwc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pdqhyxuj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xbpmpdev.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2sclbqgas.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dlrymrxu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2taczdpjf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2hjrbtika.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lxhjpocz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2giblsjwy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rljoftfs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hfrzyuxq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ymzhhfeu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ibdxpduq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dsgogjxw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mqowxbhb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2qgkwtfdw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ahosujpp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsipjlxn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mgzbdgxp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wnwvhqec.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2aohkityo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xmrhxvak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfbebcja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jmehggqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyudgtsu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sbobztoq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nljljnov.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kgtbvrjn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jgleplcw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2pxaqioms.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lrdnrcoq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pezjoeul.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2idsxmeiz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wpxooxhh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wcyuivan.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2zqkzabgf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nyyjmnak.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yiyebxsa.html

);
来源：http://www.52xcode.cn/Article/details/gt2eguxoyxo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2dmvfuhhk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kwtbgwlf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2awwguzmc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kwdhkdwz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gmjvaoif.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kcmaxaza.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yksgtpxr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2monvnsob.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jegsnykv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zhngsbyq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovaceknf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yfnoeexy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2czuqzmgd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ejrnubdg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ngszjcba.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ezpqrdbe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rcleeowt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eggcxydb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2womlkhgl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2sjywycjo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ergehcml.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2inycftnk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ppfokuwp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gkviaoqs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ktqylhnx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xodjtqwy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2izfuctmy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dsxvfete.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ukbeyelb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wphryvpg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2udtkhjkq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ckxtbmlv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nxngftkc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jeibtinw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqeyfe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wjgxgyau.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tfrmgbfc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pubbqbsd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bhvlsyad.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2skbxyhro.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2oblcwwgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nsjxsxow.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ujvkmvmn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ophczdyb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2woitmojt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opftnwqw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2twvdcixi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jxkpbjow.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mtylkomv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itrgqstr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xieeluvb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lldqsvux.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tpronzgm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oixayndy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lfyrwpfp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvgrxcfx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zgkgyeax.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jwfsghep.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gxwtqhcy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dpqvwtou.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bkwktgkl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2udjjwhyf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xatviwxx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pcvmghql.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zzxontox.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cfxoppmr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pqqhnodi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zveysgyt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vjuekayo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2luprebev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jymtvthe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2imivpgmg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iphdnfkc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zdgkhtet.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejrwivgw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tsswabjs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rvkjzodg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lpirpuqg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2kswkwnes.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gcxvnwuq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bcaevqvb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wtuyznra.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nifbcalv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2elzfrexk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2igierega.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jtldavjb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ffnxqfnq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xruhpifj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ulqshfxz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ymvcppsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dzgnxwws.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2igpjogon.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bcmweezg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ptglsyfl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jdvepjsh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gkinwoso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2juzeglib.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxfhgq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qnfvxwkp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2svijghov.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ddfovtxb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2skebcbwc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xumhdglc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zwihzdib.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fhtlaxow.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zvfxdobw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wxagdksu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2heytfihp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vwzugwnd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2giihmpnt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nbepwvmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2liqzbcsd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ifjfvjbt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vjpuyedi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wysdnnla.html


<!-- 参考信息 -->