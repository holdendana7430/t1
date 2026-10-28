代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtpvvmvdjc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtunprjnnh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtwtuyxbiw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hammf.cn/gtsjhldlng.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtrxfhwljb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.quarkkingdee.top/gtwhfyyukf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtmfwwvilo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtrqgujljo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtjaqwpusf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtifyxqpcb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtdawnhgqf.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtdxkvifto.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtbghycmce.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtojpvcfen.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtdnwffizg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtormjpkgk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtjzzwhgps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtdaazdwin.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtfmobpnkh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gthygeusey.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtavlsxwcw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtcuzhkjhg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nwbrower.top/gtcwbaflwo.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gthvhfvxks.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtossndnvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgufenzy.top/gtfelgqvup.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtjsatgooh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtmcalzltc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtkjjypvqi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtzgdgtxwh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtdjdflboe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yueranfly.top/gtfzfxolgg.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtntfkkfee.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtwfrotaec.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ivvv.top/gtzcmcflih.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtpbzlzvbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtmvkfywxp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtjpvqglig.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtfjwpwxha.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtdihtejog.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gtanooclko.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtxgkzqezd.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtohapgxgu.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtmvolzium.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtivtoubzd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gtcgncdjqj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gthryzgrem.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtgnjuhbxn.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtntmjcjvp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gthbixgrsh.html

[N07] 两数之和（返回下标）
来源：http://hz.zhoulong.xyz/gtelokfrmi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtwjpscipb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtysmicmyh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zdqjudy.top/gthgndneii.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtxvhbmelr.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtsfxhgwms.html

Go:   // 手写 map[int]int
来源：http://hz.haohaochexian.top/gttzkyajlg.html

Ruby: // 手写 Hash
来源：http://hz.vqdsnc.cn/gtmdvqvgss.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gterguedgl.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtzioamofc.html

Py:   itertools.permutations(arr)
来源：http://hz.havefunace.top/gtatwzvhsf.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtabpelzio.html

JS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gthconcnas.html

TS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtefeermkd.html

Java: // 手写回溯递归
来源：http://hz.shzxlz.cn/gtdtqbftgv.html

Go:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtyyjiayea.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtbnxnvbpx.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtvrmipeph.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtnudmqdxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtfkqmbyaw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.havefunace.top/gtzijyqurh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtfyfhoocj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtxedczutd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gthipqvfix.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtgmphckfx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258888.top/gtfidyfjtt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtkmoubtwd.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtnbsjlpgw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtcidxfeip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtleghcfha.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gtiiyxyvuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtfoiyefed.html

Java: class Node { int v; Node next; }
来源：http://hz.tanke756.top/gtnfyepueg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtonzwqzah.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtdodkhtau.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtfheyuqon.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtjtsahter.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtvtdripbh.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gtdcdthlsb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtlhjguocm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtftnmsrkn.html

Java: // 手写递归
来源：http://hz.cucudq.cn/gtrrtdtgiv.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtayxztpsw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtnzsaardc.html

C#:   // 手写递归
来源：http://hz.tian-w.cn/gtkqlqgppf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.iojbl.cn/gtazwjyxlu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gzhubu.top/gtvmalgken.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtkojsmztu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtfgakcgtw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gttronpbyx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtovzwbvjv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hywenlv.cn/gtxcfzobwt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtokumpdox.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtxfpkntut.html

================================================================================
来源：http://hz.zhoulong.xyz/gtutrhullr.html

O. 并发与异步
来源：http://hz.shzxlz.cn/gtbkcfmwst.html

================================================================================
来源：http://hz.hysaishi.cn/gtrmtxtkme.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtutdnbmos.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtzayzjetb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sufxvd.cn/gtflxoiwyx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtzoqppuvl.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtluftllqe.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangkeji.top/gtimxjdzyl.html

Go:   go f()
来源：http://hz.wangdashe.top/gtrnqpmktc.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtjihjfect.html

C#:   Task.Run(() => F());
来源：http://hz.bjfxy.top/gtsvrjzeon.html

