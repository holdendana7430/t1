代发 wailian999

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxomtwjhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gisgnneky.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gxcpqodds.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gpcovrgsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gqkunfsvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gojubjvul.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gybowgmdl.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gqvnvoshu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gpttsabmk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gjbbcgurd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/godfupefd.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gjovdrrzd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gspxifobz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gguowqdqs.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gguvnodjr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gezghoird.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyfvwtrkc.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwwxoklkd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gzksqvfrz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghdogeiyu.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmfmuzvbu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gasczmbjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grblkjgdw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glpnitnuy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gzmzvdygs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/glusvygpe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/ggowjctnj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gmdffkjvn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/ggmuryrbj.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/grdqxwfbk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/glgckrvti.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gouzozldo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/glmacwcxc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/ghhpcmisj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gaykglwvd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gvxvqqoji.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gckubbgwc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gimmxizxc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gybdmdwsn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giqtfimtp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/ghsvckgdz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gitgngtat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqgbfsqci.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/guopmkyzo.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gnguqmntu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gtarowpbu.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/glnvgmest.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gufezkmzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gglryjlyb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gpdhtpmgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggxnuiidv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gbmnvuovk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/grnouzrhu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gjdnfuyoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gxkgmageu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gtgofyyqu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gijtszjkn.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/grpktwoyv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gceidvstl.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gunbgdduy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gxrykhatt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gdlzqvgrc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gskiglqoi.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gtxrztstv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/govqzzogi.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbyuxuyjt.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gettdgqyd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gwuduupze.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/giwbysezv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gqcqexwkc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gwrgkbvsh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gfdciwpua.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gztlwzeuv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/ggpvfkjlc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gqlchekan.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gcaezdfuq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gxsrlbpot.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gjnpfakbw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gjavvtvty.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gguzftpkb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gtpyemqxb.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gflywebjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwpgwzqek.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gxxpvxbru.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/guxuueavg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gmyqorqhb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gdpmltlyo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gxbxapbda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/glepjbrym.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gupwghevl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gmecjlvqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ghrlkntrh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gkmsdficv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gulzmvlla.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gpuamvpgs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gillqhmcv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gvfgoibjj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gjmwqdhyo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gturjxdej.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gebdubqvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gfguzeatx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gbpukweuw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glnbiwqps.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/ggfhwrwfv.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/glgxrceyx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glqflhgdx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdfuorgus.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grdaqjdre.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gjfjdhsxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gzoplwvxs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gqvcbgxwn.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gdaxnacky.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gylonssqf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghilxfawv.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gytcsfabp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giushinmw.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/ggkktvmza.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gzoivqzzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gibjadzji.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gbcrxhmqx.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gdnteitjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/ghpbdkefg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gwihbiecj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gbdlvjslh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzfirhr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gwwwbtbjq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gizgljatp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gqtafflcr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gzmrlpyix.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/ghijgnxrw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggjhjtuhb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpghmji.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gpmjpvzse.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gelfapjuj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gezbhcecm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glmhmbdlr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gggegcegl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gfgdsqych.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gqbrrwtjb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gjqosfdcp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gdldjtnbs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gvmxhmjqg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gtmpkqiwm.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gydzvkbia.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gnhyqxvau.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gukshrcxs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gpzheawjf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gthtpawum.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gelymqgcm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gdjaqnvtx.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gycxbtdpr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gginkncte.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/guathcuvx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gdlclymbr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gnglfixua.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gbsfbvwdf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gztpffpsu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gwowbffov.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/ghjpzrhqj.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gezjspykm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/guwtzelfq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gwdftjdtd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gpjhawrje.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gmynyonas.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gyyusoxhp.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gttpvlsed.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfqamjbwa.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gzdxowutz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/ghypxypaj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gowlgyjxk.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gqxkpjrhd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gsuorvpjn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gzdqeovti.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/glnodzmrv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gwllzcrph.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gqqwuilbx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gnvboxyjw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gtndofxud.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gndxlmjdm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gcvxxkytg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gndfphbbx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gdpzzvxmb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gaawemukz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gmqexmuvd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gpjxpunci.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gszlzaqjl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gwocsbruj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gagqkapih.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gobhkzfcz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/garxwsyql.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gybjxrchx.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gfwtteuvt.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gqxkojajj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/ghycbilov.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gtjelaxnh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gnuapqkff.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gjdevaeps.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/giotyewzz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gptmqlbed.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gbzhulxxc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gblhkrqgo.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gxoobxfqr.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gkcczmxom.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gugoozulx.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ggbvccqob.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gnohcokrl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gpirrlnof.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gidtzqjqr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/ggwftvoqq.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gwaytfsqs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/ghkygrjik.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gezcqegqi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/grwpdcmkr.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gtluotfkc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/ghxgfkeos.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/geksrlxzy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gvaugmtpq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gzvubpxym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gkbqtrstc.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/glscbictb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmirbcvkr.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gdxxtkupa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gpjkwmlfy.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gcnhiptrw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gqbhmwlir.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjdeafi.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/geyhtlwuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gznxztscq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gjnazlamb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gjkwzrhvq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gmpynryts.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gkcvevcah.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfamtoohr.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gqjkcpufa.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqbutoxbt.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gmbybccck.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gehetjakc.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/glvaqdnub.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gcdteantd.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gzlfviooj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gfeuaitlk.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gfadpmkve.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gieplssdf.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/goepddhal.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gialuzxlv.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gfkhreoqr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gkijdumvg.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gwtnfggrg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gnyxvycon.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gohibhcjg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcwholukc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gephgwuyj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gmxwtbfrd.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gufmbqwbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghvivdfjb.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/guryiqgkm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkmpxlyjv.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gprmfyaln.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvbsgfvqg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxbnoeh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkkdbhrgq.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gmugqfygz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gibssdhvs.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gjaclwdlx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gwhonfdvc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/geojhcwcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/grxymkkkk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gbrdqgxip.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gbrloocve.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gcljpdyml.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/glijngfwu.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gkmgmjljd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gjlakptud.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyeeozkst.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gqfrwpcet.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbqzlxirx.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/grlqhbdfi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gtjlaeutr.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gpuaaunfe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gypkhqymc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/grdwcjapp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gymarbezg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gnkdzucxg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gdknhkflb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/grpumxhjq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gnyckbndv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gjzkafyzx.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/glnzpjfae.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmynllxfg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gokmjujzg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gjdevlndt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfrbidffc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gwxeetkqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjrlakr.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gdtmolkfu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gtznesuhn.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gjsfyvrxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/ghqzsqnkz.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/glgkrkryy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdsodraxs.sHtML


<!-- 参考信息 -->