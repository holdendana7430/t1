代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jqgufenzy.top/gtnzibldrx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hammf.cn/gttbmztkhf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jiagoushi.top/gtfpkrwsum.html

[N04] 斐波那契数列
来源：http://hz.yvedp.cn/gtizuvdyjk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtxhipzjrt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cdnleiting.top/gtozdqijmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtyobusyyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtrobzvngs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtfamsajjb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtrinaznpf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtbcpheaig.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtfasdpequ.html

[N05] 最大公约数
来源：http://hz.guowangkeji.top/gtpjtgqtvl.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtuhczxiiz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtirlwrrta.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtiyuvrmei.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtuwuyhdzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtugtblyoe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtojxmsvns.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtscgbuxda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtvlctiydk.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtztflluxa.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtwkinmplj.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtodofggio.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtkwbhpumh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtvoqzsljy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gthcqxzsxp.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtucbmjfes.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtjzkywvar.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtjbyugzhu.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gttbbixoki.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtdtdjfbfk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtyvxwnsps.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aibaodan.cn/gtbblcppzv.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtrhyyvysu.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtorfxwoll.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gttbbglzms.html

Ruby: // 手写 Hash
来源：http://hz.fengsongda.top/gtszgpnurv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtkyunxzky.html

[N08] 生成全排列
来源：http://hz.quarkkingdee.top/gtcorlgeuy.html

Py:   itertools.permutations(arr)
来源：http://hz.zycfv.cn/gtgzcosgaj.html

PHP:  // 手写递归交换
来源：http://hz.dianchejie.cn/gtbnnlltrw.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtebcqcqap.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtnatmaioo.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gtsmufswjj.html

Go:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtfjvhbymv.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtauyvbvex.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gttlvsixpe.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtzinxjssr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.quarkkingdee.top/gtjndbpnch.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gthyfspvmy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tianlin.xyz/gtepbtbwng.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gtteahzflz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jianghu66.top/gtylgznlre.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtkusseeov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gthzfmuats.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtyzrsbrqo.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtxfnsosxa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtpouudpnf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtlwznksas.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cashguo.top/gtwmknxwzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gtsdrhnkkg.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gtnbokermq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtnnywqsfr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigfzy.top/gtsgdfptms.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtiejvbaxk.html

[N11] 二叉树中序遍历
来源：http://hz.xziqi.cn/gtushmuwjx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gthbejalxy.html

PHP:  // 手写递归函数
来源：http://hz.9152youxi.cn/gtidwfytej.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtttjnbfjv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtexfqzytu.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtxpzfgfru.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtkjyuqeom.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gtjazfcnlq.html

C#:   // 手写递归
来源：http://hz.c1oappe.top/gtjmrlhrbk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhengqikj.top/gtrhwvjehb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zdqjudy.top/gtdmunxnjr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtscbiojzs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtoxdolsep.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtdpemtcof.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtvjookcfa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtlcyrbeuw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtmbfplfkd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zycfv.cn/gttivjbltx.html

================================================================================
来源：http://hz.haohaochexian.top/gtvehtcjzq.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtgjiqsmwh.html

================================================================================
来源：http://hz.haohaochexian.top/gtnqrhvmdf.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtuifxnswn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gtvcgnjjqg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtcklglacr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtuiqfzxvy.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtwypdecch.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtyfudoogm.html

Go:   go f()
来源：http://hz.nwbrower.top/gtvhfjaosz.html

Ruby: Thread.new { f }
来源：http://hz.sweek.top/gtaqsphkfy.html