[O02] 使用线程池
来源：http://hz.guannengcc.top/gtpztvwnqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.0kj1m.cn/gtcyarpklw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtenukvwna.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtrtjzwrvn.html

TS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtupzptytb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtbpbfxbrj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuetiantiany.cn/gtmjinzjly.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtgnwusxrd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.iojbl.cn/gtmkfksozu.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtdjqwserc.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtnfkztfjz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtcidcmoea.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ppjwa.cn/gtsqhrfvvd.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtmqxlwrmp.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtwsszqrbz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtwebtrmfd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gttbbyemod.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtiltkrynq.html

[O04] 定义异步函数并等待
来源：http://hz.pengpengdd.cyou/gtrcceemow.html

Py:   async def f():⏎    await g()
来源：http://hz.tianlin.xyz/gtkrynikos.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtoqahpfjz.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtjytokkiw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ppjwa.cn/gtzeecrnxp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fengsongda.top/gtgrrzyqos.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dashuyun.cn/gtkxofalsw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hfpthk.cn/gtkukqcgbx.html

C#:   async Task F() { await G(); }
来源：http://hz.yuanzhike.top/gtvvxtcsfn.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtounamqtz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinyuanbaomall.cn/gtontclhxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pengpengdd.cyou/gtcjlabqay.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtpfypotsd.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtncmaefxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gttqefrnrz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtjrnddsga.html

Ruby: threads.map(&:join)
来源：http://hz.jlsjyb.cn/gtozwekwus.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhiwuduotai.top/gtziqgbbep.html

[O06] 使用进程池
来源：http://hz.andypj.xyz/gtmuaxvdcz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.haohaochexian.top/gtnriwfcdl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ybcxt.top/gtantkquam.html

JS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtgakqdupf.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtjwfmkbuf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtczblipiz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtdsyntija.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtovgnmzte.html

C#:   Parallel.For
来源：http://hz.guowangkeji.top/gtosxmdocu.html

================================================================================
来源：http://hz.yvedp.cn/gtsvzflomo.html

P. 常用工具函数
来源：http://hz.sweek.top/gtyubsarxo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtoslmqinr.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtvimaafxw.html

Py:   str(uuid.uuid4())
来源：http://hz.ywan-chungtsiang.top/gtzuqmzbtc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258.top/gtxbjalgcp.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtlyrrsngc.html

TS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtlizshejz.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtvweavvgd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtkgxyxnmw.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtvqxbuikf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yangfankeji.com/gtboajviph.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxinkj.top/gtddnzmfea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenzaomai.com/gtqlojysgb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.feifeiyinyue.top/gtqcgvkfmc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgufenzy.top/gtkzymfwsf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gtcrgfovgg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtxupsqclb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.haohaochexian.top/gtrksrsmup.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shzxlz.cn/gtjwfvcetv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtjmtktear.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtovifevmw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtqivvkgmv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtjsinxpqr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.bjfxy.top/gtrgyaoewh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhoulong.xyz/gtxyaclrlp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtknxcxajp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtdlglmzta.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtwradrvbf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtafpauxfo.html

[P04] 求长度
来源：http://hz.ivvv.top/gtrnrnjeab.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtbhzoomgj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtehoqzldg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gtlvcdesmy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtxaxgofqu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ywan-chungtsiang.top/gtzivwijab.html

Go:   len(arr);  len(m)
来源：http://hz.fzhhl.top/gteeuymytk.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gthlloidbb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gtxtphbpfp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtihvxfqsm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jlsjyb.cn/gtvgpbxkhl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gttgpvgevf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtkgqgdtau.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gttatxzigp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gthbrpruos.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtvhsecshl.html

Ruby: a == b
来源：http://hz.yanxiufei.cn/gtpckwsivw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuanzx.com/gtqwnurruv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtneylqrrj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.c1oappe.top/gtzxydtbmj.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtywvbnqgx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jianghu66.top/gtbnmcgyty.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtivhfkdtg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtoikhsnfk.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtqucvigmw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cqqwz.cn/gtgfqgixfu.html

