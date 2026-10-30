代发 wailian999

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gkufxorbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gdxhqrlwp.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gxbrclycq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gcslostdn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gaswdrouz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gvkpddxmz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gqdcxtyaf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gpetbmqcc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gaajxmjhb.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gkspwdvhn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gmjffpcnz.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gmzisbwbn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gogmaeymp.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gvtnwewez.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gyqznrsjd.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/guksiilzz.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnekmzhsf.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gybgrysuj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gycpplhxf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/givxckutb.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gazxlfufi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbjhkmqri.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gpjhctsfw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzmvpax.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gvhhjkand.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gtxfefqws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gckdkzvnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/glejezbyd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/grfmzygvx.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gnzioiazv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gvvpabool.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gotlvpgrv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gzqvbfgxu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/geasgsuxy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gspbtoljg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gmwzeiswl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gpzoawxef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/giyermubq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gkljrzqje.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gkoehxwcl.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gvpbuvhdh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gfsltlwqg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gjcgwdaoo.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gzfslukqc.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmjnirtah.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gubcjjudn.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/goladbmpb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gucytmikl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/ghorfhuny.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gfdbpnbrf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gqlqhaumz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gzrhtkuwj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gnoktkyjq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/grdoyhqht.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdihskbyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gixporxcn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gshpgwkhg.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/guuzsoqfq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gewwiklvd.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gkkrurwcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/ggavgrouo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gzcpvjmim.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gqsmhblim.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ggbuavduy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gtrjpaxen.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gjhftgjie.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gtyeogxhu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/geadooepe.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gcipozlls.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gajlialld.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gchfiwfxu.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gtgibdifs.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghizhykaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gexucjjkn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gnmyowftk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gppemcqrj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gkpqaudxq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ghkvipyuy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gaqazdmqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gtlrbixig.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gphpqktqc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzhmcegrv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gtxalvsks.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gwyiicquz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gozgjsftj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gwaqzjrah.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gluivjrfp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gevaerqzq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/glesmrokt.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggbfdqkcj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ggfmhqnqc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gjotzgmkm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/ghiooetjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gbqjuhncf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gotkbzekt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gnaxixnak.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gfxwskvux.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gpwmfoitl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gbxlrscwj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gucxpohrd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/giqbrpxkk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gwglrkidk.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjdyntovr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/grmcgipsc.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/guiiyditp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gyewqgfei.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/ghokvlenp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gndprrfwj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gbwxbmwiz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/ggpwrcyrr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gevngxmbx.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gqamnnqmh.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/ghvvwylol.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gufqbkccl.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gyaqnwtgf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giqjtmica.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gwgqtdkgk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gwxbqbiws.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gmgeqtrpb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gzjnzqogi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gwxixjrkd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/glqnofeiw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gxsbunluz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghbxfmfhq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gkbncngvm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gckaqdohy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gucchfowz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gqgrdoluo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gwuzwvmxc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/grpszagxc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gkpcggrdl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gzmqgtabr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/grjneaujw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gvamqjcks.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gumypkvnq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gjindmgdo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gomyxeaef.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gpyjcpphl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/geqfuxrex.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gpiimwrun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/glwccndqp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gnqveejgq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gzcjtfoad.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/giqhgmpiv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gvswakeup.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnojmzxsq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gtfexfgnu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/guaeicbyd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gjjgugtsr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gomripoho.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gllgokrqu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gmwihloen.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/grayvqivy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gayvghcpi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/giebiyzdf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gytftucaf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gureasenp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gaxusxzes.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gdycxaxlp.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gzzoriysw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gsooxmylm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/geeagvloy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gbbmrjpsj.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gpyepvaef.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gtendktxr.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gzjrbxqmb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqutnhjbm.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gooselrec.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/glnvvcdsh.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gfoinrofo.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/grxfmecdq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gnjdemqym.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gcssjzdlb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gonzhblps.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gfdolpeuj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gvvypynqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gefvudcdf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gjnfluing.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gyheuyxtd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gxledhjpc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/glhunvflf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gaqquqiuz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gozfoljqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gpjtxjphd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gtpjulxwm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gqqbxepsc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/govmdiwce.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gcdrduoeb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goylvbedp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gxbyvcvwr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glxajzmil.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxuasnf.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gbmwzjlzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gfrvcxlly.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gmqtytqmr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gwoalxqdl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gevqaeibj.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gaeepqniz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gkmfqiucq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/ghukygxmp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gwtqrbfgf.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gwobjjbdt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gaxtfqort.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/ghhkjvlpv.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvblaqvgr.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gnchnrwot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/giklocpih.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gwtufdbgx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gnaqzypov.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gewpzuhby.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gpkxajpdn.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gtvlouvly.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gtpllxivf.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ggfkrsqef.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gvlzgacto.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gozweiipq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gyqlicczn.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gbepcruae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gklgrdbfp.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ghhubfajl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gziogybun.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gbddkxfim.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gyiiknhzv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/glaulepwe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gkfjufcan.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gyxabrtlp.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gpzxhpday.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gjgvrjrbe.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkvutcbr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gvizvuide.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gflycujch.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/guwtatgmz.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gnoagdwle.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gzwzkxhch.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gymmbskdn.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gzgygbrxi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpnefanbn.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gwmrpnvri.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gkzpyzomz.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gkiobswxl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gzvqibhvl.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/ghtxvuquk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gjkikszns.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/glpmpkhyt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gkdtkefht.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gqxhaatsv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gabbitdeb.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gawryqnvi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gqrthekrc.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkyktolcu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gslxgfsio.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gpxljlbqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/grbxchlqh.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gmytregwd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnvbpsbm.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gbokcnsai.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggilykiny.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/glrhygdmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggqzjutnv.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gwfnbgiik.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaqisopcd.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gpylemmlb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gycclzfar.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/geswlvmig.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gqhsurkkc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gobdxkabh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gtgeucpdk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gdfuhjkjk.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gfmicyseo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gbqnottxy.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gsacutxhp.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ggkfhmcth.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gbjkosbvv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfqshhgkk.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gvuenblrp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gywkcomwy.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gaetgohlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gfbeqjvzl.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gkaiwpyxc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gfpcyqnno.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gnrghblcx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gknlteefe.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gdgwhqkim.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gwicsdleo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gdwwgrgnl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gqdwifipu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gotwnbokq.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/goaetwusm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gotuqdfhy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gbdqoyifn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/ggvmlykzz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/genemsosu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/ghckzkbol.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gdgvaqccx.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gjhdfzhzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gondwlnak.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gwuzkhiwo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gcwaceadn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gmufhqhur.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpldxnlkd.sHtML


<!-- 参考信息 -->