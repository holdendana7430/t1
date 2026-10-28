代发 wailian999

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtgsqvuzuf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtzefzvsla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gttkjddqqo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtjafvcpta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtitppsvvp.html

================================================================================
来源：http://hz.xylfe.cn/gtcavnhdem.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtidktfgll.html

================================================================================
来源：http://hz.wangdashe.top/gtcwtawiad.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gtpjnwbikq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gtmvwmeaii.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtejohabbs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtqittrtbq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtwazqckmd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtkjumrgko.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zycfv.cn/gtcuhjrgqj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gteciejyan.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xinyue.icu/gtlvnzfplt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtxkjfqzxu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtdvkyeplb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dianchejie.cn/gtyhossbtd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtovdazekd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtqfusuwqx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shangyingyoupin.top/gthchpzctz.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtdcmcgnua.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtunthmgon.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daxiang520.top/gthfowmain.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtgamdxoeu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtrqxqgiff.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtfudzzipa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtcizbshup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtumdfeevo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtahtnkhgf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gtadthcwhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtvmlhsztu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gttbllopog.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtmxeqnbyt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtuodilumj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gthbjkrkls.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtiladimdk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gteaqcpcmr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hfpthk.cn/gthowgsldy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtvekwfhtl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtcpgdkyfm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtcyhxdglg.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gttxyluukr.html

Py:   math.gcd(a, b)
来源：http://hz.xylfe.cn/gtiqogvdei.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtupfbppbr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtwmgfxado.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gteeugaeqc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtfahlqctn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtpqztnqun.html

Ruby: a.gcd(b)
来源：http://hz.tian-w.cn/gtbokamxdh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtbemkokxo.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtbopvnkhr.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtgsilgocs.html

PHP:  $s === strrev($s);
来源：http://hz.sweek.top/gtxqdfovkh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtdjaqiyvo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtgnubyxgh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtroostkse.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtutgumznw.html

Ruby: s == s.reverse
来源：http://hz.jqgufenzy.top/gtawavigpz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtzyzgzmdr.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gthrdvonav.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhongyouzk.top/gtwuivpcsh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtauydwrcc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtrnngkszb.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydzc1.top/gtfxmykbei.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtczyfgucl.html

Go:   // 手写 map[int]int
来源：http://hz.meibo888.top/gttvvzmwfj.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtofxwluyn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtesqbojym.html

[N08] 生成全排列
来源：http://hz.xylfe.cn/gtqlxjcmml.html

Py:   itertools.permutations(arr)
来源：http://hz.cheryme.top/gtttllmmcj.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtiidslsfu.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtxncmfyjh.html

TS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtrlhitjtd.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtgjxthnhx.html

Go:   // 手写回溯递归
来源：http://hz.yj202588.top/gtxkdmkszt.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxinkj.top/gtpsxwnsah.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gthmeafirl.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtbhkcteim.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gttetjmsso.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gzhubu.top/gtscztywyg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gttrpcuyja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtroxermpf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtyxgnffak.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gtbdehnaqi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gotoacloud.top/gtunlwhdca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtespfsnqp.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtlpiqjvbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.birdmap.top/gtlvestvwy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gterpubcjq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtqzsycicw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtgvgtdksj.html

Java: class Node { int v; Node next; }
来源：http://hz.yj202588.top/gtqhoyxmwl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtipcnrbgr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.316326.xyz/gtibbbaxtv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258888.top/gtjvfnquem.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtyzjqwkaa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtfqqvggiw.html

PHP:  // 手写递归函数
来源：http://hz.c1oappe.top/gtfqonlpig.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtqxtroeku.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtxovplbrd.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtxoujtgqn.html

Go:   // 手写递归
来源：http://hz.guannengcc.top/gtycxbpzpf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenlongwang.top/gtmnahvjuj.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtlsbqcpkw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtrvvpgedk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gttpodusvl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtkcfyyoxe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtxjkdgyta.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtknueisca.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtdqnarkox.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtksgcmdwe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtrnevsysz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtuufresso.html

================================================================================
来源：http://hz.shzxlz.cn/gthhmotfrw.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gthbmpxrdo.html

