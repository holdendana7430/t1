代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtnyeiwhwx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtfenpypjs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtnvuyxgql.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtxnkwjggi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtyavblfum.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtvbhxxuyb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtfhscskeb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtuytxvupf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jianghu66.top/gtvxthbodz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gthagcxdlw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtwhxeusix.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtfjgpqafz.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtqaumpluj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtxulhsjdj.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtaohvjrax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gtjltvbmvn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shangyingyoupin.top/gtqngepcfo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtqbkubzza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtxdfiggjk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hongshengwenyu.top/gtecthuniq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hfpthk.cn/gtgcnrebaa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtqdbsageo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtvfihigum.html

[N04] 斐波那契数列
来源：http://hz.52xcode.cn/gtpgtsebqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtnmmfswrd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtpopuikqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gteiotggqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtnmpiwpeo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cdnleiting.top/gtfvnqhzvb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtzxxxaujk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtruooxyjs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xziqi.cn/gtttugqoea.html

[N05] 最大公约数
来源：http://hz.jianghu66.top/gtmcaviokj.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtipidowqe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gthjrwpnel.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtfbijarcl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtsugsyszc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgfzy.top/gtxqvmrbth.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuetiantiany.cn/gttvcfuaae.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtcwppprml.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtqoqawavg.html

[N06] 判断回文字符串
来源：http://hz.cashguo.top/gtuosohpwc.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gttbqwpeex.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtgcdyhzth.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtvukwtsar.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtwkyakcal.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtdjxwjyft.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gtqjeujcla.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtcukvnwvh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtjxlmyrsr.html

[N07] 两数之和（返回下标）
来源：http://hz.svipenyu.cn/gtgvvyljuw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtnxxlzydm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.snrcjt.cn/gtkpycdlha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.9152youxi.cn/gtlrkmgnlz.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gthnemdnzt.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtpjdiohij.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gthngqhtjg.html

Ruby: // 手写 Hash
来源：http://hz.aibaodan.cn/gthzozppsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtumrgrnvd.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtadleopgg.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtdrczomwb.html

PHP:  // 手写递归交换
来源：http://hz.chenlongwang.top/gtkqbpzwhr.html

JS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtrmtkffzv.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtdxeldaim.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtvuortzwi.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtdmhrhftb.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtklgjhbxe.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gttryymewr.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtwlgsroso.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtgrghnimi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtzojkfzhg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtznlgrkoa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtnnirguuu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sufxvd.cn/gtfssxntre.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtrgizhqfa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtzeimqaum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydjk.org.cn/gtnyhihmhq.html

[N10] 链表节点定义
来源：http://hz.ybcxt.top/gtsoaizdjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtgadiblsr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtlejmfrip.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtsjcxbvfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtmtnubpul.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtkixhqvuk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtlkwribwh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtchkdoijx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtfaxzcgxl.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtfxafyzuc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gtikvylsas.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtbhucedyn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtllkngccp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtkrpkpmnh.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtbpgrpnmo.html

Go:   // 手写递归
来源：http://hz.jinqigfzy.top/gtsqysevzw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtsxmzmcul.html

C#:   // 手写递归
来源：http://hz.zhoulong.xyz/gtyumqiwai.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aizwys.cn/gtsnpwmcnb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtdogagtgt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhaomingkeji.xyz/gtqctokrbw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtioyhifum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtuxbjancm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gthjlwqsls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtxotooqge.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtlieupezh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtadbyhkwv.html

================================================================================
来源：http://hz.hnqzz.top/gtveekusby.html

O. 并发与异步
来源：http://hz.ivvv.top/gtzkgjgbwu.html

================================================================================
来源：http://hz.yj202588.top/gtipyhxjfv.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtmfxmtwat.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtweikbwwl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zdqjudy.top/gtkewrxvdc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtqbyhmpvy.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtderixvkn.html

Java: new Thread(() -> f()).start()
来源：http://hz.shzxlz.cn/gtkrdgnkle.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtlpwrpdtf.html

