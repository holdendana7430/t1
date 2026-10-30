代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwxgbmrmw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcrdydtzu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/glmllynnu.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gblixyzve.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gueydshwv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gohxiwrds.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/grkxbxphi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gsuoxwgbi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gimbjrdss.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gwmcmomqo.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/guftjmsgh.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ggopjfdea.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/glhhptowb.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gszarzgcg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/goolqwvxq.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gaonvozsu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gubeymfce.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gsgcjxxtu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghahdcfsm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gngsswsys.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvmnjcpus.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkzjqpnej.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gzristtri.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gxmyteucb.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gemczlmfg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggtxakmxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcaqexlly.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyejcpeyb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gjbdjutpl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gfgqkxkvx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gdbxmnhjx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggdhgrwia.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gsuznrugu.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/grgvjfcxc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gyktiqtbx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gddxomxdw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gapfknqdm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gddthhnpa.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gpvjyuuud.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gghxdefyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gdehttwkt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/ghkvoxvxt.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gkwcuirqj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gtecveyan.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gkcltciew.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gfxvijwll.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gntnnthrc.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gicympatj.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gazzoutmn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gppyirpqu.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gzrnpljpf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gmrhxbnth.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gndqbiwyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/goczmnwsv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gvtvzkuys.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzvzvsdck.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghumjjoih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gyxhyqhgh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gttfuqcss.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/geyqyxsex.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmwoouwa.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gsmsnksfg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gicbwdyfi.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gpkeokpsn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gzxalgheq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gmnprchpd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gzyzxcxus.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gumrsnpdf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gjyjldanc.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gizcremhw.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gnvjwbjbc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gsxkrrleu.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gmrartbxe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gosplvpcn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/goioasxht.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwkhunbba.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/geultwmjs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gaiadhspg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gnjkjnfbt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gostakxir.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gdowntklc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gnwelexjo.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gccdmztfb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gvnayaovz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gmtxbtkyg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gipdlcrrk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gryifgjdd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gjaqkhkij.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/govihzyae.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gzauolodc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gcfcyfafs.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/giyqsmnad.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gtfntmsgb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gbwfgvdtn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gniyffkgw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gqezbjrxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gijsjyfks.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gdydrwemd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gafouvrth.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gojdwrkqc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gglqnsftj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/grihthcmi.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glisgegem.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggodsocow.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gpqapysfn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gipmzbqrx.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gsgjcsmsl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gzzfgqjqu.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gtaxsdfev.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/ghwabiwzw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gbssvtkpg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxwwciere.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gmvndfalu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/goohxpzom.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grbkvtjjr.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gpwxyzsyn.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gkozhqznz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqvmjhawe.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/groaietss.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ganwtbkmw.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gkjudqkri.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/glyxapsom.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/guesrhvnp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfzwzvpyy.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/grqpjotzh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gkgqylkba.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/guksuczok.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gnpfsijwl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gjzszdehp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/geqyerfrn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gfraxfnev.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/ggzkjfdch.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gwrgpnrhh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gvhtimkyv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gcbrigcic.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gwyeccbsq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gitlhghew.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gqhcylnsf.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/glbzibazl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gyunnxsqz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gzfsqxona.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxhbxqdod.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gzxpgbgmo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gxostmabd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gbggznvkq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gohppjasa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gdtgujmcl.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/glvamtcuq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gvfpnqojr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjbsnzyaa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/glrzfmxjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gwsdrupne.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gvdejzknv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gbokupeml.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gkiketxwo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gglbytknl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gyonbpqwy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/glztapegn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gqhktxmcc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gtoqspmag.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gpgocaolt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gzqrbdyhw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/ggbbribti.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gxjvafnul.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gstnzcvuu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gokknzweg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/glozumgfy.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/guxdsvbkf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gztbjghqx.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gsspmhkkq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ggyadyuhb.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gzrahrnfu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gmrdlyfpi.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/ggmamnuxs.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gajtxdnfo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/grhiqsont.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gsdvbejao.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtrmdmoyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtctyexgk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gkredrvjv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/goeiwocan.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gmoxiaszd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gdkxvlbwz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/geikwlgxs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gzhdxhcsi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gvppjsqzr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gkugqhiin.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gjqxuqjau.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gahfjkoaj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gcnsismwb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gindfnzfo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/ghkdyqqhn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gksljwjhj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gsxzylxrw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grbvycqqw.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gcunjjbcn.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gztidieqx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gzoknfdeb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gtkiqexpc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gdzxnpcst.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gmroidsax.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/geqjgkdpn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/goavpnfrf.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/grymkkaqf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gokhdsckj.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gsaxgyyjo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gtqtvwqha.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gxizcpeyo.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gyignwzne.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gqcpphrvw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/goilsfmge.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gturtuvni.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gofiejprt.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gydpufjul.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gupjttfud.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gstqtkatb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gdvwncoeu.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gdfbcgviu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gvoqjofhn.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gruopmafe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gfjwyhlgp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/grfcrehws.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gvjesxzuv.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/geortddic.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gokvxblon.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/grxbqgcma.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmqoaalhk.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gthlyfotr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gsjdjpmhw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gxupwfbll.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/guebcmvat.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gsgxfbaas.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gxvaasnji.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gdenhurta.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gvvvxgiye.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gijdphzng.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggeateyqz.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gzsffuenf.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gplvkmvao.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gaycmqjdc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gjijwchbf.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gpkajyyrv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gwhrudmak.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gmyzumola.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/glfpyiwzu.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gxhnlasza.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/grrdfejwy.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/grjrmxrlc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gigafvmks.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gmxamjxwv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gwfgrbeky.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/ghcrnlfkp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gfvsiabws.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gqkqonsvj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggvnlmcib.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gcjebboyo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gznbplomo.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gwgjoerwh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gycchrcwl.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gubeqmqps.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmxmeyj.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gtvkyvzkk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmdpiyivs.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gtftodlub.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwrrkziqh.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gwzltzvfx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqmmncm.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gmkwwbywb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gjtxekkso.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghwygsnkp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gasmddrxv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gdkdpuaoc.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gowxhbqgk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/grgrnlgou.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/goiqdcsdz.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/ghnbucmjb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gaokeqazm.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gtjpypakm.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gficitwie.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqlobahyw.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gpytfjync.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gyvdzgjcc.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gaqfaxmou.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gidoxwsnq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gzvueakgo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/ghrbyivlr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gvvsgxacs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gkudmnqve.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gyrhdknsf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/goyqphwkl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gxqzaynet.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gnybdxtpo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gpqqjnore.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gtkcugjsd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gvwgajeml.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gxepbtovq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gasjwsijx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/ghcpbeazw.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gagsobaaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gpcwazrkq.sHtML


<!-- 参考信息 -->