================================================================================
来源：http://hz.birdmap.top/gtuaafndgg.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtieqrwiyo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yangfankeji.com/gtqszaoxmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtftncwhfu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtpbgtmqyq.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtesrtsgiz.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangtech.top/gtklznsell.html

Go:   go f()
来源：http://hz.sysykeji.top/gtctnrzisi.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtdarhjzbd.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtqtxdosxa.html

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtbrnwibzm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtjimuwkzu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnxiangtu.top/gtbdvhxvzb.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtwgjfcxnm.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gthmnvvcqa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ppjwa.cn/gtncukfnbt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtulwuaama.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xziqi.cn/gtefirufaz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtowbobaxs.html

[O03] 加锁保护共享数据
来源：http://hz.sysykeji.top/gtuvuzwqev.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtriasnaud.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtphzhgktd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guowangkeji.top/gtrwkdovkg.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtxunmprik.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtjwlpjeod.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258.top/gtgpwcmaue.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gttdpmcyzv.html

C#:   lock (gate) { shared++; }
来源：http://hz.cheryme.top/gtrhnlytum.html

[O04] 定义异步函数并等待
来源：http://hz.gotoacloud.top/gtrlxcrenr.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gthgxbnywx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ywan-chungtsiang.top/gtcakvlfit.html

JS:   async function f() { await g(); }
来源：http://hz.ivvv.top/gtlcssrxas.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtbstebeds.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gogol.net.cn/gtizcwvcau.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gteloetcfc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.quarkkingdee.top/gtcxudwswq.html

C#:   async Task F() { await G(); }
来源：http://hz.pycfn.com/gtnmefyjlj.html

[O05] 并发执行并等待全部完成
来源：http://hz.cqqwz.cn/gtshcaawhq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yvedp.cn/gtatlvkmql.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtuobtuwvf.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtlmudkqjv.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtezbpalig.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtecaabbge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.c1oappe.top/gtjeviueai.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gtekkqwttb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.birdmap.top/gtumfmjioe.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtkwmskopj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtuvvewqmh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtsgdeplne.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtafvaleec.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtvgdlemba.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nwbrower.top/gtxlgdnyln.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtihuxtelq.html

Ruby: // fork 块
来源：http://hz.andypj.xyz/gtgmwxmcpa.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtfkjjahll.html

================================================================================
来源：http://hz.gzhubu.top/gttbuulbit.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtllcigwdt.html

================================================================================
来源：http://hz.jyoumei.cn/gtlvrntupp.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gteqkvkhkl.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtftoaexyf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gttplfgwgu.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtbotzfxjd.html

TS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtnsjifyuh.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinghuilouyu.cn/gtrawwosni.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtqjrqjxjq.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtxnstcmdd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtmsiodwdf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hammf.cn/gtdyzwtqym.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zdqjudy.top/gtwbvdcqwd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.bjfxy.top/gtszmnviok.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtdmysjzvo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cucudq.cn/gtetuqszgr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtbzqmujyv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtzlhbdxsl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.haohaochexian.top/gtnwprylgx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jianghu66.top/gtgpjtycjb.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gtiatzgvlk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.quarkkingdee.top/gtzgdsmavc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ybcxt.top/gtqpvksdzm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtgeqvrwnc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtvdwberih.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtohyrrnxl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuanzx.com/gtxvbmviqv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtqbdtqczp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtmrjgwdgo.html

[P04] 求长度
来源：http://hz.xziqi.cn/gtthxbgkqq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gtwdbkgqrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtgxhhqjjj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtaupviwmp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtuykptgbo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jyoumei.cn/gtthciexga.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtzvzvrlav.html

Ruby: x.length;  x.size
来源：http://hz.tianlin.xyz/gttvuifadh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gaohongyu789.top/gtdgjmzgwb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigfzy.top/gtdjwjhdrk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtzsccfaap.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.redwolf501.top/gtkgljnjab.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sysykeji.top/gtsmcwwqrv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtctilfxfw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtcfcqgfhq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtqfwlxofq.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtuvsrkhsi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtpidftyjq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtxtzpvtmc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.iojbl.cn/gtydbfsxgx.html

