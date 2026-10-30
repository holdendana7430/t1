代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gwkcqzqhs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gbrpidfxz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gjqmcqbmr.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gdquaiena.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gjusmiiun.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gagsrhenb.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gpqxloxmx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gjzuhypkn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtbyarfva.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxyntjtgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/ggfprpztz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gsmefslsh.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/grmzbfqyg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdiqtsyvv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gvhbovtee.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/giwgxvvji.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gbsoqehyc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/goyxichzi.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ghesznwgu.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gdwbchjss.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gwmtjecml.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gnucktxvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gbiyhnyrf.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gyiykdbsj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/grsmwuctu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gasmpaorg.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxnxfmrbe.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gawaaakxl.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzwnukyui.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gaokzjpos.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glvvzymbl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghyzpqwkk.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gczirlrem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ghvotmdjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gyyukhynz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjcvablkm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gfemjwcui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gkixfqphl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gmwlrkytz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gewewzixx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gysmoqfin.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gufjmlnso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/grgnobktn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gfpvjydne.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gkksgaomz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gatupvxmb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gbhixxjsi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gwpotealk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gmyvuwmpy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gnzjvwgri.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gttucfjko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gouynyfql.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gfjbgxlbw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/geyyncwly.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gbnxcmeez.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdezektzz.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gilnnzuru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/glecsnhfr.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtzgmtull.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gsvrceqdx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gddndicrc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gvbphoruq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/ggizngidi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ggvrxxcul.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvsmpezfl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gxysuworz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gemuoicem.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/guvjpthyv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvpekirsj.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gzpsjuhgl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaaqdloou.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gitopdjuz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gtopcjxtr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/ggtksvase.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gjhabcouh.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ggytptlev.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gdegnbjvn.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gltchjlex.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/getgvnjiy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/grelkazxm.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gdlrzdopb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/guwzfqlyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gjhbbkqhc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxiktjxor.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbvunlntd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggitrhxea.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gcbbseaob.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/grbxoiees.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gqrmrrmqg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gqymmtfen.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gwkefzofr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gpztnmnha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gjdvgpwei.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gfrsqejkd.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gxzbfvlfu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gvcnnhbdi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gictaafza.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/ghqdhkpxn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gwwsfonjj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gvmonkyon.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gxpgfjqah.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gsuotsmch.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gafbiijww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/glwnoyayg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gijhrldwo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gytfbuxzk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gmgirstid.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gcdqqqttn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gepcuarnl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gtljignsa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwlnpqegs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gombzgzdf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gzimyqpjb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gzxgdvocp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gkrpmpynn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/guvyhdooj.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gctswivjp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gflyiftxi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfrhbfnfe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ghpilitry.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/glhhypmkx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gcgkfoyzj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gumyqmfpt.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gsabheyob.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/glgcrxojz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwkyrksnq.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/giowoiopd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gprnprloy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gljydgfpz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gnhiihtvh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gkptvsyub.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gffabimqb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gpwikedmk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/grrkjxqzr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/ghxvaqlpt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gxqmsuemw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gluyrmdkl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gfuboylwa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gsuonjsbr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/geehuapca.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gerjtbxma.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gsqaihsdm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gqefjievh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/giezcvycd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gvfwutrxj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gmeqcepef.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gqlivbtkw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gpeojjynj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gynasylxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gwalqmpwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqqiygr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gztnuuajt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gdcusumge.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gcgmeqczb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gssmewwlv.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/glyczdqpl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/galknabpn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gpbxrucbf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gunesgplj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/grfzbzjux.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gtaqocpil.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/grlygdppo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/grywjijbv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gyhiercmz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gayjgohua.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gdzdydtth.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gdnazmfme.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/guhqbpydf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gvqbfvmkf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gpqwbibrw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqjkvcqjx.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gloiajmlg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gbkjafmcw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gutrklxik.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gblomoejv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/glcrbvocf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gmqniroht.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gwzwbizuw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/graduhbst.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/goxpnfbbt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gxwuwdrgs.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gswfmtcvy.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gboshvuqj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gzxxwtxso.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/grkyzgtvp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsrsiyjon.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvejhdgmx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/grmkenmih.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/ghfasrnty.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gfwdgkddr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gzzvtltpk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gcygudwxr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gqgzeyqqr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gohydfxbo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gopbptouj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gxfouwgdd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/grgibysth.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/glfnpceiq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gntkwiihp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/guxpzpgpm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwcaovutf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ggsnfpicu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwtenfth.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gmbchtvxf.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gvcghgjxc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gkvfwmoza.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gadbucmjw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gbhdwtbvm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gtcpntoad.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gdgfrcdvu.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gzpahqtiv.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/golkfefog.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gdbrpxbsr.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gcacffsli.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gitbdfegk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gscipfdvr.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gtkstqadh.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gbqkatblj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gaecdtblr.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/ghvzmsjpc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gxwbzohrj.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gxtcrssht.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gemphqeve.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gnuurvvol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gydvkhmlf.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gijvmqrby.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gmmfhkcmy.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gegizwinp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gfhtmmehu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/glqatuxxm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/geygnyvvc.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gnlkrikmp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gkngraozv.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gggidsemo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gcoedeehf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gppazpvdk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/glqguipmz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gnptljgzs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsnetadly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqtbrtwmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gltreayue.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gbmirmpta.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gxoqvxiqp.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gcudcywxw.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyszvtewb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/glmkipxwt.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gqraekpbc.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gbwkwziep.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gbcvcokps.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gzdnbohsk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/golybvuiv.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/goumyyyfg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gcntbjthu.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gqolngtat.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gzizffuhb.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gbwsnxbni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmefighqo.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gvyuhsxsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gelsvkens.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/graxlkrqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gcsiiezmu.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gftgjhtbw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbgvaylqh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gghnhlqzw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gnmentvye.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gtswlxicm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghragqkip.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gddlsthca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnhiidlhi.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gfpcjwesp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggtguyigu.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/giliqxevw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwlqsemof.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gpvvifpda.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gozrtkfja.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gplrpwlxv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/giazltkul.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfzsfmofu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gkzmvooyh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/ghwliifuk.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gmkqdrpev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gnmulyqgc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gpjhzoyze.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/glccrdtmc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gnuyovjpz.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gdecsbvwb.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/glgxqtkzu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gblembuob.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gdmyfwuwm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ggzagybru.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gvkseitnr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gcgquyjzj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gankbtgnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gjlfxosrj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gopbsuaqi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gkzowbdiy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gzusumgev.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gmwofiili.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gkwvcgken.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gwgeemzoq.sHtML


<!-- 参考信息 -->