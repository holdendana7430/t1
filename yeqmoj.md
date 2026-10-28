代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtmihinvjo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sysykeji.top/gtpgoojahx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.svipenyu.cn/gttnypfkia.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtgrfikauc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtmatbidqm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtpmmzkzjd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtsrzuhibu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtclfihuzq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtfkqjudmy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtdssevmdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtvilblbxi.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtiavvumnc.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtskehhzyp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gtwqedtayd.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gtcqtmbiwk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtjjzpuupd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtcrqjpqfu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtgwkgercj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtjhmkkudt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtybdshejw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gturoelnsj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtyqxrcoia.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guowangkeji.top/gtdvatztps.html

[N04] 斐波那契数列
来源：http://hz.ehwqpu.com/gtxuxgwech.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtelpoifsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtkwmhxovk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtfyxlbtld.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yongpay.top/gtgfnegxag.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtdqigwwqb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yonumen.top/gtgrnjsmza.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtsuydoafq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtfcccsnkm.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtoamqxyhh.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtotdbnjpw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtutltxmft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtmzsqganh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtdiridkld.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhongyouzk.top/gtujanmvug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigufen.top/gttsoegekr.html

Ruby: a.gcd(b)
来源：http://hz.cucudq.cn/gtjnrzcedo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtmqvmtbbe.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtohrfgvxl.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtxvtxkrdr.html

PHP:  $s === strrev($s);
来源：http://hz.cucudq.cn/gtzqnjconl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gteqsfyqyj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtiocbruwq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenjidiqi.icu/gtfpjhivxb.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gtovliedzc.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gtutrbivyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gthtodrpre.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtcnunibpk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtvfwawkpu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtfvrzakio.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtuphdpacb.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtyqbanbny.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtqtjgimwd.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtapvukbbz.html

Ruby: // 手写 Hash
来源：http://hz.jyoumei.cn/gtnongdbdq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtcikgreow.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtrttpwfad.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtjxtnaqqy.html

PHP:  // 手写递归交换
来源：http://hz.wangdashe.top/gtbhxkbigt.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtpdgpxbgb.html

TS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtcgkmbxji.html

Java: // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtydittoqc.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtrwgauznu.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtydsjgopa.html

C#:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtnchquvld.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtwzgpjfhi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.pengpengdd.cyou/gtfaazjflc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtueosrqdd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gttqdjhtir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.haohaochexian.top/gtzpdclqip.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.c1oappe.top/gtjxhcmlkz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gotoacloud.top/gtshibekeb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtsvdabkjl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gthumofdxg.html

[N10] 链表节点定义
来源：http://hz.smart0.xyz/gtnvvqafnf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cashguo.top/gtmuaqglqe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenzaomai.com/gtmytkvgmf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gthhblehnc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sweek.top/gtaqwiukbg.html

Java: class Node { int v; Node next; }
来源：http://hz.aizwys.cn/gtvrzhalgp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinghuilouyu.cn/gtfqeytnpd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gtkpgdsrtw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shuidangran.top/gtbpruxlsm.html

[N11] 二叉树中序遍历
来源：http://hz.cdnleiting.top/gtmunewvbz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuanzx.com/gteoxebdey.html

PHP:  // 手写递归函数
来源：http://hz.jianghu66.top/gttzasprhn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtpvdiorbx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtsqyiouti.html

Java: // 手写递归
来源：http://hz.smart0.xyz/gtsghivakz.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtnupcedxb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gotoacloud.top/gtxvuplbub.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtlcefxvkw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjfxy.top/gtybpnjpbq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gtwyrwgreu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtjuwxfevr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtoadhkvii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtemoeojqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtrbgorzgw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj20258.top/gtpnycqklb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shuidangran.top/gtczajwtws.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtulxcsdxj.html

================================================================================
来源：http://hz.jiagoushi.top/gtatxypkcg.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtlefinhsa.html

================================================================================
来源：http://hz.guannengcc.top/gtmfjeckjy.html

[O01] 启动一个线程
来源：http://hz.0kj1m.cn/gtzgqajuyd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daxiang520.top/gtpdomyvoc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pycfn.com/gtlrszqwkb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtbpeznnzf.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtgvaqjtcc.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtbbdljiuz.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtjztkzucr.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtyxpsvroj.html

C#:   Task.Run(() => F());
来源：http://hz.jyoumei.cn/gtkonuujxf.html

