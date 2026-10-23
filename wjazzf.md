代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldyukhid.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ldojmyxa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xyffskxf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zklqenmo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cigksndv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3npaxignf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ubcwetiz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzgddvah.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3chdebdwn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lnyjdzvp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jxiqqjou.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xwbubrjo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3crnepqrc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qrztcajn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ncoeudif.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tcruwqgd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qscuhfqf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ydqeejal.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yvghopyl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcplcw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zwiweqyf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wrhmiduc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3txrnjcqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oidegpqv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dbjnjhag.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3oqlsindh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gcnwvxwa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3oaffutai.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3momgcxbs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vbmysxwy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bklmitkd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gipjfzkt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3shlrcphu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3aomcptdl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kayxcqzi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lapndtzn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3iewjnkrt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3agkdiahf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fabcnkwb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cvdinezy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pqhubphq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qufdwazl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fodwvpkx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xmyjpjxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltpdyotx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fyshxvwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckolidym.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ynogfxan.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mhcevufv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ytbwwwzm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nctbskgr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gwtdgxra.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwqurpk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sgyjfnyt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hloqakyc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rbjfnevo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ciyypgyc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uiufmumg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aatvnjqa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rrzfdkoc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3udiefprp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdouzyb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jfekhang.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gqtvanvq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mlusqbmq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fhtgxubq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhidfuch.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fbdgkkim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3htebapco.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sdvsqtmc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yqcslpcy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pnjizzzj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tqhhcoag.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xhhqxppw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3khcbbzfq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cndyvjma.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cpzkdtmb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3diwadndk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wmmpppom.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jtgitdqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3adfwgalk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jfvxcdtq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nymkwpyi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rxkulzsi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rrfvovck.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3arrullhw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3clzsehiy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qdzpvidy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hyjuzdkk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vszaspmh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iswzyner.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hqqelylp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ajekptun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3owljjacp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nqjckbbx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kiyrkokm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zfrfrixw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rkygvwtv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3aanquwov.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3sgjczeoz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3irsjnmot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzruzyua.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpmrghhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfpgthcl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3txtgaqhd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3opwzeehj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3itctssnl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3edxcddeo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jiwxfozb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yfpukpxq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3npqjjtyc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cqbxpckr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zaxjqtrk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yvunmtqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3temtlezw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3guvjnrac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3xqkvejgw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3laliebqu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3coapykje.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rrkjhiyi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjifcbx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lmnokbhm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cbpzasjm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yuzskenl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gfctynnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ugddxboa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lyaftppl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3whsytbdo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jekblgra.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eakgdegu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vsjsthuq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3izjvvska.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ikssfuzx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rizlckbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ryiozigm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3svcammmi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iwuglqaq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qraboabu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xxddhqeh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uskbhgor.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wnbgmpic.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3imfnlljx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3iyxlhwqb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ltdduidy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gyewcdhd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3axohkgkn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvgfoft.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zzeswguw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wbpefgey.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3mogybqjp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hjwciuzp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wnmsmyvh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ixdrhglv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3unhghnix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hiiogsll.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3srayjklv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wudfdpzv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcwvujfj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gqplqnmi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ublxkhbr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fpshwehe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qjmweahg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bznmcpoj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szwzequa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tidsynfk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwezdfbr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bffnybnv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pbedifqn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kbneypxd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3neswrtlg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kklkdpou.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zuqlniun.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hgdvlczf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ktmgshwi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hcbymzeg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pmwowedz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgpsjypz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ahcuwodw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvnewtfi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zczafrus.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ebaxjiil.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xitnaeht.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fjulyugk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3oaglpsvz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mrglqnmy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3usdeptck.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kzluvbex.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wqqkxfbm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jeedicmy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hwzimgsr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xihzcwup.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dlseogel.html

);
来源：http://www.52xcode.cn/Article/details/gt3dggccyet.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ctonaxsu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xwcxgvhj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3jpebvplh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iugaghgz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3pckzmsob.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhspxlgn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pdsaxbcd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fcewxdnc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ofnmnylo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cdqfhpew.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rrrxcqlf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbtzif.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqumaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bprkpsgg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ziqyoofh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3enguammo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qgvnyylh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3emczkfhs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vnhpzdup.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xbwfqsvg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3prrncazg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tcphdxmf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3upiiooql.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bpedoivx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qyrptazy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfwzjtj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qcafokwd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjjrnao.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zjuarxnu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axcwzkne.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hcifbcnk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcgkbpdo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ibfliipj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jjoxdydo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yuirhvyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vhnvicfe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wozzwooc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uyvzszeu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kllozrtg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ontckkes.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wbejaulz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nnjzbmtb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dgxwsdbe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lgcdwxis.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gugyssdv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfbbejni.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jbcftqaj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hcqyuhcp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hbjehpye.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eexdhgms.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3eyqzjtmb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebbldvjp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gjfdawlj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pvfyacmf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yfnxuhes.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aqyrcixw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3unkaygmv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3suwcjplw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mmkiitwx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bpyvbrmu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjhawzvg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bjaglzuj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3twykauxw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zlwtualc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pmpwtdag.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3llwrlezj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xvtaiekc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uhiaigea.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3khuqwcag.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hobwolom.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sqgqfter.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ifhuexcm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ijwawjbs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3qcjjxtne.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bxazxcss.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ffgvvkkn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xeqwbmlp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3hmzumuvw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zyetwyrn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3prxgbrbx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3deonggts.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3uuthdhfx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tyxrwklb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qvkdisim.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nbcssvba.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3shsrcmfj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ntqvfeje.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3prnqgrpo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dqwjnrav.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gxjnvlmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tapubwve.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qqgnzisx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zfbjmfid.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kjxhsati.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hhnqgtwr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zfouaxdg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yugsmtwl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3eypzednp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cxqedfgu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fwyiutyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kfakhedm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3matiyexp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pozvuwdc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3azruwveg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3crbglyje.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yqcifwml.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3chstjvhq.html


<!-- 参考信息 -->