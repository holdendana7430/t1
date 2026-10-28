代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtpkaugquj.html

================================================================================
来源：http://hz.tian-w.cn/gtdrsjxazk.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtbepxujhi.html

================================================================================
来源：http://hz.hnqzz.top/gtzrdoodpn.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtbokveetv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gthadokocj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shangyingyoupin.top/gtpmsoeezg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtklxyczmu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtobyyqysk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtwqisqkcx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtrcbvjjqw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ivvv.top/gtpqrytohp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gthyihvjmb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtygvtzybi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtenwciixa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gttkpzqtye.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtkwtttyvp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtjdjalmxs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtkfvjshiw.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtvdlazkwv.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtphobmbxv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtcqgliiqn.html

[N03] 快速排序（分治示例）
来源：http://hz.yuanzhike.top/gtutsrpuza.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtisoievth.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cdnleiting.top/gtkgocgtct.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtbkarxkdq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtzgkvaaws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtvjpoddpt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tian-w.cn/gtiutognqk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtwltxokjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtfebbsmof.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtpretzvxo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtdjfjqriv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtchvclarq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtskkfuvms.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtkdyymdst.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xylfe.cn/gtqapdjfzm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtigqcquuz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtpvgbyncs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtdraabmav.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtyuhvgrnu.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtvqhwkncy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtepjnxnvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtgsrmgzpf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtwauhqauc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtkmfpknob.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtjocrbcrd.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtrtmyvywq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtgutzzyny.html

[N06] 判断回文字符串
来源：http://hz.guannengcc.top/gtggwvuhbk.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtpzfltmul.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtelepxqcl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtkvhlyneq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtzkyuzncl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtbirvvfuj.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtuenapqte.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtprinrksb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtrjuxrywn.html

[N07] 两数之和（返回下标）
来源：http://hz.sxryk.cn/gtedgdnybl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtixmotydn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tianlin.xyz/gtnxvkbtsq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtzdkimunh.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gthjunfmhb.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gthropdvzn.html

Go:   // 手写 map[int]int
来源：http://hz.9152youxi.cn/gtvvxkcnhr.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtrwqyhgfo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtpradfzxv.html

[N08] 生成全排列
来源：http://hz.gogol.net.cn/gtlfntpddz.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtlserhhjf.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtirpxonde.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtdikkwdnf.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gteinqjaun.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtvancfuwo.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtjhetigxs.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gtxgzauhhd.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtadbqckvq.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gttpxehxgn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yueranfly.top/gtntnjnidy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sysykeji.top/gtvlayptpc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtrzguedbv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtclvzxlzo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhiwuduotai.top/gtjimgkkfy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sweek.top/gtmyaqdbmy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtnbzgjcfg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtrfhnjzff.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtpfviwpip.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtljuzjbkv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtwlrrrfca.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tianlin.xyz/gtollnzfnn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtkuzrdyyx.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtllxsibri.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtyxyemamk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gtxxinkhrl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtvqhxlmtu.html

[N11] 二叉树中序遍历
来源：http://hz.jyoumei.cn/gtocviaahd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daxiang520.top/gtdzfjbbxf.html

PHP:  // 手写递归函数
来源：http://hz.shanyushiyangtech.top/gtsndgkmrp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtwaudzwth.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gttgwyvsfw.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtukvsmsyi.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtmhqnqauh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.snrcjt.cn/gtjomdsmkr.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtuopglinz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj202588.top/gtrwxwdffr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtimdvyyhx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtwcdptxek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtnlcqozwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtovjoovte.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtltfziken.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtbqbrbadu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gttfkakjsn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtketwmdxr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtguvoqghj.html

O. 并发与异步
来源：http://hz.zhaomingkeji.xyz/gtjneyjznd.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjnitgvwf.html

[O01] 启动一个线程
来源：http://hz.daxiang520.top/gtpgyzzpfo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gtcygfgxqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtanwzyitk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pengpengdd.cyou/gteiugoxfj.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtngktyqqg.html

Java: new Thread(() -> f()).start()
来源：http://hz.pycfn.com/gtpganwfet.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtzymfquvi.html

