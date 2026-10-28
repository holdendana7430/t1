代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtjtecjtzt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtmousxjvn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gthnwdvzhb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtbfyelmmk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtiafhzyja.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtzqymqkhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gtmdhwmvrr.html

Go:   slices.Sort(arr)
来源：http://hz.jianghu66.top/gtsifxfhfn.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtzemqbjxt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtogmicqyi.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtjmkivtic.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxuanxn.top/gtdhaajhsu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gthocbunzv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtdypfmkte.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtnmuklgdb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuetiantiany.cn/gtvdcrjmtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtajvgfswp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtmtfiiseu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtryhkqpkx.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtfnjsppuc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtyypgbnak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fengsongda.top/gtebkeospu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtwvgfiodv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtjhnbylun.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtgivlojol.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtmdvffskp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtwvyxapuy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtkmtjggih.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtnwchwofv.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gteyxatebj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtnvjufpkw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtexarstxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtnjvsyktx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtygdllhxc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj202588.top/gtpjmtrdmp.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtfrxmnucr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtczytntmn.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtgfezeyed.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtjspukwgq.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtcryfnfqx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtunndciwz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtfurtgkgx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtwdreggya.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtqsiiqqkp.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtpojrubqe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gttwvphpeg.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gtrqadooha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtnrfxfgor.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtqxlldfsr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtcodsenvf.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtzlecgsyq.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtmigkbksn.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtluiwblkd.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtdtizcqfl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hongshengwenyu.top/gtlwoksblv.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtlmjapxtx.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gtsxfbrams.html

PHP:  // 手写递归交换
来源：http://hz.nanxinkj.top/gtplewzsmk.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtrahszdcr.html

TS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gttanieerh.html

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtsushbgyg.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtjjitwawu.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gtyrlwlbzl.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtotfcjpbl.html

[N09] 栈与队列
来源：http://hz.nanxuanxn.top/gtfiotaapx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtmopbieai.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gtpzpdllsy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cdnleiting.top/gtmtsbbhig.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinghuilouyu.cn/gtlogpavac.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangtech.top/gtnxonwqee.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gttfsknixx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtvrrglpjo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtipcdnqsf.html

[N10] 链表节点定义
来源：http://hz.nanxinkj.top/gtcnvtikio.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtpicsgamk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ydjk.org.cn/gthuyqprnb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.kuanghao11.cn/gtoensyayx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yvedp.cn/gtphacknly.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtgsdiwhmt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtxkgvbyfm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtekjltddi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtqxxwiymy.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gthqxbuoio.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtjysbgtrt.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtmtaiavbz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtidxnjpaw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtngtpsvqz.html

Java: // 手写递归
来源：http://hz.wangshuangyany.cn/gtpvbayziy.html

Go:   // 手写递归
来源：http://hz.xuanzx.com/gtwzngobkj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.iojbl.cn/gtfvehtzxk.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtqyadpxjh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtrjqyggdt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gtrbjlchpy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtywhvxoya.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtylfuwzum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtgozbpxei.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtvgvzxgzu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinyuanbaomall.cn/gtbiehwkhi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtbknzdoar.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtdrpxmffr.html

================================================================================
来源：http://hz.c1oappe.top/gtscjnlftd.html

O. 并发与异步
来源：http://hz.hywenlv.cn/gtdgrmdcgp.html

================================================================================
来源：http://hz.yueranfly.top/gtdqsqirpx.html

[O01] 启动一个线程
来源：http://hz.fzhhl.top/gtrevzfyff.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhongyouzk.top/gtinztctnh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sysykeji.top/gtounlrqwh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtenagvaua.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gthvjmcfcq.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtiuugnnrr.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtmaybtblg.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gthudrmlhq.html

C#:   Task.Run(() => F());
来源：http://hz.xingfuxueyuan.xyz/gtypmichnp.html