Ruby: Thread.new { f }
来源：http://hz.jinghuilouyu.cn/gtjmlyhlbk.html

C#:   Task.Run(() => F());
来源：http://hz.zycfv.cn/gtpyoegdzc.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtctcvifzc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtdmjptyyt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ehwqpu.com/gthlhzjphw.html

JS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtqpfynonh.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtamigvkdo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj202588.top/gtjgfetzzj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtiwkamfkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtsztgtzci.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nwbrower.top/gtveoqitqe.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigfzy.top/gtdforoiix.html

Py:   with lock: shared += 1
来源：http://hz.hysaishi.cn/gteybwbxdy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tanke756.top/gtqinkmczz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangshuangyany.cn/gtvucpatyz.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtjajoyhhf.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gthrmnhake.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jqgfzy.top/gtbeniuwfy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtwslxiuix.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtdzdqzhpu.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtposgfcgj.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtmqfkydvp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtilnestqf.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtpzzcwroo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtqpsfocgb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtvbcueiuj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtucbieqge.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtyyiivqvr.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gteqzzpate.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtejvpnvlc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ehwqpu.com/gtktgnlvtd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtpjzhxwtn.html

JS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gttzosmlix.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtrakkmpty.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtbqboykxf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtafeofkhj.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gttzfladki.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtvxuthlfb.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtllleotqd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtdpwhaiuz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daxiang520.top/gtyghcdzzi.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtkxkwxpty.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtpixkdxrf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sysykeji.top/gtvzikixdz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ivvv.top/gtdkvnqkgp.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtmpagkhzb.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtfbtjcwgv.html

================================================================================
来源：http://hz.xylfe.cn/gtdlvmaqep.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtkxhuhupe.html

================================================================================
来源：http://hz.jlsjyb.cn/gtaiuyhbgb.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtedlkmtxq.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtbulqbeye.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtjcjvmgmy.html

JS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtiddohizu.html

TS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtplplzawp.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtlhtckfjt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtsqpomyuh.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtijkqmjen.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtdhihcmpm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangshuangyany.cn/gtymwqoutq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtezcxedcv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.smart0.xyz/gtrtmokmdp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zdqjudy.top/gtgxlmudcw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cqqwz.cn/gtbhkuuaux.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtmocigwqe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.c1oappe.top/gtlmfnsuek.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ivvv.top/gtlumkhvlh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hammf.cn/gtajkmzwxk.html

[P03] 生成短随机字符串
来源：http://hz.andypj.xyz/gtcqsxyasv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtshpwntbs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gteadgevli.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtyytavtmc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtjqunuxzr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yueranfly.top/gthyyrmurl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hnqzz.top/gtwvzozpke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtcjzjijxq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtcrzdnkws.html

[P04] 求长度
来源：http://hz.316326.xyz/gtggmsygbr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuetiantiany.cn/gtdgsxuefc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtcxwrrnuk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtdclueuzs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gtkheapllq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ppjwa.cn/gtokvfwzee.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtbvynyqvw.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtnqnkewln.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydjk.org.cn/gthrcfdazj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtrvimabau.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydzc1.top/gtoworcxia.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtmugjdvvm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtkyghcfwm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gtzjjevrdg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtbkuoxvsw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtgnjcfrdw.html

Ruby: a == b
来源：http://hz.316326.xyz/gtpefxhxba.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangshuangyany.cn/gtsjphkooa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dashuyun.cn/gtkhyrwehb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hnxiangtu.top/gtxscazmzs.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtzibivbmc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtptvpwcdc.html

TS:   if (x == null) {}
来源：http://hz.gotoacloud.top/gttfhsncab.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtapcouoze.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtlyquekzd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtdhveylgv.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gthbkwnlcb.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtsgltvijl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinqigfzy.top/gttecpnedl.html

PHP:  // 手写时间戳比较
来源：http://hz.tian-w.cn/gttzkbqesy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dianchejie.cn/gtlieljafa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtwxarozop.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gtfhaldvxc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtnzmozrcz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtlyhijpua.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gtpwqivvtz.html