Ruby: Thread.new { f }
来源：http://hz.ivvv.top/gttonpspfa.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtcuqrnaov.html

[O02] 使用线程池
来源：http://hz.yj20258.top/gttfitfwqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxinkj.top/gtycaypaad.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuxming.cn/gtsnqnotkq.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtvgsbzqsu.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtxzgevxlx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtawihcfqe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258.top/gtgzdsnixm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenzaomai.com/gtnqkhqazb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.smart0.xyz/gtyzmjzgcy.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gthdcwpgmc.html

Py:   with lock: shared += 1
来源：http://hz.fzhhl.top/gtjizpvdld.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuetiantiany.cn/gtzlckkruc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gtzmqcygkl.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtguyzghfk.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtrsugiuzj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtughenvgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuxming.cn/gtapejqyqj.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtppajnouz.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gtpeioppyv.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtfarpviwk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtjpsdspnd.html

JS:   async function f() { await g(); }
来源：http://hz.havefunace.top/gtcxohhohw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.meibo888.top/gtwzcqtjiz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtmvwocemj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gtyvyxmbbq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtiqqwhzkr.html

C#:   async Task F() { await G(); }
来源：http://hz.tianlin.xyz/gtjugtptjr.html

[O05] 并发执行并等待全部完成
来源：http://hz.gogol.net.cn/gtryxrebgb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtmjycbkwj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dashuyun.cn/gtgdfwwhre.html

JS:   await Promise.all(tasks)
来源：http://hz.yj20258888.top/gtsemmmqqo.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtfuyjzgra.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pengpengdd.cyou/gtwmtddxzu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangkeji.top/gtdabwknlt.html

Ruby: threads.map(&:join)
来源：http://hz.redwolf501.top/gtomysejre.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtyujduohj.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtdkksovmf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtvjenkiie.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtbqsxeifv.html

JS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtgbsgjooi.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtlskateko.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fzhhl.top/gtpegflpiq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtppgeugla.html

Ruby: // fork 块
来源：http://hz.yj20258888.top/gtjoclrleb.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtbwfrvhjd.html

================================================================================
来源：http://hz.gogol.net.cn/gtrxquzdft.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtrxoxnyxc.html

================================================================================
来源：http://hz.guannengcc.top/gthjxrhizm.html

[P01] 生成 UUID
来源：http://hz.gogol.net.cn/gthxytqcxp.html

Py:   str(uuid.uuid4())
来源：http://hz.tian-w.cn/gtuwdgybql.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jiagoushi.top/gtlbvbsskb.html

JS:   crypto.randomUUID()
来源：http://hz.wangdashe.top/gtqqeezwrc.html

TS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtklennyca.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtvdfyzbqo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.pycfn.com/gtktvgellu.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtcdeptcpp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cqqwz.cn/gtntotsbwy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtzhvsjwty.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtwrmrkqdh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydzc1.top/gtzpjfvxxt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.iojbl.cn/gtcyryamxy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtfbscsstm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenjidiqi.icu/gtwlgzxrqa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgfzy.top/gtwekufrdl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtjlmdfmav.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gtznvlhwue.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtstzuzrop.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtwxhwzwxw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtgtzgcjgs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtvcrutyca.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtfwwkjcoe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtvcmbqhtq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtmogwbpgj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtkopojfge.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gtxaadiczl.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtyatdnarh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtlxlpqrgn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtefxnufwg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtbmxrfgoc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtltlrsulw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtlyqqhjuf.html

Go:   len(arr);  len(m)
来源：http://hz.gzhubu.top/gtpseyhlsw.html

Ruby: x.length;  x.size
来源：http://hz.birdmap.top/gtbptkccdj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jlsjyb.cn/gtwzpvwlau.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtmxrlbske.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yangfankeji.com/gtgbxldnnp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.316326.xyz/gtsgwodflx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtpkbrsdtj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.birdmap.top/gtrajsqzcw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtkqpybkvr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj20258888.top/gtojgzyjoy.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtbjhwzdbu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aizwys.cn/gtspaqhuqf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtudriagni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jianghu66.top/gtvylaazsj.html