[O02] 使用线程池
来源：http://hz.guannengcc.top/gtorrbcrxk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtsrzvowya.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtwyzmruvf.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtemhasotm.html

TS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtndkspzdd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtidfgyxdz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtmfbqgzsz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.iojbl.cn/gtqojdllbb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tanke756.top/gtcooscpzx.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtizquinjy.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtcmxlvtck.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gtehzohfra.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.bjfxy.top/gtakfsospc.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtcqoyolez.html

Java: synchronized (this) { shared++; }
来源：http://hz.quarkkingdee.top/gtzxxmnofr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ehwqpu.com/gtfdmcdbdz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gtbylwiepj.html

C#:   lock (gate) { shared++; }
来源：http://hz.316326.xyz/gtuyaylmfo.html

[O04] 定义异步函数并等待
来源：http://hz.ehwqpu.com/gtwpdjimkv.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtohqcbkys.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.snrcjt.cn/gtmwlostlv.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gtknrqxohj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinghuilouyu.cn/gtdhtymcbu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenlongwang.top/gtouisqmeu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gttgojbvsi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtatyfvgog.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtrjmrymcp.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtjyfhdmpv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cqqwz.cn/gtjsunrdpc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtgwhpdpml.html

JS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtyvihahzb.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtxtwscxqs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtewesjwdz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.havefunace.top/gtydyprpdt.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtipfsehcg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtjwuijyba.html

[O06] 使用进程池
来源：http://hz.dianchejie.cn/gtyrthtvjp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtfrodvqwm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtzjopgaqv.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtoexzhqvq.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtaccntqif.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtdctpdvoa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangtech.top/gtchncvmnj.html

Ruby: // fork 块
来源：http://hz.sxryk.cn/gtcfriisri.html

C#:   Parallel.For
来源：http://hz.yangfankeji.com/gtbalkiaob.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdgfidedb.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtyfqohdbh.html

================================================================================
来源：http://hz.yonumen.top/gtpcoqaedz.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtjtduqguz.html

Py:   str(uuid.uuid4())
来源：http://hz.tianlin.xyz/gtislqzjrk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtwmgdbscj.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtscldlaov.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtejebfoad.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuetiantiany.cn/gtlvnmdule.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenzaomai.com/gtkeesabbc.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtrnckwtxx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.52xcode.cn/gtzgxlmoay.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yonumen.top/gtphugcbgx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gteynrbgvg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtvroaphiy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtvpqgmasz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtjxkroysb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.haohaochexian.top/gtmsqzvcgy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtdifglguy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ydjk.org.cn/gthtyinluw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.daria6918.cn/gttldommzl.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtxwuhfkah.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhongyouzk.top/gtvxdldtoa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtsqzokleg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtyotmqdtv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtkrutlfso.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtkzbncjty.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gtdhobzlne.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hywenlv.cn/gthfqgvmxa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtzwidchwg.html

[P04] 求长度
来源：http://hz.bjfxy.top/gtnuvbwhui.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fengsongda.top/gtjninzuzv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtfpttuvnb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gttitjcyyg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sysykeji.top/gtivxtotar.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtgucpyecm.html

Go:   len(arr);  len(m)
来源：http://hz.tianlin.xyz/gtjvhmucvv.html

Ruby: x.length;  x.size
来源：http://hz.316326.xyz/gtmdngpeec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258888.top/gtsdxfjboj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtdchxtvzu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtvxflvdbk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtmtgjijwy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtswmnzson.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yueranfly.top/gtynwoqwvs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pycfn.com/gtfjoburkq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtedakplha.html

Ruby: a == b
来源：http://hz.sweek.top/gtmfiahnmd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtcaxovddm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gtnymjlluk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.haohaochexian.top/gtwkjrkmzx.html

PHP:  if (empty($x)) {}
来源：http://hz.sysykeji.top/gtbypputyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guannengcc.top/gtenhwlyst.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtcymvdeyh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtmttoggop.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtbkuhqqek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtdywofspg.html

C#:   if (x is null) {}
来源：http://hz.iojbl.cn/gtrlgbcwvk.html

[P07] 防抖与节流
来源：http://hz.shuidangran.top/gtdkaorbti.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gtnvaufmkw.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtzmwxepri.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtytjffpzh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtiubswbzx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xinyue.icu/gtolbaequh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gotoacloud.top/gtclbaasrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtgopzqaum.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hnxiangtu.top/gtqkvcijqf.html