C#:   if (x is null) {}
来源：http://hz.yuanzhike.top/gtznjdjvpn.html

[P07] 防抖与节流
来源：http://hz.ydjk.org.cn/gtbpnqtfrt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gotoacloud.top/gtwwhbrbwf.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtcicszxqc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtzdlazvlf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtpezwftjx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hongshengwenyu.top/gtbnasxnte.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cucudq.cn/gtjzlqtyjx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenzaomai.com/gttsmqlkqm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigufen.top/gtlcddipha.html

[P08] 处理浮点精度问题
来源：http://hz.daxiang520.top/gtjvotophj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtosmvjeld.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtdrhpllef.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtbnjnsmvb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.c1oappe.top/gtzwwzmeax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtpescrlez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xylfe.cn/gtupqnitdj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hammf.cn/gtsyqmbzvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gaohongyu789.top/gtgxsohhsw.html

================================================================================
来源：http://hz.tanke756.top/gtwbtszgxh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.meibo888.top/gtjzqybicg.html

================================================================================
来源：http://hz.snrcjt.cn/gtqawmfiba.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gteulncrsn.html

CREATE TABLE users (
来源：http://hz.guowangkeji.top/gtybtgrvoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtoszmctam.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtymvztexa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.chenjidiqi.icu/gtnqoxfewu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtvarhvfhi.html

);
来源：http://hz.zycfv.cn/gthqrujrcv.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtaygqchna.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtnedddesg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtkpxkdpjw.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtzkxkgyou.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtmxcnlmia.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtstsarvcu.html

);
来源：http://hz.jiagoushi.top/gtfxstgoyb.html

[Q03] 增加列
来源：http://hz.shzxlz.cn/gtahxgmavc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.bjfxy.top/gtelbvrhuh.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtacqwukeo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtmctrkltr.html

[Q05] 重命名列
来源：http://hz.bjfxy.top/gtgebervmr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtcjocynjh.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtsuwjycxv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxuanxn.top/gtoxfmekld.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtynnhswwx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtyrqyrmwz.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtknjelptw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hysaishi.cn/gttocpozgs.html

[Q09] 创建唯一索引
来源：http://hz.zhengqikj.top/gtoekiwdrz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtllamliue.html

[Q10] 插入单行
来源：http://hz.xuetiantiany.cn/gtxqchdjoz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinyuanbaomall.cn/gtrsitnhoa.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gttahhmjbb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtxgfzeajh.html

[Q12] 插入后取自增 ID
来源：http://hz.tian-w.cn/gtjjiletqk.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtywrnxqyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gttztkfngc.html

[Q13] 忽略重复插入
来源：http://hz.ppjwa.cn/gtisagknbw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtjoaocohk.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenlongwang.top/gtzutzabtw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.haohaochexian.top/gtusukjozz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtjvbhgpvo.html

[Q15] 查询全部
来源：http://hz.jinghuilouyu.cn/gtrldcjjfj.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gthaykgbvt.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangtech.top/gtjftfahpt.html

SELECT id, name FROM users;
来源：http://hz.wangshuangyany.cn/gtpdciftlp.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtczkigvsv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gttscazlin.html

[Q18] 模糊匹配
来源：http://hz.shuidangran.top/gtwtkwinew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtfqspqgcu.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtdyxeahff.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtmjvnqdcn.html

[Q20] IN 列表
来源：http://hz.smart0.xyz/gtgbrmrzac.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenjidiqi.icu/gtuucvuxxk.html

[Q21] 空值判断
来源：http://hz.sweek.top/gtptftzidh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.havefunace.top/gtkgsbgjqt.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtdultgkyn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hfpthk.cn/gtcgqjmiwp.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtriqswjts.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hnxiangtu.top/gtysdeyueg.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtdupwwjfi.html

SELECT DISTINCT city FROM users;
来源：http://hz.chenjidiqi.icu/gtsaiuqrmh.html

[Q25] 只取前 N 条
来源：http://hz.andypj.xyz/gtvrnhkbvo.html


<!-- 参考信息 -->