[O02] 使用线程池
来源：http://hz.52xcode.cn/gtauqvwfne.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shanyushiyangtech.top/gtpjlvwslg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtovsuwstc.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtndigxdtk.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtvvuodtfa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtdppbuoaf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtheycosye.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtpggpgpow.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tian-w.cn/gtcpqwfatu.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtokdkeysj.html

Py:   with lock: shared += 1
来源：http://hz.cucudq.cn/gtijfjsfxj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shangyingyoupin.top/gtflokxqlj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtljvsqbhw.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtxradbhul.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhongyouzk.top/gtxrzwmymx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtzmshrmhq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtiolxgpzj.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gtgwefqaog.html

[O04] 定义异步函数并等待
来源：http://hz.gogol.net.cn/gtyulbibzt.html

Py:   async def f():⏎    await g()
来源：http://hz.cucudq.cn/gttcsheydf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gtstpkxwos.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gthcmpjkou.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtzlyznbdp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.feifeiyinyue.top/gttpjmtbqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj202588.top/gtyasyispz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sysykeji.top/gtedajteli.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtctpbwcio.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gteuuuxfnh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtppomtfgq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtjusiehgl.html

JS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtlhdwxdbm.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtjzqundzr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gthcjgqnte.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.andypj.xyz/gtlncbhnns.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtvejimzjx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gtpwnxtbju.html

[O06] 使用进程池
来源：http://hz.jinqigfzy.top/gtgcrtroof.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtmpomelam.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tianlin.xyz/gtxirvkgnq.html

JS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtpxguyhjz.html

TS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gttqvndszm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinghuilouyu.cn/gtttkucvyh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtjamhemha.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtfeneahoa.html

C#:   Parallel.For
来源：http://hz.9152youxi.cn/gtuytbvttq.html

================================================================================
来源：http://hz.cdnleiting.top/gtbigfhzdj.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtwpfqcavc.html

================================================================================
来源：http://hz.tian-w.cn/gtcmoeogxm.html

[P01] 生成 UUID
来源：http://hz.gotoacloud.top/gtejiupgav.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258888.top/gtgxmabsja.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ehwqpu.com/gtjszzlhgo.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtiyqejxrf.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtxjzhkbsn.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtjecruwxa.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtdfaghuon.html

Ruby: SecureRandom.uuid
来源：http://hz.hammf.cn/gtjaankfkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hysaishi.cn/gtsjynqgld.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cdnleiting.top/gtixbitzeb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtetozawav.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hfpthk.cn/gtacurwwvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tianlin.xyz/gttbcvxsbe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxuanxn.top/gtsodbqqmm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtnmfplnyb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtqqwujdfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ybcxt.top/gtoasjzoub.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtjpsdvpxs.html

[P03] 生成短随机字符串
来源：http://hz.nanxuanxn.top/gtxsbuengf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtilnjgzfr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangdashe.top/gtfzmwniky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gthtilfkgv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtrhareyap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtyeaxqtix.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hammf.cn/gtinwcsrti.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtsqtaihdl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ywan-chungtsiang.top/gterqpcqlc.html

[P04] 求长度
来源：http://hz.meibo888.top/gtcsowymaz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtowcjryfu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtnfnpmjmn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gttuuwcund.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtnnegrbsn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jiagoushi.top/gtmbjjhlqs.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtcubbtnvc.html

Ruby: x.length;  x.size
来源：http://hz.snrcjt.cn/gteymuhsuc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuanzhike.top/gtxfwrdokh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.316326.xyz/gtzrcepxyr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jiagoushi.top/gtodhmuydb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ydzc1.top/gtzepfrvxo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.bjfxy.top/gtogbkogpd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nwbrower.top/gttjyeruue.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtlrrcrlze.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj20258888.top/gtqpjbpszz.html

Ruby: a == b
来源：http://hz.nanxinkj.top/gttcnqjikb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtturwevyq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtctzctwti.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.wangshuangyany.cn/gtgqtiifhu.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtlqsvzzmw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtfmfhqwrj.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtlzklgmux.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj20258.top/gtblcsjwiy.html

