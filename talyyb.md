代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ztwtcpmb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ukulezqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xsoyevpx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rwydsekr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqnclwci.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ojmhyvkd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvfmlonc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yvlqjzpd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fptqaiia.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmawctph.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yswraueb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3trnwslip.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nfdsmjig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3upmwnamu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wbpjljss.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhtvibsh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pjgzgrwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kcfvpydr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jbvidusv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hqerafww.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eptuaerh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pzfypsdm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cgwdadcj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rcyrvaaj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wmaqzhwe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdebhiz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ruiawccm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nroxbhju.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3heeudpkt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jmcwnulm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3iwjgapgv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dptkhjib.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vhqzjxmb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fceyuwbd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fhkbuaia.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qrjjaovl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3upmflmuu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pfsjljyx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aubbjpxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fsticmhr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dzqutkya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kdcmaukb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uvqbtugv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lesddixn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iekpagpi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vveiprvv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rdjpnlxb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wsuvpfhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdobryzg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yxqhqrvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxizowis.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gurfvowv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pvfspfta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fuxgodqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yamgpebd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3omxbwrup.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ixwhqtio.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fvhbpmwf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmddbqk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cxnusnpz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ksykeikm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3irycrxsd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dcqcraqj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vhdrrxnm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ycupoavf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ncfjlvzf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ocufohbl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ecmebysv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nuiticjg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uwaamfya.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ceugglfh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3taaqndvs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dxhdpqgf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eeaflzlk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivmmivyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxldte.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfvmzfe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cswvjmrx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cjvcbzut.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3valpidbe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qrzmaiuh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oloycwsq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kmqenugp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pbdaxime.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rschmryd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dlkjbdub.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhlpkica.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vkbsefhi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vbtidmqs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zbshvltt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfigcnq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyqfowx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3eeukvxnx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jhqyqglp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yrpxqjru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubokdzdr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ohyqpgdh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3eepzlmzt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uhfeiauc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yedomfig.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3afrszujx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xoukcxyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wrlghqks.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rfjbxqke.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3wdcfjtuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aktbcoun.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3juqbumdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcgvbwxo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3myoubrqz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xdosoifr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3suoriadl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iykyfvqm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dxkcgtdq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kbqianen.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ulduyzel.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fencnajj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nkgzrjab.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ahmsrycq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sralewmg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfwckel.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oogesywz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tuuiyfwd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwrzanm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vkiimkls.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvfkwps.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3oqxnjyka.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anpexnpn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vbbddcag.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tzopcoch.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3stnlackj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fwojltsi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3quibuvvf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3axwfotcg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3szrxctfe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3eueghpkn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ihfoogwn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oatyeawe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vbjhieoe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zcshelqo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3andhokay.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gkewwbme.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xtrshojn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fsfomwqt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vizptspq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3nvbpdnqo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3iwyjxhts.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wnrdyxmk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3luqbacsx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yqnazfwh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mxgoxbew.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sloqhlnc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wwkoljds.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qydyvhle.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hnniaslb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pnmmiuxr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azfgkcqf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3umtbhtha.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3thoupgkt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dptlggqy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppbgqnue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nhrqmgjk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neqjteix.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ylvdigmd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rafvtuyc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xvcpqdlw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bhocsitx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qkwwfwwv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vvphlxer.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gdzglozp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kxahhqhw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vvrzjvao.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yskutnuq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3djytdlxt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vwxfvfal.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3unzravzr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qeowxkuw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bbwartqc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hrmktflg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpycbna.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ckolmooy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqkzsmaz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zwvokzbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwnlaobj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xwsgndgl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xnwgsmea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cnpomwxy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yvchmhsv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lxlvkvkq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3svwxvrjb.html

);
来源：http://www.52xcode.cn/Article/details/gt3wdiepexo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqwfvr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3twwiehjf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3srxufxlf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qsqsenwv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wlnsjsjz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3arqpntqr.html

);
来源：http://www.52xcode.cn/Article/details/gt3oaksxrdc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3skpmuwof.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3sthnirlx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtmsevqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jqehozrw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3otnhwbqb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lpdayhos.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rgqjbjhz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ehugpwdz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vxyxbppx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3nkfzkcrg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gegkzdtr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fynecahc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ldldwshw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3joiqlpcr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tkwkghgx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yrihoael.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3otdzercf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ipsdpnss.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kafzyfee.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ertnnuil.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ijfdophw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zyxaxzqc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3knidmbqn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tbjvtput.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3omexthxj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3rqctwjpk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3knktfhaf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xsdfimkx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kfberxyt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndprhsyj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hmyvtowk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lqkaxnyz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rtiotbvd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nmgkudjp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yaitcmsh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3twfquzpy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3rrnxzcow.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3kfdemepl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ytaecvti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3klkxqxhw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3arwxkxky.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vffypxav.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jtpydzte.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zjhqbmpc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3odpzgkgj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3olwugrid.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uhyxjnan.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qfckzcas.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ilizumdt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dpawfppd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xelajmqi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbuwcxnd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zxvbajpf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3scdaiaxh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zsgkarlw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiiliubl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mgqevaef.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cehvbnwq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hqtlxgbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkybvd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isswkwbn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3athafgzb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jipowany.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcbwbndx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3lkttpfgg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sxchjzdn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yjjvhgir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3exozeags.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vpoabdbq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3iqaizzmi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xdqesxue.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ypatdbbv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ivgymhmt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jvtuzelo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3atwqoxjd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pvromvbd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3upmxmyxx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpucmhxi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bysgvzxf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cwzijdjg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3brmvvmdr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qfrbrejj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3cclijnqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ixlipgxi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uvpmdzhu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dgimlkns.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mctrvwoj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ngewpqms.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vpowhjlz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sirxgscw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lcjrypvq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hnpfpjij.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cllionnu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lttlsazf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rqgkbjtp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cegigppg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hnpfjhsu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3nivshsqp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lxgezqbq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eavvyirm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcfmzft.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3leicygfa.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ekzbnomr.html


<!-- 参考信息 -->