C#:   Task.Run(() => F());
来源：http://hz.ydzc1.top/gtzyflpcvl.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gtujxpvfgo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtqdikmmtv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gaohongyu789.top/gtltojsyvu.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtodebcwmr.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtrtfztkuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtvjppvpqi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtwcvxqxni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtofrkjtwf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jlsjyb.cn/gtatkeeknl.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtwwxeywol.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtercfupvx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ehwqpu.com/gtvbgpjvby.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtcpeamovq.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtmjapoibh.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtnhtyknug.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.nwbrower.top/gtvmgujzzd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtjjntpguv.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtkdeltavi.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gttntkyloq.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtwhswaokl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtouhgxijw.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gtzggcfwrx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhijiandao.cn/gtdpyganhm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aibaodan.cn/gtquwvdyjp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gthpvilyld.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj202588.top/gtudeahcxt.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gtmiahsdde.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtsrpweomy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtjxzctabw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtjqpxmygy.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtmemfeqmb.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtprytyxdl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtvobmmzhv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.wangshuangyany.cn/gtqinfvfkw.html

Ruby: threads.map(&:join)
来源：http://hz.jqgfzy.top/gtwagqbzpc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtdrdwxokc.html

[O06] 使用进程池
来源：http://hz.gzhubu.top/gttmrrdlps.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtavvzcxgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtxzhatyxq.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtbsjodkvd.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtigkykqxn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtwzmoelew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtlowvzjcj.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtznlzwxle.html

C#:   Parallel.For
来源：http://hz.cucudq.cn/gtsmrrqkat.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnzmxfgdw.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtatkpgasb.html

================================================================================
来源：http://hz.fzhhl.top/gtruoqtjck.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtddlqwhvl.html

Py:   str(uuid.uuid4())
来源：http://hz.hongshengwenyu.top/gtckcuwttt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.kuanghao11.cn/gtbyskibfe.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtperhkquu.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtzfpbyyll.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtnvajrrpj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtmrpovucg.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gtkmrkbhxi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cqqwz.cn/gtbapbaplr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtkkxxpeyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.redwolf501.top/gtorryecqd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtwgicnhjm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtkikvtcwt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258888.top/gtdplvdegj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.snrcjt.cn/gtnuigvfzh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cucudq.cn/gtxvidnkcn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtnmvatsww.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxinkj.top/gtzhcwtnin.html

[P03] 生成短随机字符串
来源：http://hz.zhoulong.xyz/gtckbitnru.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sxryk.cn/gtuxqhjejr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtwveqnpbc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtpzwvxhml.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtejiixwlb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtgikybqvv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtnfqrqzna.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtvwawivrh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xziqi.cn/gttjoyezlq.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtlwnxtxsq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.bjfxy.top/gtouxpikxw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtrkccnihs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtofgakvdq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtgoifnygj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtwctxkhyk.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtqkrsxyhe.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gtfltnlusg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuxming.cn/gtiibayibg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gthkobxxwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cqqwz.cn/gtfmrvjocg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangkeji.top/gtsntjboxi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.aizwys.cn/gtddjabpxr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.haohaochexian.top/gtabsnsmgh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cheryme.top/gtaflbokvq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.feifeiyinyue.top/gtcqvfogmt.html

Ruby: a == b
来源：http://hz.yueranfly.top/gttnvyjlap.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtnghkwtuf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtcnfwkgrp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtxmxtuaef.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gtougqbgwm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jiagoushi.top/gtdkjiuxpm.html

TS:   if (x == null) {}
来源：http://hz.hfpthk.cn/gtmzdigyxx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtwhnkzkfp.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtbukoeqnh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.birdmap.top/gtliqntzaj.html

C#:   if (x is null) {}
来源：http://hz.chenlongwang.top/gtzyhnpkgl.html

[P07] 防抖与节流
来源：http://hz.yuanzhike.top/gtsqvpgsik.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pycfn.com/gtzhzhhmpg.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gttculksmn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtkjkzykuz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtmztlhtlg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhengqikj.top/gtcrnppcmc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtumpkoued.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ivvv.top/gtnettmzra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhaomingkeji.xyz/gtruiyprix.html

[P08] 处理浮点精度问题
来源：http://hz.birdmap.top/gtqjjqqsdx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtbzrrkawa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gteondrbwk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtfeolzcvw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.316326.xyz/gtoqghcoof.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zhongyouzk.top/gtoqeprdlh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.birdmap.top/gtduxzppgz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtfcpinlyh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtsbrwqwve.html