PHP:  if (empty($x)) {}
来源：http://hz.tanke756.top/gtbouohxsh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtqsfmjoxm.html

TS:   if (x == null) {}
来源：http://hz.jiagoushi.top/gtdlhayfiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xinyue.icu/gtinbppwmj.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtxwvmaofx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258888.top/gtdtzfzzpf.html

C#:   if (x is null) {}
来源：http://hz.yanxiufei.cn/gtwrhpcrlc.html

[P07] 防抖与节流
来源：http://hz.jiagoushi.top/gtwauzbeos.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtwlezpqtm.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtqbbpbcih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.0kj1m.cn/gthmxruxjw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtoalwdxyv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sweek.top/gtptneodvz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.52xcode.cn/gtwifedqvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtstpxxsmr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gtyhhmbuzf.html

[P08] 处理浮点精度问题
来源：http://hz.birdmap.top/gtetmrqroa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtmfsalcko.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtdntdcaqz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtivecdkip.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gtlbagnzdm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangkeji.top/gtmiigemca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtujogwgcw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtdlpsvdkn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtcqsvcant.html

================================================================================
来源：http://hz.sufxvd.cn/gtqapjwjkr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtevinlcwp.html

================================================================================
来源：http://hz.zdqjudy.top/gtqamswnlf.html

[Q01] 创建表
来源：http://hz.ydzc1.top/gttfibpolj.html

CREATE TABLE users (
来源：http://hz.xuetiantiany.cn/gttiwtryqt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgfzy.top/gtnncvthox.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhixingplan.top/gtzenutbso.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtafcaxqkf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtkcdwdchu.html

);
来源：http://hz.cqqwz.cn/gttfchywem.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtyesvymeg.html

CREATE TABLE orders (
来源：http://hz.yueranfly.top/gtqsnxcsec.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtqhfnkgmf.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtwdhvxiff.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtbhaadjor.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtkqpscgyt.html

);
来源：http://hz.jinyuanbaomall.cn/gttraeiftx.html

[Q03] 增加列
来源：http://hz.9152youxi.cn/gtyokbbszc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtijmnvtov.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtwtaatyle.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yvedp.cn/gtbqflxgll.html

[Q05] 重命名列
来源：http://hz.sxryk.cn/gtsdtzwgtd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtqrjqlsau.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtvjtctlyx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtvlaxzhya.html

[Q07] 删除表
来源：http://hz.xinyue.icu/gtvnrfvyqs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hysaishi.cn/gtvagxcrwc.html

[Q08] 创建普通索引
来源：http://hz.sweek.top/gtdimhjkvi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtdmyvcxrg.html

[Q09] 创建唯一索引
来源：http://hz.yvedp.cn/gtdjvpvdde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtsomnoayt.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtqaywsxco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtwtionbog.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtawxelbyo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgufenzy.top/gtqloocvhh.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtlambfumo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtnbjqzabf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gtoxdadmsf.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtilmfvyct.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jyoumei.cn/gteiavmclg.html

[Q14] 存在则更新（upsert）
来源：http://hz.svipenyu.cn/gtvdfhuquf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtnevuckxs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtqzoiplmj.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gteujkvkez.html

SELECT * FROM users;
来源：http://hz.xylfe.cn/gtqqjdawgr.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtifevrnlh.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gtynzexbjb.html

[Q17] 条件查询
来源：http://hz.shanyushiyangkeji.top/gtlvzsennq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gttadiciip.html

[Q18] 模糊匹配
来源：http://hz.nwbrower.top/gtjkgxvxpp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtiemxxtuj.html

[Q19] 范围查询
来源：http://hz.xinyue.icu/gtebykepdc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.redwolf501.top/gtyiwjqgac.html

[Q20] IN 列表
来源：http://hz.chenzaomai.com/gtvcmzficv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtajvfebls.html

[Q21] 空值判断
来源：http://hz.ywan-chungtsiang.top/gtxjxpzngq.html


<!-- 参考信息 -->