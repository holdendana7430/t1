代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.52xcode.cn/gtmzbafwem.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtryecqvzs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtrhwrqdoi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtegllvsvp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gthugrnlce.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fzhhl.top/gtxavtxpky.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhengqikj.top/gthxsfyqxn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.316326.xyz/gtstakumls.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtovsucojo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnqzz.top/gtjqbbfawc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtmkcbpigr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtsxchdlpo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtcimqfexk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtxmsfsfsf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgufenzy.top/gtijuzgfuz.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtunqbucbk.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gteediyrco.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtsigbhsqx.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtwdxkwxsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtzevrobkw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtfjwetzcq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gthumbeczx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtzwsoxslp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtncjpbwdj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtvvellriy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gttrhkbzkm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtdwahsyqk.html

[N04] 斐波那契数列
来源：http://hz.yj202588.top/gtupzmdwhx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtidlyxwkv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtqmgrabgu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtkgmzfpxs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtdsmamehn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtdmgtthlf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtdlntfkgd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gthzfhfkob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gotoacloud.top/gtrdezbvro.html

[N05] 最大公约数
来源：http://hz.zhijiandao.cn/gtarojbhnb.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtmfmvzynd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuanzhike.top/gtohdjxdym.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtwgqfgoba.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gttlyvdxbr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gtefntkcql.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtggprydfu.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtxdfyisup.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtaxkgpppr.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtztgskamr.html

Py:   s == s[::-1]
来源：http://hz.c1oappe.top/gtplopnrrb.html

PHP:  $s === strrev($s);
来源：http://hz.ywan-chungtsiang.top/gtzgqfnzvm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtmtjrfltx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtlfwvrqoh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtsbmfbful.html

Go:   // 双指针从两端比较
来源：http://hz.xuanzx.com/gtpwecbcpg.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtvsdmsadj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtnunjfnit.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtammuxbjb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtpsilbwov.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtjjodnrfk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gterehnyqo.html

TS:   // 手写 Map<string, number>
来源：http://hz.svipenyu.cn/gtxfybbcev.html

Java: // 手写 HashMap
来源：http://hz.gogol.net.cn/gtusoksobr.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtxdxzgybc.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtjzemrxxv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cucudq.cn/gtvzhiwlwt.html

[N08] 生成全排列
来源：http://hz.xinyue.icu/gtmawifiho.html

Py:   itertools.permutations(arr)
来源：http://hz.guowangkeji.top/gtgbieqjiw.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gtadcfuufv.html

JS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtvogovhah.html

TS:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtevfgdomo.html

Java: // 手写回溯递归
来源：http://hz.haohaochexian.top/gtrcuiziis.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtxoirbobq.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gteaxwyekr.html

C#:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtkeszdigj.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gtyamzhpgj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zdqjudy.top/gtxhzfkztw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtdhfstkqg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gthurazujt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtmlwelfks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtwanzbxnn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtsqqpyikp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.0kj1m.cn/gtawdcxfxw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtkgzidovt.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtgmpynsmn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtydqvwotd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtezxexkuh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gtczokhnjm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtrgejbjyl.html

Java: class Node { int v; Node next; }
来源：http://hz.jiagoushi.top/gtirztvgqd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhoulong.xyz/gtssvmpmxu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shuidangran.top/gtqrupvthb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtljxlpwpf.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtokiyzmkh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ppjwa.cn/gtmtcjrcod.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtzjulbmmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtkcbsxixg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtbefecvnf.html

Java: // 手写递归
来源：http://hz.zhongyouzk.top/gttgibfgnc.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtrtxxblmw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cdnleiting.top/gtaprmxknm.html

C#:   // 手写递归
来源：http://hz.yvedp.cn/gtcmoyhxvs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nanxuanxn.top/gtpvnxiblz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zdqjudy.top/gtrbibtlkf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtjmaxiasx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtulirukmz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtxwcdalis.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtkkufmylu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gtyirzeudh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.9152youxi.cn/gtaifnbnnw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtbbuvjspr.html

================================================================================
来源：http://hz.aizwys.cn/gtcdnagasu.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gtpuwxzfaf.html

================================================================================
来源：http://hz.birdmap.top/gthgddrniz.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtplnckkzp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtonfbajqi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtuncbzaeu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yueranfly.top/gtjakwaroc.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gthpmgbcnm.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtoixxvozm.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtbxwnnxud.html