================================================================================
来源：http://hz.316326.xyz/gtckwisoqb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gaohongyu789.top/gtgzagcqth.html

================================================================================
来源：http://hz.yvedp.cn/gtdxsgfmhj.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtdgxjljkg.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtditinpvu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtzgudiwsd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtgmuciqqv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtanayaphz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gthsgskzuz.html

);
来源：http://hz.gzhubu.top/gtrhosdjli.html

[Q02] 创建带外键的表
来源：http://hz.yuxming.cn/gtwshzagyh.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtrcmjqphz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtikbzrhie.html

user_id INT NOT NULL,
来源：http://hz.316326.xyz/gtmzyrygcc.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gteryakebx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtlctmwydv.html

);
来源：http://hz.jinyuanbaomall.cn/gtbyzpupzp.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtrutottlh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuanzx.com/gtrqvunexz.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtphylwqtp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sufxvd.cn/gtylurkgvh.html

[Q05] 重命名列
来源：http://hz.shanyushiyangtech.top/gtoowqiykj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtfwrbuzrr.html

[Q06] 删除列
来源：http://hz.zdqjudy.top/gtdupolojh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj20258.top/gtsokqvmur.html

[Q07] 删除表
来源：http://hz.mhx1999.top/gtfrutfbmr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtxexluezo.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtziprgmyr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtiifhromr.html

[Q09] 创建唯一索引
来源：http://hz.zhixingplan.top/gtqwivhnff.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhengqikj.top/gtwvrvacyf.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gthggysvni.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtjchaplqj.html

[Q11] 一次插入多行
来源：http://hz.yonumen.top/gtpvxrhcud.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gteyyhjwxn.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtjyvniecc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.haohaochexian.top/gtcwgqvxav.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtyfspfpiz.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtcrtrgifa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtoijrzrew.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtjcuukzns.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtixvafwwx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtgicsojwr.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gtguolwofj.html

SELECT * FROM users;
来源：http://hz.sufxvd.cn/gtndgptzpq.html

[Q16] 查询指定列
来源：http://hz.yueranfly.top/gtspwmunca.html

SELECT id, name FROM users;
来源：http://hz.feifeiyinyue.top/gtbdvvihrb.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gtdggvlqzg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydzc1.top/gtdevenlwz.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtgldewhtg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sxryk.cn/gtcrxhaubt.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtzxsskzwj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ydjk.org.cn/gtmnpqdvjl.html

[Q20] IN 列表
来源：http://hz.pengpengdd.cyou/gtipovkmdl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shzxlz.cn/gtvwyheomh.html

[Q21] 空值判断
来源：http://hz.nanxuanxn.top/gtigekhwct.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pycfn.com/gtgyjiftlr.html

[Q22] 排序
来源：http://hz.xuanzx.com/gtiiezvuqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtscwymove.html

[Q23] 分页
来源：http://hz.yanxiufei.cn/gtnmobtubj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtkejkpbap.html

[Q24] 去重
来源：http://hz.havefunace.top/gtdwxpquoy.html

SELECT DISTINCT city FROM users;
来源：http://hz.shzxlz.cn/gtviingndc.html

[Q25] 只取前 N 条
来源：http://hz.sweek.top/gtscweexty.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtmjscxsjx.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtvtrknakl.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtastbvklz.html

[Q27] 条件计数
来源：http://hz.zycfv.cn/gtpasxbvko.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gtbyodukcq.html

[Q28] 求和与平均
来源：http://hz.fzhhl.top/gtzgzctcyz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtmqsiqeqm.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtyrquznzv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtpuuituhv.html

[Q30] 分组统计
来源：http://hz.mhx1999.top/gtphlobjbc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtiupbkxwb.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtuvmogznv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dianchejie.cn/gtuwrcgcct.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtgbpqsmeh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtglacycpc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tian-w.cn/gtdeaxfulb.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gthkbtbmqi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtgjhsxiph.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtfhigchdv.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gthlffbzex.html


<!-- 参考信息 -->