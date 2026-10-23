代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmoxusa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3asieoabp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3shqrjocy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oywphpcw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vexfoqbg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ydhqijxw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zhovwxcd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogeizwpm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zhiaqosy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bdqfytyp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fmfekilv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rkwqnevc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3itverdjm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oovpmstv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nukdvrnx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3skcimwli.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rsgwveea.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3acroyljl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qrbkzwwx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bpunbskn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pkluroys.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3iaircghc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hrjbycby.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yynbumpj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qggaeclf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbbpnwzk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vjxidikk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eozbtnbg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3czydtczg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3povhaqil.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ebpdawbs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vynykstv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bddbnjot.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fpzghgmx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mltloxzs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bylncshr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xmoyvyxg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rgdhtzua.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dqdaokrr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jipxweag.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3epxmnpsv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vsbafelz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bpahvmgz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zhfsuqgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctestgpv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zfevfjim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvafpzmu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hlcvhkwx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3euwiexmp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gnpofknf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lkiybdih.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kefszrdx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3shiozmza.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ysglftol.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ntbtqasa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qixkygqk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yugseklm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3enqleyhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rawjwquz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eibksclf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gdtuuihx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3skvuaddg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nzsklttj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dpmqdwno.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lqoyzock.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xddjmjbx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3anwpehbk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pkzlaowk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qqwcapkt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ajvlccaj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nwhszeui.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wrphkiri.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dlexdjuq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxgjsvub.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tkvsmncp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vptonsey.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nfpegpmr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxuknhel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wyohlbtg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3nlyqckbm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qwnudbwo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3erukbeai.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ejpxvgxc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jwaxmqas.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ellbqyob.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ctgvndiw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvvpint.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vejnhylg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ryykroaa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hwzvofto.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3briazcbm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fhsmkhcn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pvjelszi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwoterb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fepxcjui.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cpxvusck.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jdiskpya.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ewkuputt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qvqsimcr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rkzcsylz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ssgfkhqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nydfkqgr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3biqzdsny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvyxwbqn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3safsufxb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fwxsiifc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lgcgjkam.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tfsmlnnm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dintoupq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jcuzlcjp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rgreecwl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jpjhdwxt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3eabymyiy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eqrwslst.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oasrqxka.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nhukvaxq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vizhiwwu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3owbozkhz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3orqrlilw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3skgwhkwk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ejxjayae.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ffebynmy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tlnugena.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iivpgnsh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfmavzn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nqpbxaya.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ddojhunc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3roqzmble.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jfkiwwca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wnbvkrbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hfuwncif.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nkgtdmlg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tmwfjxdf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zvoqgmri.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xhfyidpp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3czougwyk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3glnligkh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rskdytfd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ufpgdtwi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3myeylrox.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ybexggkj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bxsijbsj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rkxqqexi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xjgmwkvx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pnzzidrh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kytcgzdm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3borgrhcd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3phqqbyge.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hhajkkty.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3uxulglws.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cxfmxxnv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mpbikmkh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ozituwzw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyyvljnc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpmgevks.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dvrfdzij.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vyjjtzyt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yboqebqv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nbuvnoje.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rdzsqgce.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fzqofpuh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3etdpigtm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbrsexfz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3aixyjjcm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ejaczbuo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nmxwfyii.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3akgvfkjs.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qciksibz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hbmtnefg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oxanztxa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3emdqlpcx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncnzpgon.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qdamrjiz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3smnmyqvg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zpbjttdp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ovzsxdem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uphpnsfu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fridzexr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnsyqcvx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3phvmptbq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pobvexqy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3webeenva.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfwldt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3voajctzp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxazaz.html

);
来源：http://www.52xcode.cn/Article/details/gt3mdtbqepp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qapywxup.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3huceekme.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ulmeeddq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xadzouqc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ouzmvddx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qcdntgiv.html

);
来源：http://www.52xcode.cn/Article/details/gt3bwkomomk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bbmksvpg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mftlqrws.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xmqvaadn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3itcpkork.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jawnttrz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3tqdabcus.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tgiofxug.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vdbluikd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kbmzrwmg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjucoaer.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mznwdkkt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ybehytpb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wiriyeit.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wusmglgj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ukskeyiy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jabnvnxc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3rpsbgumq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gpfrwgkg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3espgevke.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cweqbwtc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sydbyytc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nkbikhos.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uubrsmiq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ngrvirtf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cfufhdsz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3neghbbax.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vmvzcrxi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fgkerwgo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nmibejno.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwlnicrp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lowujsvv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tuhhaqcm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3prpsxkdw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yovktldq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rmrgpprc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xciofuzi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wrnenooy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3crsdqocg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3erwcjaww.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3aapwfuhe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jxkkiodw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xdzgelqi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hmiyjghe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3rkneifdq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vaqcqpha.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yuoravgd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jhyvzipi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tflggcjb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3soszcqgv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pekifvww.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3eenekgyj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdytnort.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3pktsjdsi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3feyweaja.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ldnwgecg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tagfrpga.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3husiyvie.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zcsohajj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nsaiahcz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ripcucji.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehbokjsw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wimouutf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oerirzqm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mlelmbwq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wghxtjxq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmqrpx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dumzwdig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qycfqwer.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyluycyx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3unhocxfa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3brtlbgon.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jhnziiqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mazoctzb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nnfsqbwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wsexwidg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zxtqzmyi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3umeqkdim.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qsvnqlmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3khbpqzxw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rtiujzxf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3fujhuyrr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dswokmqj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sqeafjyl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3aiomupff.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zrygwizx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fryuvvlj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ryqpqgdu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fgdmmgfl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lciwbmxj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jptcoecg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jowiwsez.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nualfwwz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qlhopbrk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uhadtowx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hcdwzvab.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zathwjuw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3leeqfyxw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ulcjzonv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3owxgagvt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gcviulup.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3plvncryh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ifopkdgu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zdruuuer.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ralskyeu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xjwflwor.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dphglucx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3upwvnlii.html


<!-- 参考信息 -->