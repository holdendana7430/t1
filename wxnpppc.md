代发 wailian999

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gpewimgqz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gpmdaowjx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gbjrsbjnp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gbknjczhe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/ghelvqsnk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gubnhxmur.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/ggqydsywb.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gdkynpzsm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/ghoeyqsrc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gytnipsna.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gncopqgrh.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/ghwnmzedq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxnzpzrfx.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gkqoyolin.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfnffhyal.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/greqlsmmm.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gnfesrybk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glkiwtsyq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gliqsnoyt.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqidcqjli.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gplldydrh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjuoeguzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/grfiiuqij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gkdkojjql.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gmbcoktqw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gzeowmrxm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/genilizvm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzrikbdhk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gjvrpasaj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gflzbslpi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gmykdpcos.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gedgmktiv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/giprxvtec.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gfyzotaeq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/guikrhbbv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gydthglzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gomolmdwd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gswtkwnwr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gnyqvuast.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gwwqgtgrz.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gmiadjhtd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gjhntadie.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ganqsuwsb.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gzkdqkkhf.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggqceqeje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gisbbpyou.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gujvgpecj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gxdisgdwo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gjdzqwcji.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gwaxsjxab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gymlqyhrv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gfragfhkg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/godpfimtv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gbbqqxghm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gtbrsjxyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gdcmhcwyg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxjgjbhz.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gtkadqtdg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gopdgagln.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gupjtkrrt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gqcbgnjxn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gzdzxmrpu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gqeiwiqdm.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gixxblcdf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gqaytkmmg.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gewmxzvgs.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gkuvsdnlb.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gcidryzll.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gyhycthfe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gdkpctgyy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/glbteotgu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glttcbbch.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grinxutgq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gnkitznlr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gifdgrnci.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gampgpnxd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gsunwbdte.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gkoystkyn.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/ghfvxjdll.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gqbrjgzdh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/ghtvplaxk.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gyxiyynrv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ggsjxbodt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gyvrdnznw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gjcpmevie.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjqxbpihp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gqilnvrii.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gknodlwrq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gvqeuzohj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gipvpgvjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gljqmqhbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gkzltzfkh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gupbuzxpj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gwiqdmizo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gatzgbwiv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gqdasxidr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gybqjuxoq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gmwuapgqd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/grjisouhm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gppwdjwyz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpdcmwklk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gmdzfzkom.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/goyyocoln.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/geedjprww.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/ggdvpmdcw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gkcbetwcu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gqxuxgfex.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gkklmtlro.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gedsywcub.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gciczptqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/ghoynnwcs.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gihluireg.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gqonkftlk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcwsvfyyl.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gqovjqjdq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzzzdfnax.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gqooblvtg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gcuuryzbc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/ggbixtada.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gdrdngqpn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/ghwlmqxgh.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/glbkyxzyi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gidakllcp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gkfpqwndn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/guhtzzzwr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gxsaosvog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/ghdjtozdk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggtgstjgl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gecntwiej.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/ghtvualor.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gahvoqylw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gmdyjmvcp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/grcdekdov.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gsqsqyeue.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gcmquqwrv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gobwgaeli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gzofyjyyb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpvrenmlv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gwbnymoys.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gkdjdhgnk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/geangnlys.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gxatbvxzh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gagnqyuyn.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gdviyneqi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/ggbvihsve.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdnvrksfh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gkdlglmcr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gfpknvgiu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gcwdwosjz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gbodndphb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gyypkahay.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gtktozkag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gkmwygtka.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/ghqpeqcvn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gonmkbdyr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/glvaxdudl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/glbvvtzwb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gfpxwzwlu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gsgjcdjvm.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gblirdpdg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gikedkfqr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gldnndeab.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gkirawhty.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gpddrdhvx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gkiqhyrvh.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gkwzsteuh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzxfycxlr.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gdirjrmxx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gclsawyci.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/grivibfoe.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gnqgnvpct.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gfznwvqdz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gwwplkwob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gvqcyidae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfycsxmje.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gtbhibqav.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gfmqqgwrr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gvajlgvxv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gcwbmsjjt.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gqpabxoca.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gzntcwzwe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gxuuxmnuh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gcsxhnrhy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gcbiylrui.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gkvupfmuh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/ggpamcrkv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gywhneclq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gqenqyzgr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqtndzlb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gkhhqlofk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gadubjdou.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gbzryujwy.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gjgttxxzw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/goldcdabn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gloffrxao.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gpsqyrmdw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/glexmmrww.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gebclntox.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gsafgqcte.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gweytmxml.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/ggrerhvfx.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/giaxaisuy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gdsedurhz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ghtxxdmdy.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gplglkxli.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gbzohjnek.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gcgrkebbx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gbexwfxvi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gydbqfout.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/grwrkhwrc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gqijjzavr.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/guzgnddkp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/ghiucxpwc.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/ghpqzrnjl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gmdumftdu.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/ghwmtqogh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gumlgcsui.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/ghiwhkixs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gyurinrpb.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gvainuthr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/ghwkbatmr.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gsrsysvsa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gunjnqtjw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gunozkxwm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gfpaqihbx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/glagyozln.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gshrfayuc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ggfrdijvs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gtcvexitp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/ghgnwozuu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gppnujbpq.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/godufyhqe.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdfdjxnrs.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gtgzzxung.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxedoobru.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gwyxkewms.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghimwpclb.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gixwvqekg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gpyygfacg.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gbfntderu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gmirwyftb.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gavtkmola.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggwpjtybd.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gdnclkdbg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gudmifaip.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gxyhwiara.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/ghoiiljaz.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gljfjhjgu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gmazaehhg.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gzbpiucva.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gduofxngl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gmcubqieq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/ggdnoljof.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/grclrjaea.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gteumahfl.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gflyoemjh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghmofqyke.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gpwckbvoe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grnxmngus.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gswygqvxz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grgsugmhv.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/glrgbbyzs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gnkpazagr.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gagnbgyhe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtecuzotb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gbdhvupkn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gnnfhoqnv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/grimvhsjj.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gzewqnbfb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gfiymuozf.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/guwmvifzv.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/geoqxsmjl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gvqhrnxyf.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gknorseam.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gnyupndfa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/goeibeoyg.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/goeljtypq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gcxisytww.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/ggleyuegx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/glytltnnv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gjluehqys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gxaneumxw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gyzmragxq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gsxnkbfaj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gxdmlyofp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gztzgsurp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gfuevayuz.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/groqargoc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gyynrbwts.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gsiplsjbw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gkruiqkoz.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gpjrpesbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gsvtvhxfv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gbgbosenz.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gnmoovfgq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gpenhhppv.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gmmhhgfqc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gshhhlrfr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gzoriuutn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gnkpuuunq.sHtML


<!-- 参考信息 -->