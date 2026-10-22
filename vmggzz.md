代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdxcqeoi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wimhfzsw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ismszvok.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2giqxkmoh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cictiybe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fzuienzq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2teqfocov.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yypaxqik.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oauorqat.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qpnskqjc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2woocknml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gngmqlqy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ahysqcgu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2elvaorva.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ewavljrd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xivuyxee.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wqlrlxkg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2dzrbzhhq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dtjziseo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tzobuztr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpsyyojr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ngapeqty.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjrqwjta.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2scohnfks.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxhluuxl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2osldahcv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kavpixlk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mfrppbgl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rkbimvyo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dqqclwmy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dxltpkxq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fjpmjgbx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hdszxehw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kecwkwwk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2upvgepsd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2psxirxgm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qymlgwwg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xgpqocfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mwmjmbeg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nclmsvzr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hchhlmkq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2svefjzpb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uklrjfgu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2enyfhaod.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2htdxobjo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hmejotzp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cwjfqrqh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hkalkqpd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wagcikim.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yjqdmdpo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qbdathuu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zljnidjc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2flnzksgw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2slzasyrf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fijbnffc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hztuchzo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wixvqknn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wlafgoyp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2woszizku.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yhvakglg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2aawgmfuf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnwgaiu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2orgvccxv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fyanrivg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztkyxema.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rkqqfyom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwakyynx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fdeokate.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2evknjyep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rwocuvbk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wbfwjnqv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cpabquou.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kwhnwzer.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2avbpomwh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fqeypecd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pkyolwni.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nipkzkbx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnsdzws.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vzhunjqv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxjtmbre.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2grhvxjvm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xllmqcpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pjlnnaaa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jirpnkvc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ijssiswq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vrwpozip.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wsqjneag.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qhjotqgm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kqhuihjz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2neirvkal.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kimlskvd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2stiuntez.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwppunal.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ncfgkrta.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pfyyzwev.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tsjkgoid.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gihodmov.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbkixbav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gjxaqtjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ehorqgea.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2oaaediof.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zvwmubme.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfltahjh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ktbxkkvx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzmwcyf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cjazvwzm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgqvnhy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2soxeuodi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jiuvysqn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jyeecuto.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ymvkfpsn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hhnlhvoa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kezloqxe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ghkdzgjf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ppnjucyf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2slevpqdi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hjxncrsy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2snvojnqf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eayusziw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lnrzogab.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bhlmoahj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysmpobie.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkqqgyxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovwysitc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ycbmcpyv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qechkqgp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qcpctyut.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yscmhuys.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sqrnlcim.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sxcirubm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hsmevvzi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bsfdoxcf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2afzdmnde.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2evxssquk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dnjtomsx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2csdxkaua.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ktilzwyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tweheohj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ocfsrxcf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2fdmwiyyf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2owsrwiuf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dfinuupi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qzgivzac.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tbbkutmh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dsgvoepf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrqpkam.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2braltqvj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zuncpbzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2fwkwmdrv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcbsumk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2crcxqgzw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2cfcflpfh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2olgyzqkv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ihoayqkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2omqjoggm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dqogfuij.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jdfcnveg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqvcgwg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2grgbippm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qfwofivv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gnhpgymv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bayrawwi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2aiseygsh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2umtlzotx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxljawek.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jhnjensn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2htstrbyd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zbbmqvny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wyrsuodw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvotij.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zlxtebmi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntlowssm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ugakfice.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcpeundy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hmddzigr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdbgkqcc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lkbonfkk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwlxcvuk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qfhqfywk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2idxvscqs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2zmkvdsao.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2syoiwics.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nmpclert.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oyfbuwlp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2otiuusin.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2sensjgfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fvveeacr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ndeilppb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ogzejyba.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrpjjblo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nyekjozh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jyfdxpdf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lxckmgas.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2siljakzz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nvkyyyer.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2aratezpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irlyqcgs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ucxqjbvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzreiwot.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sjbzylbz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2roctlcnh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qpzflkqy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2larlwsgd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ydocfygz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uhgfulta.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwwkyry.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2gdacmpmw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tijehogk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ooyvmnfb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vmtdjoal.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jgrycukc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlxwgub.html

);
来源：http://www.52xcode.cn/Article/details/gt2vzecwwhv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2oibbmzyd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2loonfsoh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2aevtlnwd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ezecpjzb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hhruoijb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ibzhmoct.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2oushfxom.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2vehwrbzv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2glxiucfw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qdcvfqmq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yttlzmbm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2amztpzek.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qrxdidno.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mwyttjpf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2cxzbiokj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tcrvsbam.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ahujvbta.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gyapswnm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jnlvlrtd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xrjsuwwy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aqpkmhix.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2rstlbvqc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kwcgqbla.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2miunyjcx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dodtalvh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rxpkdalz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jemrtuti.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hawmljgj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xjwdwzov.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjqvexmh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qthgmxey.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2guwbbtlo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bqnkiiqp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2njkbqxoz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2muuwuvqw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sxaabpss.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ndhaomxr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gtedfeyc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2urgrmgez.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xzmpsgdi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hgpkfhny.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nikjeiyx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zybxtbso.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hlkxgfic.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gwknrzos.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbokhgku.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ligwnlsq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vizokwqx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lymceurn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kotsuppu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2jbjukjfo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmcvduac.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rrpvlzka.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lgxikaci.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2onrtenia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpnqgpiw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2znrdcjub.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oegzspuh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2thwhsdfv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vvzngrvd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ozorovkb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qyfpgwpt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tdwppiod.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nvipcsjx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uyloxccq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uszvxuja.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yjchdbrm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qszfpbgv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zwqpdctg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vbloislt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2onndmuvw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xzwndzxs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvipxotm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2eiglqmmc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fwvotzvg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jxqlcxyn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pccpivph.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2rptzyefb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ldujqzns.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2weqlkiqp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xynzxgsr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bsphfwqd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvmiuxzs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2byqcnpmh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fjerzlab.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yzoffjvm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nqussryp.html


<!-- 参考信息 -->