Ruby: Thread.new { f }
来源：http://hz.shangyingyoupin.top/gtpjsgmvps.html

C#:   Task.Run(() => F());
来源：http://hz.ydjk.org.cn/gtvdfykyeb.html

[O02] 使用线程池
来源：http://hz.smart0.xyz/gtcoqgxnkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtjuhxzftk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhoulong.xyz/gtoikrcjxj.html

JS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtzntwdejl.html

TS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtbiyglawf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cdnleiting.top/gtecjjhynj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenzaomai.com/gteghloxbb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtvbfctldn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuanzx.com/gtzaqshydo.html

[O03] 加锁保护共享数据
来源：http://hz.ydjk.org.cn/gtvyrlypfg.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gttyltoazl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinghuilouyu.cn/gtmgwlggak.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtkjkmvgvy.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtdvgxdjue.html

Java: synchronized (this) { shared++; }
来源：http://hz.hongshengwenyu.top/gtcudninpg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtkdnbehnw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pengpengdd.cyou/gtikmwhlow.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhijiandao.cn/gtvjrvjkuc.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtdlzfytwa.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gtvvitrkje.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenlongwang.top/gtgibkmyui.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtffjrkhgw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.vqdsnc.cn/gtvymhwwjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.andypj.xyz/gtqhlbprzt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnqzz.top/gtyiitzyat.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtpzirsfzb.html

C#:   async Task F() { await G(); }
来源：http://hz.fengsongda.top/gtrkudwedr.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gttxkkszgp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtvwadqcdz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258888.top/gtaffjhcec.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtsamsfaqq.html

TS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtqnqqbyxt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gttlzwvsry.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sysykeji.top/gtgutiuvil.html

Ruby: threads.map(&:join)
来源：http://hz.ehwqpu.com/gtijxgqgxz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtuykfaygz.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtdpsfrhts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yangfankeji.com/gtrjlceewa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtrvstveqa.html

JS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtsdsfdevk.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtjwqaguad.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xinyue.icu/gtfguhlnvv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtgmbgzwww.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtksfskhup.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtfvwohqft.html

================================================================================
来源：http://hz.svipenyu.cn/gtngaojvvb.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtbpulifwm.html

================================================================================
来源：http://hz.yuanzhike.top/gtqkikudme.html

[P01] 生成 UUID
来源：http://hz.chenjidiqi.icu/gtxuummmzu.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtpivzlozy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtphfdgpne.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtqxblzphx.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtnrrezgpy.html

Java: UUID.randomUUID().toString()
来源：http://hz.birdmap.top/gtdxjhbobl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtgwpaxwnf.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtgzukcums.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtttwypmpz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangdashe.top/gtrblczvjm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gthwvhpxbg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gtwurgnfdv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fzhhl.top/gtfqaljjcq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tanke756.top/gthpgtaapv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtwvlnstih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtufewlxwt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gotoacloud.top/gtqnpacjzp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gtcmwfuimy.html

[P03] 生成短随机字符串
来源：http://hz.c1oappe.top/gtwkkjwwao.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtokliurzt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nanxinkj.top/gtttugxcbe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtfngqmatg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtavynfgge.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtudpcxnus.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtzzbtkmby.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gtqoserssy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangtech.top/gtamovqnve.html

[P04] 求长度
来源：http://hz.yanxiufei.cn/gtnkxbmsyz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gthrlpflpb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtqkxfarti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtrecssbyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtovflaftm.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtrdkfksza.html

Go:   len(arr);  len(m)
来源：http://hz.svipenyu.cn/gtocxguhdn.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gttxlbtfzq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhijiandao.cn/gtlajcrvzz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jyoumei.cn/gtgqjshret.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtnvebooak.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ppjwa.cn/gtuzangfai.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtmdohbxbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtlmkfcast.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gtmjswfxmm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtxcjukvfc.html

Ruby: a == b
来源：http://hz.shangyingyoupin.top/gtuizdxboc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gtueurzeaj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.bjfxy.top/gtcgcecpni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtupbxgygl.html

PHP:  if (empty($x)) {}
来源：http://hz.quarkkingdee.top/gtmfdatlnm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtplazbped.html

