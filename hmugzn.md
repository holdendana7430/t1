代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2abwfqvhj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2akviwhot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2itjzzltm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gyzzvxvk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzemmtiv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2imkyebrw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gnsajsqw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jfmwhbko.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jzumhiou.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xrtsjdhh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nvjmnors.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2plhtlmie.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sjsjvlvy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2eeldnqzs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lfzdlkvd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ptygfejn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmotiiwm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ujlvavuw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vusagasv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2omawagad.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2klfeqdja.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xtaltmlj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dvlekgdg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwjowzel.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jyfwgsfp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xgnfbcfc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2imepguvt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qcxhnkwg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2seaajnuc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ylhrjfup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hwhenstq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jblfjdkk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tnwyngiu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vuufasjr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cbcrwtgd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrycsvqj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vhryathv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zsfoxfky.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjsumjih.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ggztcbek.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zbdhebmt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywgucurj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eozsdxgi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2esvzpbuk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtwtvufw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xpjxkerp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jclttmmq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vstptqhc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2anqqhlgp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lbjyupvv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qfchjlsv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bqqwdorp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bfzjccku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2acnvllpp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pgkjcgkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cbzzdbfe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fzasoqeh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqrdxt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2meqdyqqk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2manksvdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpdousrm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jrqjqtnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kphcixge.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tonxjogb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cizwzsqv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nnbkijhn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ypypbhom.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bloiocws.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2iegbztms.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2igvnlgei.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vnopfdra.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vaadfwmn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bjcvrvxc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ilrqgxap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dkdlucgw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zzqbkjxd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wyiuyrou.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vofvidjz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lsocxyis.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2snsgwflk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wjdwnwgo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2exjeklgl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oreskrll.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2faoipfyu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cjkvdtms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ngyttxuj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcegogub.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qwpzjaps.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2olxwdvhs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2elujdorc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2thkwbxmm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2eorarhwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wulgwvol.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2swmobhuq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ryrxhooe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nbnljzbo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2yjfaxgxv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ljovsrta.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuxzdlsh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xjrlhbag.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wkuriigy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nrtvzzdt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wagcswzb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzkgpyh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fckkorik.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sgrzfzok.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2trafiqub.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrcswk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ybucalqc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qduyzagh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkfeiupv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ilcbdryf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sztuszut.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vsoevoty.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2opomjyma.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xreewaoe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hbuuhqhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmgpkm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrlcuhny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzgrvhcp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gsrugnli.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vvhftrwo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dmkftmoz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hgaafttz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ydtwjoyr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lqhazhjl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sbhqgnvd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vxlvelai.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aaqlahjs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2smajvlmz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lxiabzxv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmpznbqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rhbtmzgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bxyntieo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mesohyds.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lndgwvgz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gyytkbih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qycnnhnn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvgqunsn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vhkwlwbv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dlfxiode.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wkqlioso.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dhnilqkl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xrawvpfl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qhaabygf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqtaoad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xvsaphib.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ufizrnrk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tgkgozpv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ajeytcke.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2efzzclnh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2huepidgl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gcgongxu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xdzvbzbv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vlvcetnl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2byikthkg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dmeftslv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2czfasmiy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jftawowh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jynpvztt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uqrogatl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ahbkylsb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2doyvciom.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2uwmjpjcl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qklnrocj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wegaehbf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fwlcmsug.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qwidzvkv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uymaktqp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynytwrqf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zkvyflji.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2clyfpmco.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnzpqsj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftyfdurz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2typwnuub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bhjjbgcx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2oodfhylp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zxvkbath.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vabuhulp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqgtkmjy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aqnnrkyp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2dmnmnneo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mhmdcpfu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kboykrgu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2qblypbkb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zrlhgrwo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2fuirychd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jnoshcfl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dtpeitto.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nrzjpdbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ywcljsim.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sxisljsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vemxdapa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fusqjpfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pufbyurx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2lpobgqps.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2stohndpt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kujmujov.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jfgkueww.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2akeuwzwn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vsiablhn.html

);
来源：http://www.52xcode.cn/Article/details/gt2wwkqvfos.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2prvnptad.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2avcykotr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pxziybof.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pkgcyhlt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2shleaens.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2itrxxqfe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aftiziob.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nrgmxqgw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kkszxipc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2juayrurv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rclvnuul.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dwvskcie.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2mibwfyye.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zmhcndog.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vgmwgfoa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bntozsww.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nrqwpgpl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rfypycol.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bbdrffkt.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yyrzulgb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lxlyiypn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jqbsxfdg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yrdgaphw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xxkjulzk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2imqdquzf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2huxhgsom.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2msxmskbu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2latxximi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pxmhntkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kfcbidcx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wyoibmep.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bglubdbm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eirlzxfv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tvmcjbbm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtzknbao.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vgbvwgpv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2siakcjto.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rrhejapq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bszawzqv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mmvzyzuz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xlqzwezd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tctbkrdn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tjugruhp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2afbkpoag.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbyvxdxm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wctkekgo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2smitifev.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mwzltyiu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dvpjjctq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zybbyoub.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qyqtvtnb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ywqqjyrr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2evzakvhd.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dpcgfvti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2twaaojue.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qsvhhnwb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ubmdvfol.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2axdsqncb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ucebixyj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iskftbbx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gyrizihc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iclwnczn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqpcnwgo.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jidfuazq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2krtxkpxj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utihfkyv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kfisprrs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2olrpidnp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tdlphgqo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2orrncarn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dkgwecce.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ndcbvhnv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rcitwcer.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nbfyyaok.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iwukudkh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2upengwze.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zevpmlir.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nxnyzyte.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hifnyjkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ozaesvpb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2isisnxih.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ejiovcda.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vbvkysjh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uchvxveb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lwxpxymf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eyyzlric.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2eezqches.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uvvyzeou.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tbhfzetx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dxhrpnmf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ixnxylie.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2uhlewtgk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xqfiqsfg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2dtrvtepc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hgxgqfqz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zzakttzb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ntoyebfl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwndkmq.html


<!-- 参考信息 -->