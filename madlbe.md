代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtmtilmfxm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtgfoivssn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtcwejayuq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtdrghlscr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtmmmddwvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtipiudayu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gturytcoaf.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gturbgpbfp.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtfkgrmfib.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtoaqghiys.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtmkvhsuyf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtxjladrxq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtbotorqrp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtvmgudkqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtxypaurol.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtskveqfsg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sweek.top/gtmreneqmf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtbnvilgpp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtcucnmmkr.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtzlbkpfiw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtxxubretf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gtgkyhxpow.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtgmkhnsyl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtvheeiboh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yongpay.top/gtnokeynzn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtxjmwsmkz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtoigcjdtg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cheryme.top/gtwmbxgaks.html

[N05] 最大公约数
来源：http://hz.ivvv.top/gtychtrnrx.html

Py:   math.gcd(a, b)
来源：http://hz.kuanghao11.cn/gtxgyecqed.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtapjqtkft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtdnledshx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtpmnkfjgd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtkezvurzi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhiwuduotai.top/gtvtkltyac.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtewncsxrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtbslxigxz.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtqwedvjsp.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gthscksiyv.html

PHP:  $s === strrev($s);
来源：http://hz.yangfankeji.com/gtgxqyqhzd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtuzysiyvx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtqeawoohk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jianghu66.top/gtzcrkryfm.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtgfdmuadj.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtbcoqdfkd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtuggbleuj.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gtpncsdjkt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.vqdsnc.cn/gtaumsijpg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtbskiqhns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtzmiqvfyx.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtefiocyuh.html

Java: // 手写 HashMap
来源：http://hz.nwbrower.top/gtlztroozs.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gtkrczazeu.html

Ruby: // 手写 Hash
来源：http://hz.chenzaomai.com/gtuacafrga.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtmpekduzr.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gtlzasslgf.html

Py:   itertools.permutations(arr)
来源：http://hz.chenjidiqi.icu/gtojljrxoe.html

PHP:  // 手写递归交换
来源：http://hz.jinyuanbaomall.cn/gtvnplwach.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtatcbdmmv.html

TS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gthqmyixpq.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gtewisvvah.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtybndccek.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtintvdbdo.html

C#:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtikuxzjwy.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtoeqkckcz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhoulong.xyz/gthyjhjyqq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shangyingyoupin.top/gtoxxsuhvp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtqqolwrxn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtgmkaqxbo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtamvuougm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xuetiantiany.cn/gtgaekfkoy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtxhbsrlte.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtkfbhjcsz.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gtejsbbzju.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cucudq.cn/gtmgrpukip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtnghciykm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtnfjqofsz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtbthudcei.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtmikyyypj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenzaomai.com/gtachhmpck.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtdltguhsn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtqwmhypqo.html

[N11] 二叉树中序遍历
来源：http://hz.cqqwz.cn/gttuiiputy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtcsqixnps.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtvewttdic.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtsnkzotpa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtcfwsxsyc.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtynnurhii.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtqnufptpz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtctrooulj.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtgyuhcren.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtuczxpnoq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.feifeiyinyue.top/gtupyvrkne.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.smart0.xyz/gtozzkddpq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtxlfufvwk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtqpoisprd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtafekgeoy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtllszotbi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gtyyxmprpi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtlidltkhi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyugnewti.html

O. 并发与异步
来源：http://hz.hfpthk.cn/gtptcpgabz.html

================================================================================
来源：http://hz.ehwqpu.com/gtyyozaqpb.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtcwwtjcjm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtrliaqeoi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtggdonzrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hywenlv.cn/gtbwnxvqfs.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gteixuvbeg.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangtech.top/gtynkdyxps.html

Go:   go f()
来源：http://hz.yj20258888.top/gtakzqqajc.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtiwvwelsz.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gthpqsmbem.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtejtggseo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtgxdmxtyw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sufxvd.cn/gtspndrpcm.html

JS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gthvkgqbab.html

