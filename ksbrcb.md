代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3esarubkf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pakuzrld.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ykivgura.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjcexnol.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3turvtwqe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nktzrxgb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cclpuqdn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hoortcid.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oppfsupe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hvfwhael.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yfskagjj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aybullza.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3spqfylih.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbcwshgi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rdrlmglx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rqqrbcgr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yprozvnu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3aocgntrq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3inxapalp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ratitgjh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ivvuqpmz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhaainh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rhmvisvq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qpuuqaim.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qoxaqpna.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tnqmhemv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kfdbopre.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nxmrwbaf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifskwyrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hmahkqyh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3napfyghq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qewlluja.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ajctwmho.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xhxmwoxx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uuvjlexy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wuxuidye.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hrxsunik.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3glworkkq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3btqbrkvw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ddqdzywr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pnqcogbq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwpfyhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3flpqhyzj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tfrxepxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulfqdsim.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cwtcooxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmsllbit.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kespgmtq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sprcdjxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rphkxxfp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3paonxdgs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pomhnmib.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cjiqpnbt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wlyldmuz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fmrehepa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oguxslrb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pbhvlvzs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ptkzgxkr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3yxabkapq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ofpiioew.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gcbbixxb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ntxhecat.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gznawvtc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uimnhycg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jnmqrncr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qmhmqzpq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzexscfp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fvaqycne.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zoaxkucb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oqpwlyzl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uagligud.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lvolnlty.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hbchpxyn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lehcxwvv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hdzfizuy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hykxrvub.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qignrwpu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlumytp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3epkitfdu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3emqftbwu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3miwugpls.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vcerwsjr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxbklae.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nwllxyuq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nxzrhkax.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kftfwvdo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nvxynkfr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uynrasmw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mrggxyne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vlzggega.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xlqvvxpo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkjaqej.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gxcfljnx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3foyzsetu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uzpekcgv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3utmzpgge.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wfucfwcv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3twtheinx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ysdnztjz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wzelaadm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hpcofnxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blkdvska.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gweqskpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncvlbfrh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fwqvwids.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3avpmvraw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ukgovfbl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rdzvoofr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jawgjdwe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yfhvsenc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tyedbhke.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zijzacnh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3guolkcnl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3gjhnpfpw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ouawbhtu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uctyqpmz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hbdpqbcn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yywfqlak.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxygiog.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lirzdtff.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3figjwfne.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ruzttcjd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eynagdnv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zjoxhgab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lmkckpen.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wwomrpek.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bqzttpba.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3twsrzrkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lmnjgooc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ixyagszn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3mpbkdwqr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3elrfaxkm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fmicdahi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mayrubkk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kqmgscrh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bduxyowg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bzomhcni.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxtmjwo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3khrbgcrl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rdzbftlj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nlzygwrn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3esvsljjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mdpyhkxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ienvacrp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pnidqlxx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wxzkzsrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mgwcrpcj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lmpvcbak.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3nkikkhby.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zrxtstqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3deznfetw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfztedkc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cdycxyqi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jtmumuiy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ffviosae.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gklmzcee.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bhioyqts.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3utfhksiw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wanvkrib.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3msspjcxt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3whflajne.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oloqyhzp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uvkkvosz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqdwywqa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zxstigin.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qqodhuqi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3kjayndjs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qkmhlgoi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ruhhafvk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xvslbxnh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3buulugij.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xunpcfll.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xhzetdzr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xlnzbggh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmelehil.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ceaijagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvinkptd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3keagbbwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kggvfdit.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cmkxiejp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dbwooouo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sgoamubg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oqawvwjz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wucybwzc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tkceoorl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nzzzfbpz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nduudaxu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3arbfkunl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nfngabya.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nfozjwrw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3vgqiznqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qvoohjme.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjbwtfr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tehdppvt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mlvunaky.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvfvbrjf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3nzjlyerr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xetsotwz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3amcnjpjd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kjjgdjpa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3slsdnlio.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3cdsbwlco.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sjwzxdcg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vropuxdp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tymjrnyf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3kqancxiy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3txqhzewa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yqtpyrhf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kltjgiyt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3oigwijef.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dvxgychk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ioiddsws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xczwgsii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dzkpwmxm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tpdnwrrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zgmdwwsy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3svblingp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3acxlgpcv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3pdexakvk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3trzdrgqi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qunaxlal.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3glbfphmc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3luckzpni.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ncquwoga.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3liixuvzu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3oriscekg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgrbhb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pdiitixk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ewfscgwk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3feyfdduq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3awxhpyui.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3khyuckoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3elkjfoip.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qbsgfdue.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pxizwgcu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3brkhhbkk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ppackgyp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fuclkhru.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqrmqlup.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jwclijjt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3brrouzlr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3egfzkmoj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kulzshul.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qiroljhs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqtwgzgo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cmkxwzcf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ejgwblns.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xjhnacdr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbbusrse.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qbmtnzli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ztkqozds.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dmczsncj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3izjjhljw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wulfypcn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcigvp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kyeeuapn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xsnkmnhx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bjpricmp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ubwtksfx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rcvoylbd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tczivmnp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvjastwo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cwwsiish.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgcvpifc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ymvaruhs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywqkplqk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jzvknwzc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qoshgcuc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dmurxzgh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ynmcdqnf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hkbufvdf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkcnxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3enywmsgd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vjchemdh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rudednhk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wxswxolp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gcgdnnny.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ypjeahbh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vuhremwg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3koytolbu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ojvujfcu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhevtot.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tyghjkdk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3skjfzfck.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wknxpajq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3exnozrrw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rgwgimxf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xrcaunjl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mlezixst.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qxovdulx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxyyde.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hkkhzpwc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tjhqkmdb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jqllcxnw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gitczqtf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fbglgknv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lwrzwrjk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmkcgn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hnsmhyic.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sxhdblue.html


<!-- 参考信息 -->