PHP:  if (empty($x)) {}
来源：http://hz.fzhhl.top/gtxyotayqw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gogol.net.cn/gthatmundh.html

TS:   if (x == null) {}
来源：http://hz.yj20258888.top/gtrivrbici.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gthfcdkmda.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtysjufpqz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtvoqhttaj.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtvhiprttf.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtleyuqtlm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guannengcc.top/gtybifdway.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtqrbagjdd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtqorxvhwh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtzfluisit.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtbxthawxf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ybcxt.top/gtdfklgydf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cqqwz.cn/gtmbwlkgyf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.pengpengdd.cyou/gtfuffpfmn.html

[P08] 处理浮点精度问题
来源：http://hz.guowangkeji.top/gtvwhntafu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.gotoacloud.top/gtndbjxxiq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhongyouzk.top/gtqbculkha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtqxpvagcr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.birdmap.top/gtowsqqxxl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gtqzeumqig.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhiwuduotai.top/gthxshwnee.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sweek.top/gtbsnnxnhu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtulapshwe.html

================================================================================
来源：http://hz.dashuyun.cn/gtjttxrmku.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gzhubu.top/gtfvqhfgly.html

================================================================================
来源：http://hz.cqqwz.cn/gtmpiuogmk.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtuuiwpbki.html

CREATE TABLE users (
来源：http://hz.c1oappe.top/gtdplrqgbo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gthecfezqt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guowangkeji.top/gtnfjdsykb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tianlin.xyz/gtshxytfwn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.wangdashe.top/gtmygvyznf.html

);
来源：http://hz.xziqi.cn/gtteomqsyu.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gttjllaiad.html

CREATE TABLE orders (
来源：http://hz.yonumen.top/gtjgnwworb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtvjybgeyt.html

user_id INT NOT NULL,
来源：http://hz.cashguo.top/gtfakvuezw.html

amount DECIMAL(10, 2),
来源：http://hz.yj202588.top/gtvzahvawp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtzjmcrjwn.html

);
来源：http://hz.shangyingyoupin.top/gtswbiqfdr.html

[Q03] 增加列
来源：http://hz.zhoulong.xyz/gtxtqthhbz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yonumen.top/gtszioatsz.html

[Q04] 修改列类型
来源：http://hz.jqgfzy.top/gtcwythmfn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenzaomai.com/gtrtavijmp.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtktpkglio.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.meibo888.top/gtwaburlnj.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gtytcxidpo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.iojbl.cn/gtdutubldh.html

[Q07] 删除表
来源：http://hz.mhx1999.top/gtrqggfjui.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtxlaaakpx.html

[Q08] 创建普通索引
来源：http://hz.kuanghao11.cn/gtzttwxkif.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtyvevnvuk.html

[Q09] 创建唯一索引
来源：http://hz.quarkkingdee.top/gtcphlmzgo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtqiotadpq.html

[Q10] 插入单行
来源：http://hz.yj202588.top/gtmigxmtrf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtqnqlhyfr.html

[Q11] 一次插入多行
来源：http://hz.hnqzz.top/gtrgpiuxsf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hfpthk.cn/gtcaglkmmf.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gthhsjwdlo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtejjhfqdp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.snrcjt.cn/gtcvkcndgj.html

[Q13] 忽略重复插入
来源：http://hz.cashguo.top/gtbevtzycb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gtswvwrlaw.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenjidiqi.icu/gtbbunsesd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtyiiwycta.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gteolbhujr.html

[Q15] 查询全部
来源：http://hz.snrcjt.cn/gttdbsbfwj.html

SELECT * FROM users;
来源：http://hz.52xcode.cn/gtmhimgrts.html

[Q16] 查询指定列
来源：http://hz.ydzc1.top/gtfwgwkqok.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtajzuiyqz.html

[Q17] 条件查询
来源：http://hz.shangyingyoupin.top/gtpjfyyfzh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtyggniduy.html

[Q18] 模糊匹配
来源：http://hz.xuanzx.com/gtisbdoybu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.9152youxi.cn/gtfgipueur.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtedlcymnu.html


<!-- 参考信息 -->