[P08] 处理浮点精度问题
来源：http://hz.xylfe.cn/gtcwqumbqm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtanixpdqu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pengpengdd.cyou/gtmkehkfnj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuetiantiany.cn/gtjxgdrida.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.guannengcc.top/gtfsxelayd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtznvhjjhg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtctpeqpze.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhijiandao.cn/gtmekavclc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fzhhl.top/gtlfuxigbl.html

================================================================================
来源：http://hz.gzhubu.top/gtclvmpjox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtbbtjeyri.html

================================================================================
来源：http://hz.gogol.net.cn/gtfawesdxz.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtjyxwozux.html

CREATE TABLE users (
来源：http://hz.hfpthk.cn/gtozfavyfo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtvlapjrbc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenzaomai.com/gtqwozkpbz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtnlpjmkpv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtkduajoer.html

);
来源：http://hz.hysaishi.cn/gtiauqmgek.html

[Q02] 创建带外键的表
来源：http://hz.gotoacloud.top/gtjjhqdjny.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gthuffdbwa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gtyfscckfn.html

user_id INT NOT NULL,
来源：http://hz.sweek.top/gtwcazwqmm.html

amount DECIMAL(10, 2),
来源：http://hz.smart0.xyz/gtztaujhoc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.birdmap.top/gthlthkhqt.html

);
来源：http://hz.jiagoushi.top/gtlddqwazn.html

[Q03] 增加列
来源：http://hz.xuetiantiany.cn/gtrrbiviux.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yanxiufei.cn/gtrwqsvuvg.html

[Q04] 修改列类型
来源：http://hz.jinqigfzy.top/gtxwdzlgcf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jqgufenzy.top/gtnibexmww.html

[Q05] 重命名列
来源：http://hz.tanke756.top/gtlflglbvr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yueranfly.top/gtihdrldwv.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtnxpctexq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.9152youxi.cn/gtijwlwkuz.html

[Q07] 删除表
来源：http://hz.aizwys.cn/gtaxncwvjr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtszkjeysy.html

[Q08] 创建普通索引
来源：http://hz.pycfn.com/gtpguherfw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenjidiqi.icu/gtchajlhuo.html

[Q09] 创建唯一索引
来源：http://hz.yj20258.top/gtoegsfjpz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gtposkwkjh.html

[Q10] 插入单行
来源：http://hz.hysaishi.cn/gtjxeekujy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yongpay.top/gtpqopahcu.html

[Q11] 一次插入多行
来源：http://hz.kuanghao11.cn/gtpvlygyre.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.andypj.xyz/gtkkuqkhqh.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtnotpadbm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.snrcjt.cn/gtikhtxzmm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sufxvd.cn/gticxaiskh.html

[Q13] 忽略重复插入
来源：http://hz.shanyushiyangkeji.top/gtkgdxlqnj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ywan-chungtsiang.top/gtvnuuobyc.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangdashe.top/gtrsivofpp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtnqynmnwe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigfzy.top/gtmqebplet.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtvsayenri.html

SELECT * FROM users;
来源：http://hz.daria6918.cn/gtbfiijhnl.html

[Q16] 查询指定列
来源：http://hz.pengpengdd.cyou/gtjsowhsfx.html

SELECT id, name FROM users;
来源：http://hz.pycfn.com/gtvhhfxggh.html

[Q17] 条件查询
来源：http://hz.ivvv.top/gtesloadww.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangtech.top/gtcdvdcjvs.html

[Q18] 模糊匹配
来源：http://hz.chenlongwang.top/gtikjqowxh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtkdolrogz.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtdtbdptsa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dianchejie.cn/gtclwcpztq.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtylzvzqwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yanxiufei.cn/gtfclvcwhq.html

[Q21] 空值判断
来源：http://hz.hnqzz.top/gtkaicglba.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gtmpcmuvhc.html

[Q22] 排序
来源：http://hz.9152youxi.cn/gtgwmisgvs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ppjwa.cn/gtodukwish.html

[Q23] 分页
来源：http://hz.yangfankeji.com/gtdyzwkcgv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtlkkxkavp.html

[Q24] 去重
来源：http://hz.9152youxi.cn/gtmhlrezmq.html

SELECT DISTINCT city FROM users;
来源：http://hz.gogol.net.cn/gtvgjjyark.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gtzxwbdizi.html


<!-- 参考信息 -->