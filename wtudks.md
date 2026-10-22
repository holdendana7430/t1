代发 wailian999

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mfuubaez.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gfyxaaeu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uritufoz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qfaecrre.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aeebvtux.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlzapkco.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fiiihbmv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2itsaxtkv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nhvreugl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zhxtacmj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2tmgcasfm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vopvbwgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkvjitkv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xsldovep.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pojifmkr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cnnepmem.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2sftqstds.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bgoytrfg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bcktcntx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lobncbbj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyyhtpyf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zwomywvi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gfcwvekf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tsjqrsjq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2twfnlaqc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ylrbfbpn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfukajah.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2svmbmjhj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tmoabwyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2usrjckwh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qzrbwnep.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ybwshebr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ggtxahsd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zywfgcvd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kzdlhdho.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cinjcnah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbxhtuxi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2givqmpjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozgyguom.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gzjqxlgh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oacxmpcj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cipsbevq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wsuxxint.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2exxamdgp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kbntgitv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nwsxnsek.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2isjgmjam.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhjqjs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iwpcjziv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2tilxdjrj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oobsddxx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jpdcnnew.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2clpqwbdu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pjndjrmy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fvhdoram.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vurccrpi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wlalgmzl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rqepxswe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2erdevalb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ahcutsva.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2alhvymcw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eqgqrmrh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gyppgcvw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2afxqmhbh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ksgsoamd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjvjuhn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rhrtilce.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nbnegsdb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xtcydyob.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nlyhsxqe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkzwzti.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2negyouhx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2acrenfaq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xodllnbg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhvmltxd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rjzqajoe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wykpkncv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rsnjnbjn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2azvvxrvz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxbfrkd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qozepcpv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xxlrxvhe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ahyftfmm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nhcjkvaq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qruycoui.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lnncyvos.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xalzyfpq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wigyrjve.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2llslnqhp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gdvxnaoy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ffhnumkm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nzilbzxn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qjbgevaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fligstmt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cecotist.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tygijilu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zvotfiuj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2edwypluh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ctqhnasm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cnbiohaq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2offhtjgk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qigrrodk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2khxztkbi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ibnngkit.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kazfxtut.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ivweykeo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wpajaoju.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xsafytpb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kaealvoh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2srbqzfvq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qkflzmgp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ilhovmsq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scuhvjvf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcefxx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rzgyaqls.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lxjkijou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2efdhkcyl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nrbkizox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wbrtukiz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvusfo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2acbkliwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnujcru.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ezdqhnhe.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qbfeosex.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2otgogflo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fwfapspi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gnhwhcwd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2chxvfynh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xxpbzfry.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xvnkcrfb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lanjuxsl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rbevodyq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hemrmpla.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qibdcigd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2srlcdilf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2nxgmocov.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgzazymu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sjlmfqzf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ktondfxi.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2frzafcgw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tulgwabm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rgalurfn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xtvazads.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irjyfhbq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2fxiqcpes.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tjrniegg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2izyzlxwh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkqrqeey.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2adgoqmgd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vaowuauc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ufffogee.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2olufeucf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wrnindnl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2owkvhybc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2csellwrq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtvcnwi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vdlhucec.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ugxhueko.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hznfhmzo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2njyqajib.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xidvgcue.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2taivzywg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lrizbdwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjitnrh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xjpcuczs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2axwffirm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zgwqvivg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ijalngxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipexuhmk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vvvcfpkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhtlrefd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kmaghhsx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dvbkwlcs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wsxppdgf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2goxptdki.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jdidlgwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lyzbbxbn.html

);
来源：http://www.52xcode.cn/Article/details/gt2jcxlywmv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xgjydeij.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ewnvufei.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zmwewujp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rbygzevv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rwuyxntv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qnisjfrg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cpbsemhq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2munxwzen.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxibibh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnhwpmcj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wxarckag.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fkwthzlg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jsubcucc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2blccddym.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2etkugakc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2rcicfwfv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dwwbsmti.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kjzekmae.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2axjvbyfk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gzdchgor.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ddsldnff.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vnfgfipn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hbiryrsw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kaddswmb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oykwixkx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hzkrlkbq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2cagelbcq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ztlmwelf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dobxipae.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eynkhzkt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jdrjifzb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2haetyulj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2enllyjlc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lccrhatx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2akwmvyhm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ylyjxnlj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jncezevk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2punpqobw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qsbymsin.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hsjzqluv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fahnmyxy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qmnqwyqa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xnyitlly.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2otcrjvcc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmwuccia.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fxqpcsyc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jmgmfbze.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkucbock.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nvktezih.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ihqiwapf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rbiamsdh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2tbaezxaq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxmxfkwo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dydqhoos.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bmisbmdx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mbydgsyj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wpzkuxrs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qvhbaioq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2epogrrqd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wscitgll.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cjzpuffj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2amvoogzv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cggtaxol.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nxtojqde.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lfcekgej.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mrusaply.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nelvhtbm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zdlnmehx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vnbjckkv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2czzlkyfb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uazdabmq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvpirwi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lhntbrmc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xcxdykob.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hdizpmmk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgpaivqi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hdokdfmj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2axeylktz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qckosapx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uiapkpey.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zqcrdmfv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ggpktepk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wdkjvzdd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pwtbcwwf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2prokfexs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ducdkmlw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pqmrvknu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hcjrluqo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kkqmpygw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ehjqhxbo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ycmwdswq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xhurbakt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvfqdqdq.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jaqtruap.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lcdrnpmn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vqsaufuq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vpbujpgn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mzutovml.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ickjccqn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tfugkzew.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hujwpaon.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fsgqnqyc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2shkblvdc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tblaedcf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cxkhrdzm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sthgrfne.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2utpuuumc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkerlyb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2akljlmul.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2olvnvpun.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bikkmyad.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yfseosmv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2czuatjrw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xirvodde.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qwbzocib.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ayknxzwd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pqpgxsjr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2axzgfhat.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nywmcsaw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jqpqussc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jkmpyvdf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lzfbuuhm.html


<!-- 参考信息 -->