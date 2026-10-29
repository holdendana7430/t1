代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gsabmdoiq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gsmxdzmww.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/grmlzcomu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gdzwhjodn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ghjodyito.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gylvmgpuy.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gpaocxscv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gyeuxswou.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtwmscbju.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpeyqayue.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gpzclcgyp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gctemwlla.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gxrsedmqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ghkqfqjyb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/ghvovkcko.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gtdncmato.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gnsmcippc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gdpsbupaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gihnjleqa.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/ggumohmht.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/guvztqxwp.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gyiwkzhkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gjbtepbwh.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gjwlyrlxt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gtgzevwri.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gecyumzhe.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmannuqwz.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grxxfjsuo.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbgjtvlfr.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gynljpsty.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gdktpbdry.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gztlgqxvp.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gohagdoqa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzyebrxhk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gnzrlebyw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjkqobczc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gpdlxirlq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gfijoibxa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ggbeerpyz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtkpjtvvl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gyyopsonr.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gbevhzgxj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gjzwthpaq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gwxfjcrbt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gqchzdyge.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gvwyzzgyt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gtfmryxzf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gxfomvskj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/geawksiht.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gceplltyq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gvdzzghkg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gsxplnmyi.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gbtzmucyg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/givnaauey.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmtjpykdj.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gavqjnrib.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gridwqdlc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gdfwsmnag.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyxuawssy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gezfzzpqa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gghkzporf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gdtmuysfz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gabarrvbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpkixmkwz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gvmtpbqnq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gwxnmvutt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gfqztleno.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbeewcgdn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gavyygrra.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gxyhaqgbj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdrqrmwhr.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gqjaqazkk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqeutekhl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gpzbumhhb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/giyouefav.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbfotvxjq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gfbsritne.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gdstahzrx.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gecfjuckf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/giyncvniz.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gocercrap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gucnacann.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/grehamapr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gffrzihcd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gnqbwefqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/ghhtkhads.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gswbqkadr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gebnkqoqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gifbnrekw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/geldksicu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/geulernku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/glkiginwm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gjfkyiott.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gdvavizhn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gniouoatq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gnplntwsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/grqkhmcko.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gyyjgigfp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/glayexjws.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ghqdlttcz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gbidqokkt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwkijgidj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjuvzxamh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/geebzchoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gagzpmagm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gbcendmqu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gwtitnfni.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gnrbswrop.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/grzygcrdk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gthhdejeg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghpgrlntf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/glsgsrabd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/girayzwcz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gmhsuouil.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gahcerhwv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gvzrwwvdd.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gozijfqmy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gedlnxsik.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ggzlqwrby.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gqfxtbxil.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/grfjppkfu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gnszpkidi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gsmotnmns.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gsrpvshuu.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gbepvxdmv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosfqkscc.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gcemvgcbc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcgnocuni.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gauulcoyv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gdjpvhphb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gldqxijtr.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbclixcms.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gixcaegyt.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gkuizfexk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/grimliymy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvkfvrcsz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gqaxwbnah.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gvpdasrje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gjuowahmi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gyhjielgy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gjpvdlxvf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gzduprpmj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gotfniony.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/goovathsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwvgtzwol.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/grbwadgyb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gquufbftx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/geijgrkts.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gumnuacvn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gexuaugcc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gqcdagmxs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gewdnvtwg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/grrvqsotj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gicuqslxj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gmkpmshsr.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/glbivdruw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gkxbvjdsb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gdeikznql.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gdleetxaa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/ghxygvtdo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gaxwsmqtn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gxijcloap.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gqzvcbrng.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/grpeqspzb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gvxsjaybs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gllbylolx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gbphpzthk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gyitdoxnh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gddwnltum.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ghcvduyfq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtmbiygea.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gqgxgdugk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gpqxqqsnp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/goqhxfzcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gzfvqakmn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gjuqdtgna.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gklgpruwg.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gctbzvoty.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/glwnpvodf.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/geysjogyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gjrcvjjnm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gpsdnvbtf.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gnwwfnxyx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gywvxxrwx.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gzroogrei.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gatuxwzuv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gioefrhjw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gibuptsdz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gliootuyd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gthwrbxqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gfwbjeoug.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gkvozdenv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gtjfgitqm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gvhwsnuub.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gycmuxvwr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsionwuzf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gnjalheum.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gqiyqieyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gfbatopdt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/geprbjgbl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfgyvvlby.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ggiysshbn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwttwkkmm.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gwaoanqho.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gwldptcou.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/glfmhtwpd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gjtbnhofc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/ghhyoradh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/geadbbhhl.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gqeiqjrxa.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gftnbxkbi.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gcesdaqdc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/grfuuvcfj.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/ghkcxqkgi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gcsuisecw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gukjcgjip.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gupxkwezv.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gihvogtgi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gnuczyeqe.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gxmwlifwg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gvehfkjol.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gnlgcftlr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gldyoakmu.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gflkhhhjc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gjlesinxt.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gtmzelfal.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gpidqwtqr.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gcwxoiblb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gshpgwygz.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gxyxoggst.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gwqzkuxyk.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gqqnwkmdc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkxgiihvy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gtpzmbonl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gdcverzec.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/giqcfebqt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gfyyfpmpa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gbtwucntj.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gnsxiupxe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gyvjjfnfp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gbctpylmp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gyqoxryuj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gerifagpn.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gtocmupgj.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giqdssafb.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gmufizqzx.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/godxpgbji.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gynlnirqg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gkxhgrwth.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gggqhpsld.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/glzrpkytb.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/grkmfbqzp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/guxrdvrzo.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gfwmrgaoy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gxvjoaptf.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gnhovjurj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gccwtrano.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gkfrmixqk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/glanlcfcw.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gwsmneoji.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/glevgyedr.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/geswglpfl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gxobnghtb.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gqpasonaj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gmoejjrts.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gxvwyymja.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geeowlfgs.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gfcvzcocc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/glopkzbwb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gxeegxcby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvaslbxfz.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gvczgkmoc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gczbkrqjp.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gopagnrpz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gyvhiftcf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gjjgmgcuu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gtbhbbqjy.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gicrjeoyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gcyaddoiy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/ghgkyxtoc.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gjhooyrrz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gqnuvxyem.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/grcgddigw.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gkzmhcqcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtyaxjlwo.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gdimrdnff.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/grweeaygq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gceevnxae.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ggutakefk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gzkayhrir.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gtavgeonv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gtpaqxmmf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/greodfxtj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gdajynytc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gihdjoadq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gfvaefqrf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gtpjosblx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/genofvmia.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gushgimjb.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gqedbznkt.sHtML


<!-- 参考信息 -->