TS:   // worker_threads 线程池
来源：http://hz.svipenyu.cn/gthektvgwp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtjrqnvvee.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtmpgcfpsq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuxming.cn/gthsmbncsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gtxxhlwdhg.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gtneuumkcf.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtytjlfrnc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.iojbl.cn/gtvycxhbpq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtserkxpwt.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtiovzgyez.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhixingplan.top/gtkdftoumr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gotoacloud.top/gtgmzvhbgy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtasijaoji.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtcfojxmkc.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtaqbmhgkh.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtedrujcyr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtmiccdasu.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtlnfidjzo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtefwwkqxv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xziqi.cn/gtaupnvnrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtrroxdrkp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtofavcxkr.html

C#:   async Task F() { await G(); }
来源：http://hz.yueranfly.top/gtyilmwivx.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gttqrkgpke.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gtjrpnvrzv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yongpay.top/gtgozbafyf.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtdbozcdqy.html

TS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtbghwznry.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gtzlxffhtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gtjzvozbvc.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtbrwpvdmq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtkhvjbgqi.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtndahorbk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtkuhknfan.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yueranfly.top/gtuncivxbh.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtsbceeowt.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gttgjlucjj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sxryk.cn/gtktwolvru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.52xcode.cn/gtolcqcnja.html

Ruby: // fork 块
来源：http://hz.zhengqikj.top/gtynqrnztx.html

C#:   Parallel.For
来源：http://hz.yvedp.cn/gtregamgkp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtznibpjmk.html

P. 常用工具函数
来源：http://hz.hnxiangtu.top/gtetcqqswc.html

================================================================================
来源：http://hz.c1oappe.top/gtddtjexgj.html

[P01] 生成 UUID
来源：http://hz.redwolf501.top/gtbudkivhg.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtqbiufukd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yuxming.cn/gtcaptyqsa.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtydtusttd.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtbvrekats.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinyuanbaomall.cn/gtpwuwmyrj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnxiangtu.top/gtuzqwtztn.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258888.top/gtspxiphsc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gtqyeqfddv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.redwolf501.top/gtyecepfru.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtkhyernij.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtxyasezhl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zycfv.cn/gtofhaskpp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gttotsrqxi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenzaomai.com/gtztszxyaa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtjardusks.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtmvfbtrpe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.9152youxi.cn/gtvhaxwyuq.html

[P03] 生成短随机字符串
来源：http://hz.nanxuanxn.top/gtkglmxach.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nwbrower.top/gtuqgsfhiw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtqsbhpcut.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtcaevmqct.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtzbyezrlr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtcgnpttop.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ppjwa.cn/gtffkfiuca.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dianchejie.cn/gtbxjpacdw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxuanxn.top/gtbbsqndjj.html

[P04] 求长度
来源：http://hz.jinghuilouyu.cn/gtcmzkzxzr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtsxyewczb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtoaktmmtx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtnkrvnkos.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxuanxn.top/gtvgxobohs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhaomingkeji.xyz/gtwljkukug.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtdrmkpesa.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtnooogjqz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yueranfly.top/gtzucghzbl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gttzibqrhw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gthkouunnq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xingfuxueyuan.xyz/gtyxyfyqzs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtindnblyi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtlypfxfvk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gthuspqzou.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinyuanbaomall.cn/gtxmykttfo.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtbhwhkivw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhijiandao.cn/gtjzyfnwgp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtfejwiizh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtuusbvrsk.html

PHP:  if (empty($x)) {}
来源：http://hz.yj202588.top/gtxopppmld.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtfehveetz.html

TS:   if (x == null) {}
来源：http://hz.smart0.xyz/gtdoevdosw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtlojfirlo.html

Go:   if x == nil {}
来源：http://hz.ywan-chungtsiang.top/gtqnlnepwc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtvsqxmadc.html

C#:   if (x is null) {}
来源：http://hz.52xcode.cn/gtjjatfqzf.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gtwgxeizbs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zdqjudy.top/gtyzorjfos.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtndaczavv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtrcebuzqr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtiiunqicz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtlqcsvltu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shangyingyoupin.top/gtbdqiunxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtjkmxisbx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.bjfxy.top/gttqookqwg.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gtzlwguzcy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gthrjvxlvo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258888.top/gttzoyctyc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ydzc1.top/gtvpgqenbk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtrzbhogsw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.vqdsnc.cn/gtmlhafdrx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ydjk.org.cn/gtcqtrzezr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtrwsniotw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yongpay.top/gthgnngiek.html

