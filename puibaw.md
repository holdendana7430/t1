代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pszmrqqz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpdezreq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mdqeyhrw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ocimnhle.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pfcliafe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wxpmlnbq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vcdplzor.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eyixzawb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wxgtftcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2meqfxzhh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hjiqeqvq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yythbmnv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2skzoanij.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2oodoethk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aucniypv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ljioumvq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayygstce.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xuzyhmap.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bmvqgrhf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymdizrud.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xvsugaho.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzvzjpqv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rtnidawu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlcenmem.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vsmuayzf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2munjozhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtcglrbm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rgfadsxd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2lgoissji.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xzxuadqh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wtvuddno.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cgsmwefb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uetruqst.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wufdkfra.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2acjdqocm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fbkoqiuj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdmelsa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kqhnrtsu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbjrczrb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdqeblh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vftggiul.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvvlmem.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2voxrtjtf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2whawtiqa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kfuxosru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yoshsplw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mohmvvld.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nizbdfxr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mrxuaasv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gxxcmvgo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jppzkycb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2kegfvbvt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2buwazwky.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2msgqpyyb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vrefwpcx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2phfxivyx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ajgdpvmd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xfllxeex.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bwcuchtc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qenilbaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aifuxysr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tvjpxrbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvbeuann.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hbhbmius.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nwfqoxku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wotsxkph.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2iuydofeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hfznxhon.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2asmdlwki.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nrtqidgd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yorfnajo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2goppodxz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dmqckabu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2twqipxqn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2shugeocd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2owyalfrv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2afpmxhbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rzumtxor.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xuzprjlm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qkufmvyj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cjxrlltv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ryxudgjw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zfuqyomm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vkaerois.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fhemnyca.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jpxznzhh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pkwwumuq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rkwutdhn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zlflogzy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dtngpmjb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pssurxsk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qhflwfps.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lwkktgoo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ewbeusls.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgljpuf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xgmytbqy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fgtmtpzd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vcmfxbuq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hvuickri.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zvwtdwui.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gcolgqjm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rbusjmdq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ypjyqpaj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tkzdrwyo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fkbickhb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tdgpwufe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pihuwaxi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2adwuglta.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugxbzjfn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wwokaogm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2igcpkymf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ucayyjfa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fsqekxkk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jcaoywwm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sutnfuyx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2efozmsvt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hmyuejdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpulndlh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xoldlfvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owavejvs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cuokzubv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2buktjtal.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mogsxksj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sewhpfsg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xqiidhuy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jvzxvjtt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kphsjbhj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zxbengdm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2srnpvfvr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kfjbpevh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2nmvexfkg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2eshxxxaf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2dxsflaha.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hkogwtpp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fqnpvmcy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hwjkcyor.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2imywkumd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2hwiwmmyx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mkkzuome.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2sqdfxmhp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gokrjpqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ciimfkas.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjuesqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kgvvpslt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2afchjtcz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ofocujbq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qulvfkfw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzdjyayr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wuzlldts.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cragmdso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mtjbprgj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tueekhnl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yxwzppng.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpmvccs.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2yxawdbcf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ljomwkip.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ttolknze.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ykbtrhzs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jqcnwqjs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qdjyqecy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvjapqh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ahhxwyhs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rveiwoeh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zaqtsyus.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dvkvkapc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jdqnthgx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ahmhbber.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqznmzfx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2njrgfhkd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fvcbviue.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gkaavpnr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2prvajkvh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgguueo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyllkmse.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2liiqgldm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2prkqqgfr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fuayarqp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ebdgrrrl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hptynrcb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jarooqel.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wcdhswhn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wuuldbno.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bwgmpfko.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2epucudkp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xmgxaybh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gjzzfnmw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mzrzyodg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gifveucd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xxttugwg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mbrzkxme.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nmglwweu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nrbwsmhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2essjokrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mxbsznhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmqlqkre.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ckkcwezj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kgwqwawb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mkopnqtc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jisshptt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2txbktsbb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ivapplcx.html

);
来源：http://www.52xcode.cn/Article/details/gt2lrdslfbb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2rnsrkkvu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fhtzcluf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lyzsrrmh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hxuukxhy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hrymuayn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmyynaz.html

);
来源：http://www.52xcode.cn/Article/details/gt2dpnonlot.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vuupbftw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tdqbocop.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cuetojad.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vvztcyba.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2npbbnanr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2oaxmnwjc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pcpiegmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ksgjorqa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lfbnzirw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xyginpvx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijzuabtf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ihqbzjdg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rgnybptm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2augclyzy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2btflkeyu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wjcysevh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lxsrrhma.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jxcqhozz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gcoxuyld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2jpazslfh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ifdrprmq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ejvkktur.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kamiycnx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wswljssx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ndafmfkj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2oshmynqf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2apdjwwne.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eptopuwl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gttgmewm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuspreiu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ymhcgzaa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cncofugp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vixydsxs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hevakgqr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fbolynzo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ygjxrygh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nybtczbo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2arwksfhl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sbfxsmhk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2fjtlgyct.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nmtrxfzi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hoguikiq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2oidactzt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rhubvdrw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ngddrzii.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnxktbyi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cxqulwuj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2soyfcmdu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqqdlv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvzbpbjd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xzkpllgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixkwysmj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ankcwbtt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hmdfpoxv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gxtzkhmr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvrgxkbh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tdtfvnlv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qviiwuwa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zwsuwcht.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kfnyxvzm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zrbzvqqe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ujwouqlm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2esenhomc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kscjmxfm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rqrsqigh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2tzugudlq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cjogqijv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cuhomita.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xsciirgn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zweopvoy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2chvivfnr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2twgxsaqr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2niofazzj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jobzgaxx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhdkiste.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xjiwgsii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vzioslkb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nyxlvwsm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dfvxbcmc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jxpthybt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rodciqzh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ytgwqils.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2llzqbkob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hmansvbt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ldpqqaih.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wzcfbemf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uihqkwma.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2tcuawuzw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rskjuusu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2orrbvbgb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nwneapuq.html


<!-- 参考信息 -->