[P08] 处理浮点精度问题
来源：http://hz.cqqwz.cn/gtbudqzmpa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtiorlbdvg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtdexnjsbw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtufpytroq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gotoacloud.top/gtcwoaztwj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnqzz.top/gtwwedazvi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jianghu66.top/gtmlqwulhu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhixingplan.top/gtamvsfmqq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.birdmap.top/gthsrmtdvz.html

================================================================================
来源：http://hz.cashguo.top/gtjdjekrzd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jiagoushi.top/gtyemrxaqg.html

================================================================================
来源：http://hz.hammf.cn/gtsgzgozwg.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtbfwdtvgc.html

CREATE TABLE users (
来源：http://hz.jyoumei.cn/gtsvnwjono.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dianchejie.cn/gtlnmbqmso.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nwbrower.top/gtydduhpwi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtovhmuhke.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.havefunace.top/gtdpyfwsue.html

);
来源：http://hz.guannengcc.top/gtxwgrarsf.html

[Q02] 创建带外键的表
来源：http://hz.nanxuanxn.top/gtnteothqa.html

CREATE TABLE orders (
来源：http://hz.jqgfzy.top/gthcvdgyot.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtuocukprx.html

user_id INT NOT NULL,
来源：http://hz.vqdsnc.cn/gtmaltuvgt.html

amount DECIMAL(10, 2),
来源：http://hz.haohaochexian.top/gtfkevirne.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtwssquyhi.html

);
来源：http://hz.hongshengwenyu.top/gteyevazaa.html

[Q03] 增加列
来源：http://hz.wangdashe.top/gtfbngohpe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenjidiqi.icu/gtsndeecpq.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtuxubrwcz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gttqeucnzs.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtbndtzmwr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtuvfsyyyk.html

[Q06] 删除列
来源：http://hz.zhengqikj.top/gtmzriaggn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.316326.xyz/gttvihrdxg.html

[Q07] 删除表
来源：http://hz.quarkkingdee.top/gtwolcllpw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.havefunace.top/gtecysyrnz.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gttsftrufy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtxssmresz.html

[Q09] 创建唯一索引
来源：http://hz.xuanzx.com/gtzponezvq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.nwbrower.top/gtrdgbvxhc.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtfoxusueb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fzhhl.top/gtzmlrdheu.html

[Q11] 一次插入多行
来源：http://hz.ehwqpu.com/gtsfucirbz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daxiang520.top/gtnyhathbe.html

[Q12] 插入后取自增 ID
来源：http://hz.hnxiangtu.top/gtyawqcurj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gtcomzfmst.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.52xcode.cn/gtvotddaqk.html

[Q13] 忽略重复插入
来源：http://hz.yuanzhike.top/gtorrfkunf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtqsafkati.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtwjrhlzkn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtlvgwxudm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtwvakkczb.html

[Q15] 查询全部
来源：http://hz.xuetiantiany.cn/gtahzjmaak.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtgxdbewev.html

[Q16] 查询指定列
来源：http://hz.aibaodan.cn/gtsobuplrj.html

SELECT id, name FROM users;
来源：http://hz.nanxinkj.top/gtuqrgfbtt.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtibocaztz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yanxiufei.cn/gtuugyfmls.html

[Q18] 模糊匹配
来源：http://hz.yangfankeji.com/gtrruwszik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtahvzqwce.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gtrqvunsii.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jianghu66.top/gtxjuspvgm.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gteltognvj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.c1oappe.top/gtwuplajha.html

[Q21] 空值判断
来源：http://hz.chenjidiqi.icu/gtgnncbgds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtzoaltdcn.html

[Q22] 排序
来源：http://hz.shanyushiyangtech.top/gtywupvdpv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtpzuxesrm.html

[Q23] 分页
来源：http://hz.xziqi.cn/gtoxnejuai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydjk.org.cn/gtnbfucksv.html

[Q24] 去重
来源：http://hz.jinqigufen.top/gtglvjgfnw.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtvyavzjff.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtupwdibrl.html


<!-- 参考信息 -->