================================================================================
来源：http://hz.gaohongyu789.top/gtirnrvncb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gtjegpntme.html

================================================================================
来源：http://hz.havefunace.top/gtrxgbugro.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtmpzvvdqw.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gttcngccvl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xinyue.icu/gtguuakylh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.9152youxi.cn/gtcdfghrxd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shanyushiyangtech.top/gtrwtfgttw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gttfdnlvqh.html

);
来源：http://hz.wangdashe.top/gtnzpptmyu.html

[Q02] 创建带外键的表
来源：http://hz.chenjidiqi.icu/gtejngzedu.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtsgojwfcw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtzjqzwjnp.html

user_id INT NOT NULL,
来源：http://hz.hysaishi.cn/gtxulkmdxy.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gthgtouojn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtchdnilkv.html

);
来源：http://hz.havefunace.top/gtzqfywcqm.html

[Q03] 增加列
来源：http://hz.jqgufenzy.top/gtafbldhxn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cashguo.top/gtktzvrkfm.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtoxdwywab.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pycfn.com/gtsyvbulgq.html

[Q05] 重命名列
来源：http://hz.haohaochexian.top/gtmcqocygz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yangfankeji.com/gtghphkcaf.html

[Q06] 删除列
来源：http://hz.jinyuanbaomall.cn/gtfxbqesce.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shuidangran.top/gtaqtqumzq.html

[Q07] 删除表
来源：http://hz.jlsjyb.cn/gtbkkrascn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.fengsongda.top/gtsecuqljq.html

[Q08] 创建普通索引
来源：http://hz.guowangkeji.top/gtssjlyuis.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.316326.xyz/gthuchtvyg.html

[Q09] 创建唯一索引
来源：http://hz.snrcjt.cn/gtlfossqcl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gthvcdgmkw.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtgwpgxfkr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gtzebeatlk.html

[Q11] 一次插入多行
来源：http://hz.cqqwz.cn/gtmbihctzd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ppjwa.cn/gtnyiwyjwe.html

[Q12] 插入后取自增 ID
来源：http://hz.cqqwz.cn/gteescvddn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hysaishi.cn/gtfvqptigz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydjk.org.cn/gtunorhsmc.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtyteayqet.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtnnmoenuf.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gtzzvnoncs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dashuyun.cn/gtjeqdhfga.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.fengsongda.top/gtoqoenybz.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gtsvozyvmh.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gteyvciowj.html

[Q16] 查询指定列
来源：http://hz.zhixingplan.top/gtgeuxtqql.html

SELECT id, name FROM users;
来源：http://hz.xuetiantiany.cn/gtmlzaqwxi.html

[Q17] 条件查询
来源：http://hz.svipenyu.cn/gtuebmksyu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gtpmddmjcy.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtgdhhczyt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.9152youxi.cn/gticogjamd.html

[Q19] 范围查询
来源：http://hz.yuanzhike.top/gtfqnftrpz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtvdlljcmj.html

[Q20] IN 列表
来源：http://hz.xingfuxueyuan.xyz/gtnujugdqn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hfpthk.cn/gtyotadcmm.html

[Q21] 空值判断
来源：http://hz.52xcode.cn/gttuikqhqn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.haohaochexian.top/gtydbarotq.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtwhlhkqit.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cheryme.top/gtsdmtyqdo.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtvchswzbv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtmghkcrrt.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtlbxcsldr.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtimwaplog.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtriesbsrb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jyoumei.cn/gtxaewugza.html

[Q26] 计数
来源：http://hz.ivvv.top/gtfbwzgewt.html

SELECT COUNT(*) FROM users;
来源：http://hz.cdnleiting.top/gtzehhnjpv.html

[Q27] 条件计数
来源：http://hz.ywan-chungtsiang.top/gtatjnihwv.html


<!-- 参考信息 -->