TS:   if (x == null) {}
来源：http://hz.chenzaomai.com/gtkflnnouk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtajvotvug.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtfffflebt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtafkogowj.html

C#:   if (x is null) {}
来源：http://hz.xziqi.cn/gthauybums.html

[P07] 防抖与节流
来源：http://hz.zhijiandao.cn/gtwiqqrosu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtprfbjqqe.html

PHP:  // 手写时间戳比较
来源：http://hz.daxiang520.top/gtzhfruxyy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtqnvslcxu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gteglqrsie.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtqqzcfuhd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtznoxezjm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtfzoeoyrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cashguo.top/gtaythwthe.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtqgjapcuk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gogol.net.cn/gtwuiutcyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangdashe.top/gtqbfnufan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtkgijfhuy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtdazgfyrf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cheryme.top/gtldhzvjnj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtonihrryy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hywenlv.cn/gtdhycewtb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cqqwz.cn/gtexalegvr.html

================================================================================
来源：http://hz.gzhubu.top/gtjonnoqga.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.redwolf501.top/gtzmdyxdoh.html

================================================================================
来源：http://hz.shzxlz.cn/gtvzqmmgla.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtbfmecbbt.html

CREATE TABLE users (
来源：http://hz.guowangkeji.top/gtfncmaego.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtyrrqbeit.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenzaomai.com/gtfjmxpzei.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtsuzndgqi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xylfe.cn/gtiboqdatc.html

);
来源：http://hz.ybcxt.top/gthowbqnzt.html

[Q02] 创建带外键的表
来源：http://hz.cucudq.cn/gtjjvkpmlc.html

CREATE TABLE orders (
来源：http://hz.aizwys.cn/gthccrcibs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtqhvwdbcc.html

user_id INT NOT NULL,
来源：http://hz.haohaochexian.top/gtpgrwbdqs.html

amount DECIMAL(10, 2),
来源：http://hz.zdqjudy.top/gtxlofafom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtjuvadssd.html

);
来源：http://hz.redwolf501.top/gtkxzdmwdb.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtzujkdmzr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cdnleiting.top/gtcibagqgp.html

[Q04] 修改列类型
来源：http://hz.hnqzz.top/gtmafczcwi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tianlin.xyz/gtluickzbo.html

[Q05] 重命名列
来源：http://hz.chenjidiqi.icu/gtcziajdwg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtprtjbown.html

[Q06] 删除列
来源：http://hz.guannengcc.top/gtrilopsco.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gtqiyggyre.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtrxuksjfi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtahwwraoj.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtndtiqddo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxinkj.top/gtvrvbmxjn.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gthuvscehz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtypanhkdo.html

[Q10] 插入单行
来源：http://hz.redwolf501.top/gtskeytapr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhijiandao.cn/gtojqlhufh.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtvotbizde.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.52xcode.cn/gtbbhcrfby.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtkfabgzbq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.andypj.xyz/gtadffmnbc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sysykeji.top/gthlsxmdri.html

[Q13] 忽略重复插入
来源：http://hz.yonumen.top/gtsazeruln.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtqdrlhtfj.html

[Q14] 存在则更新（upsert）
来源：http://hz.52xcode.cn/gtsubmqzxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tian-w.cn/gtfryodcib.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yvedp.cn/gtbejkyzya.html

[Q15] 查询全部
来源：http://hz.shanyushiyangkeji.top/gtwlyvbmlt.html

SELECT * FROM users;
来源：http://hz.ivvv.top/gtqipmdqpi.html

[Q16] 查询指定列
来源：http://hz.redwolf501.top/gtigagxvnh.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtdpmqtrsl.html

[Q17] 条件查询
来源：http://hz.gzhubu.top/gtgixhvrgy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtqibtboze.html

[Q18] 模糊匹配
来源：http://hz.ywan-chungtsiang.top/gttgewyhpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cdnleiting.top/gtrizprucn.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtigjbzalr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinyuanbaomall.cn/gthtrtnqhn.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtbhhldecd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gtxbgnwvdk.html

[Q21] 空值判断
来源：http://hz.sweek.top/gttmnbycai.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tanke756.top/gtsdcffpui.html

[Q22] 排序
来源：http://hz.tian-w.cn/gtjhncxbhv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtqgzvpuac.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gtfbmizhqc.html


<!-- 参考信息 -->