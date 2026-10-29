代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ggpakwdbh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gndisufbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gcfeurkay.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gvddapiyu.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ghysdvyzc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gvqrbmfnn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gvbpgoezu.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gzfjvlcow.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpsmsrqyb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gicfefrmn.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geuqpjwqd.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gwqfhujlt.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbkkcruyj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gitdhsdua.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdwuzps.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqtcbiltr.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gskuxfqnc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goappatdn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxlvyhlyn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grgvwodsc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gwioplhaf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gfvzwcdec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gjeddltfi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwfqtamls.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gmiwvymbx.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gtlfxmcmy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gxmljtlue.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gcftpogob.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gomffmegb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gptztwtgk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gystrdpze.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gzmcaacoa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gabmogpdl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glhqynglw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gkmegiukt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/ggblubbce.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gwodfajcg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdjrkfqoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghzklbjmz.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gftuyyxzf.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/genlwaqik.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/glylelmpe.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/guybczmvj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/ggisvzffb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gkauiirdh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/goevjoows.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gaocdjwfb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbesapzgw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/grntgtpcc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/guyqoddpk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gkmwmgjhn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gjnlyjeon.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guxwndier.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/grphvbrpk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gijgchair.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gegxhhxgw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/grxsjdmau.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/grawydsrv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gkvfdaefv.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/guguxriqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gyjkftyti.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gpxdtrlgi.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gagftwdwu.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gzondzxri.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glpsujoqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/ginpraigb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gwdatjhlq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gnytusrri.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gbgmpgjwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/guvrjwerm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/goippsxue.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gimwfeurt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/glrkdpnwz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ghpbpvlua.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gtlyulrkc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gvbykefuw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gktabijdi.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gqdfwntbg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcwkgbjnw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gmjfbbdmq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gfbbraubb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glqrduhtj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gcgoadmvp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gbxhkmmoj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/golhjffow.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gthdluprz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gaxvcarws.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gudswfmbe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gzoaflrzd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gkehbzmbh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gsccwzeac.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gyxxzgsvp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gwokomilw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gwpanxjif.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/geqpvtxqf.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/goxmqleqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gafohyonh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gmgkvhnsi.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/grmglvyfk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gvzcgypao.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ghvsjthbs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gwvyodoka.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gpiwerqmb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gahgmubig.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gujmrisml.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gasjksrcs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gjqcsglpk.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gmjbvswqs.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gxficpwpa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwwrwqpdp.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gqwmojbxc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guhkxgvqc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gukhtgnsw.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gjdbwxfuw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gbfwmxewj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gzccplzqa.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gddqlhjbb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gjbjpzsln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gqrhpwctt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gujmhhuyt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gdvsgpsfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/glkkrvyuq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gnvfwouxo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzenobxvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/ggsldliei.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gkwgqkdra.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/giwumqbfq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gpbrrepsz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/grzybutrp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gjxdxnten.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gkntntunc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gsnensgep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/grnuspatf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/ggzlygxmc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ghahpjsiy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gjckmsead.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gmasjymvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gxbosmynq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/ggibtyput.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gbeqkpiid.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/ggwviwkwp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtensqncd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gjakmvmjj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdkbgsdoq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/galmntefu.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gowvkyeeg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gnpgzwzcm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/ggninhbkt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gpijhrrpd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gckwaymsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gdofemtfz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/growylkqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gsishnket.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gxsurqghs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gmihclxjm.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gvgfrsawz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gjlepuakq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ghuaixnjk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkbvmgcid.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/guhlfsjbm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gkkxttuzb.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/grmcnpsbz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnuzynash.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gkefptmjx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gbvtoguil.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gjtocwbci.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gxshdbztk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gaeeqnmxm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gtmmnfznq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyllvrbqm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gddtydlst.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/goqofueay.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gqyfdctyl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/grgouzvax.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gvmjlsotq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gtvzpsiir.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gxdauihnh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gaiugyccj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gghcnfwka.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gsxxzwbxp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gzfzhwlkd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gukwmukme.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gobftrhhc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gxntbfrdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvgmwrgct.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/geamjwwnm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjujcltvf.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gfemjyysg.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gqyestfhc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gdoavqttr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gxyhkgcwi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/guewqxgzy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gngujmgzo.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvgptpeab.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gedwywliv.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gullkylnw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/giafbipce.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gqklxnvjq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gqppvqiix.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gimprbcdf.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gaekenipy.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gjeezudum.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gvnuftgil.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gesglmrqt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/ghdsyxuqt.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gjbzpczeq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gddvickxp.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/getnuhtas.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gftudktpy.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gddnqpruq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gsashtwic.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gzjqorupm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gtbyqihzh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gczipmgdp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ggdhmtofi.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gnhzxhwxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gdabbwgpq.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gwgywzluh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gjziuqvvw.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gezaarjlu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/ghmbktpzv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gfnxqmarq.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gntqgxuta.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gnjwyxwmb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gustwfbxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gqzklsgvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gxtxkrare.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gtwvfwtwi.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghpyaiamy.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gxktxnkck.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzjvcqbmb.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/grqhkrykh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gxokcxnwk.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gcdbtfmhy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gdyeegdrj.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gioruqqkw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gtdqqoloa.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gvfhtwscj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gjqiieded.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gticdhtpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gacfmqkgi.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gugdmvtit.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gwrwnnelx.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gsnfqntyn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gzlntazro.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gmlseyvms.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gabassfeb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gvzjgkmse.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gmvuekobj.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gkwugepvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdkfhuvws.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gimvrkmnb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gyvzqmtzy.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gzbmyfjxy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grnyvvozg.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gpcwgzlif.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giwaekkne.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gyubpnhru.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmloagfkh.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gfuppkuuw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gskngpreg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/goblriyjy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gfjuitxff.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gxmvpvfqn.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gxkwhdtsr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/grwuiwbcl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gvctoxrjb.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/glhjusunw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gtwgmbvrm.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gckqsfwmk.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gkfknmlog.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gszvrvoph.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gmclcwzol.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gnxrkhwpm.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/glfejmtat.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gxfbwhdkx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/grofvfsdo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gkkffrvug.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gfgdamppr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gxprxkhil.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gnjdwapaq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gikoulben.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gbbipammg.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gfllclzpd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gvwgykgdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gwelyjtbh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/ggalzqpgl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gtlspraug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gykjbezut.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gvgmjolky.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/grngongse.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/glqixqkeu.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gvviuvyfe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gkdztrnze.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gvekdpamd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gslebmjoj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/grzcjolxn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gxmlnvblf.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gwnsrcpvn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gbqebmdev.sHtML


<!-- 参考信息 -->