Go:   if x == nil {}
来源：http://hz.jinqigfzy.top/gtmepshiks.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gthrblsvzi.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtdooukjju.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtufollyhx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtrtbnrwfn.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gtreiqnmfh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtfraamfmz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtuqjjzmfu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtoccyauhm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtxiexeftl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtslqwcuyk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.haohaochexian.top/gttfyeghit.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtuebbvhyf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.cdnleiting.top/gtcwoyauno.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtjowpumza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtffdnuaal.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxuanxn.top/gtjkmeicko.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hysaishi.cn/gtjsnswwgh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gttmsctmzw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtpcgnyjku.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daria6918.cn/gtdzbjwvxx.html

================================================================================
来源：http://hz.daria6918.cn/gtvybnbicp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yongpay.top/gtgcemmijs.html

================================================================================
来源：http://hz.ybcxt.top/gtfzmzoval.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtqzhedziw.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtieasmtvy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtjoxanyxl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gthnmzcvlg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cqqwz.cn/gtdkprznxo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.9152youxi.cn/gterevszid.html

);
来源：http://hz.jiagoushi.top/gtlwemvvlp.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtypeqtqbu.html

CREATE TABLE orders (
来源：http://hz.shangyingyoupin.top/gtrvxhgmta.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ivvv.top/gtgswlslls.html

user_id INT NOT NULL,
来源：http://hz.haohaochexian.top/gtpbsgodgb.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gticmmouso.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtcwzestvv.html

);
来源：http://hz.jlsjyb.cn/gtcmtipbvx.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gthxxudnnl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuxming.cn/gtatjmarjo.html

[Q04] 修改列类型
来源：http://hz.jiagoushi.top/gtmodawrqt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daria6918.cn/gtwmiajyfv.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtlrwywopr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtmmdmmdjr.html

[Q06] 删除列
来源：http://hz.quarkkingdee.top/gtimdcueju.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtkgvfpmap.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtryxjxygr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.redwolf501.top/gtfmrmcoqh.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtnnzejlfl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ehwqpu.com/gtfmlnebta.html

[Q09] 创建唯一索引
来源：http://hz.jinghuilouyu.cn/gtgzjiqtmz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sysykeji.top/gtmfwqffdz.html

[Q10] 插入单行
来源：http://hz.0kj1m.cn/gtbbcbveld.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtycptpzka.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtwyplpydt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtdfafvdfk.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtajimhafw.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aizwys.cn/gtqmxjgrlv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sufxvd.cn/gtzhldtatb.html

[Q13] 忽略重复插入
来源：http://hz.zhengqikj.top/gtaxazxewb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtwethnpih.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtjotsgpgf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangtech.top/gtcawjlkak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gzhubu.top/gtsluzzeyx.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtiobguode.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gtyjgerfkl.html

[Q16] 查询指定列
来源：http://hz.fengsongda.top/gtjobwxqvo.html

SELECT id, name FROM users;
来源：http://hz.zhijiandao.cn/gtktaxdwig.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtvwkeqmbl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhixingplan.top/gtegkzzhwh.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtnflxwjyx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gthepojqlb.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtsxhagrky.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgfzy.top/gtzkfmtlkn.html

[Q20] IN 列表
来源：http://hz.hfpthk.cn/gtyzfopcnh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jyoumei.cn/gtsfwlqfza.html

[Q21] 空值判断
来源：http://hz.ehwqpu.com/gtnjjbqskk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtfhgeokct.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtwvlxpnxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ywan-chungtsiang.top/gtbhkjhdpz.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtgjawjpai.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.feifeiyinyue.top/gttrgzhoiw.html

[Q24] 去重
来源：http://hz.guannengcc.top/gtgbdvcaky.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhiwuduotai.top/gttaqdjjpo.html

[Q25] 只取前 N 条
来源：http://hz.zhaomingkeji.xyz/gtiybjbwnd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtfynmxhdt.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtiaxlnhfj.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangtech.top/gtygmovcyv.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gtinouejwv.html


<!-- 参考信息 -->