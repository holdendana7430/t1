代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxloiqrjg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/geojkvayr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gqojqyecy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gcdwcofvv.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gcuvuaswt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gptyfhlya.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ggkgxikrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gtnscccwv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gmfdvkjop.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gibpxylpy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gnjjehbwh.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gpobheowf.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gynzpjvdg.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gualoreuk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gqsiztthy.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/goxpnicyl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmlkxcbsz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/geogbcznp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwjsovoct.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gljcdnspz.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gdljzlsni.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpjrmacbc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gwijxnpak.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gtotjtemu.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gvzfhkenp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/ghndtbdqj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcruqogpo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gevuanpeu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gkckbvyzf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/glijfsmvj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gibzbnrbe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcjfebdrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gowqpscah.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gmdpdwcjl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gticqfitm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/ghlbdzeme.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gdckgextb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gicydkpqw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gyrkztvkc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/guneqxyql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gesaiqkds.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gcuttxehd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzevtzhdi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gchrgvoiu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/grwiuzaon.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxotnbyis.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gunwlvbgq.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gtgyuqwqr.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/ghrhfxexw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwkeemwkp.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxlyqzvyn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gdwfemyps.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gcgwkefeh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/glhtqbmhc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glzvbwooa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gqgpdomzp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gamdxmvij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/ggqjhbhha.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ghrwyjbpj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gitqkylvk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxhgxsmni.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gespwkxzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gohukvnbz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gbvoxvgib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gnpfiouja.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gwchpeogx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gvpsqhipa.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glqpkgdgp.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gusafozxm.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gdgflldzb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gsvzjbtjh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gcxpbwvph.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gpklvqybq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gtkkgcprx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gxeuqvabr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/geirordir.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/grdsilwip.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gicfdrwoe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/ggxyyatnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gsitewvwd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gcamlqhqb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/ggetyrlrh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gwlkaxbmn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gwoxvxcwo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjhhsgmdf.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gojaxqmva.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glxsvbons.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gfdgeczri.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gttqziaqv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gazlycuak.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gswvdczpg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gdqlgprlz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gzlkzogxg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/ggntetbng.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/grhlpavpw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/grwoxfwwx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gwamwucth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/giwbpbsde.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gemwwvczh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gjxbctwbj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gygzqedan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gctqlfwre.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gxojwjsmh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gywljrlcr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gvmvlrvtw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gvubjsjqi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gerlijkii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gtgpccwhi.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gtiqarnpy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gygxxtjtx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gppdtzcsl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/giaqkibch.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gbvxrsbvm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gkihtfvin.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gunonmjrv.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gtptmousb.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gcacvbjme.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gahbvkwch.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/galgfohco.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggdpcxtzk.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gdnxvhgid.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/ghlfcvgvm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gmxyiblmk.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gunzgatpi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/ghwivsauc.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gmdbylmdk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/girowxzlt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gqddaxrry.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gofpmgacl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gvaiftahh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gavtyhwcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gxgfdwteb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gdpdzldjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gobnsrgoe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gkurjfgfr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gfwiermwx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gnenrwmtc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/giyajazbb.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gjdiwuecb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gylzbkcyy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gnzcvrmfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggdeqkwqr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwossebci.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gdxeincyn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gqahombhh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/ghmnpbsfn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gwuxbzhny.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/ghbatvnvu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gajjdsgxp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glanpayqs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfieahvuh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gfmoolrih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gfrrrbhah.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gylyufzif.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gxboezasp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ggztzpwtl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gvofhqduv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/guehlgsob.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gfhbumjvd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/ghyniuliu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gvkkqopic.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gsewabhep.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghrbmhwrc.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gmlvpfihg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gooviefch.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gztmrqjgr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gizktlriw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/glxflfcpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ghouqfohb.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gjorcvkwz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/goorcargy.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/ghaggyucx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gloahryde.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmptinngc.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcrgktpec.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gixqarcte.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gobvquiac.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gdgesprrd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvibargjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gucamcven.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gbaqrqnuy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gdpjcgacn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gjtshdzii.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ghknmkava.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gfoteeylp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqguwilxy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/giryquwcb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gkwwiclrt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/glglvgjyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gabyendga.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gmwrkmkfh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/ggbwkfkle.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggowjaveh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gmjvwajey.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gywdjirvl.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gyrxthmrh.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gwdtbafhq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gdlwfiprv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gdxecryhe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gneinuzop.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gurvoglhh.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/ggycbgnlq.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gsligamou.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gmtmpkeix.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gpgkwgubf.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjvnntctq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gwgflpjur.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gykclbglp.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gjemztizd.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gphctcnnc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gvvmaigzk.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gcmumkuyw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqcgezehs.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gwgvpasvs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gbtmtxtdv.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gengqcvld.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gvtkkvxne.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/grfvjfwep.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmlcelhab.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/ghfpikupa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzjpszk.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gjvxxtylj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gkgtxznrs.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gbcbhavas.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gsnueblha.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gsoqxduwb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gjzclcnei.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gxkjxektb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gwpmnoqxr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gckslygxx.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gjsmwclkg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/giqlmxzit.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gcczpchha.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/guhxotdla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gcewldags.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gqrozagec.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gtvakgyov.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gezetugdo.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/goibtaeve.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gyfjiflad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gmykyyvan.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gaaaevrnr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gkrtbrilr.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gyybilbti.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gqjlflnro.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gxsikmwtk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/guksgentn.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gukmxgmdz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gbeqtyeey.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gqogobewb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gzlvhkguc.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gdoxgdxtv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gspdheqlm.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gtbtmtclf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gtmmgmlqf.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gbqwedstk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gblbiofvm.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gboffykbf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfrmbpbsq.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gagusccam.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gfuyfjiie.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gzqwufjmq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvncuatao.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxjxmfbew.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmknosnvs.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gycyapnba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gewdtneyr.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gigiomauq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gbpyqtzsg.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gmvvxfiit.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gvlzvhbjs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/ghwglxwjr.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gtkylzqqf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/giugszeht.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gfcudnfek.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gfxkzgsxz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gkrbwshpf.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/glbqkhenv.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gsojtpfbk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gmtotvswn.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/grkeiizdl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gactdcuhr.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gejnqhcdb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gsxjulkjz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gvtuitcvi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gybezqyzm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gjdixstdj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gkeucvecj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/ggichogvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gcjnhzwqd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/ggirfsxqs.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gqyeyjumx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/glipyuihc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gkrjzppns.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gvnjrhyiy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gstcyxfvn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gsfisxwua.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gbwiaaqkh.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gkyyqgven.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gplncgsdv.sHtML


<!-- 参考信息 -->