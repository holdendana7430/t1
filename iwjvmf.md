代发 wailian999

Ruby: arr.sort
来源：http://hz.havefunace.top/gttkszgfpy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtmobpvffk.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtufbihbhm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cashguo.top/gtzuppwhfh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gthyuzyazs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtucsbuejx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtnhxkzpiy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sweek.top/gtpenjcfvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtergivktq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jlsjyb.cn/gtecjffkxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenzaomai.com/gtmizzfxyh.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtolkxywug.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtjqxcguaa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtvkynaoei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtdokxivky.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtjgnjujvv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtvxypuemf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtghybjodi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtvmheuszr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtgoqxbyiv.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtqkfyrhnw.html

Py:   math.gcd(a, b)
来源：http://hz.wangshuangyany.cn/gtrzmgpcck.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtkxfvgtgm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtcvaopyue.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtuvanpycz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cucudq.cn/gtsydrcfno.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258.top/gtlvjtpqnh.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtdcknniyo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnxiangtu.top/gtpyojiwdy.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtbulhvjqi.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtorndqoam.html

PHP:  $s === strrev($s);
来源：http://hz.fengsongda.top/gtlxhoyzsb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtjnoqlehx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtxwioocqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtrggyqqui.html

Go:   // 双指针从两端比较
来源：http://hz.yangfankeji.com/gtigdotopp.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gtgxxffnsd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtyrmamrsl.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtlrfsdyqt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigufen.top/gtxldclkty.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jqgufenzy.top/gtgnobpusq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtpbdmihos.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gtofyziqxo.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtgzypkpbn.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtsubmzpzj.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtzotnrwxk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gtsoyukqlf.html

[N08] 生成全排列
来源：http://hz.ehwqpu.com/gtsbzjumzx.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxuanxn.top/gtaexmnhzi.html

PHP:  // 手写递归交换
来源：http://hz.jlsjyb.cn/gtwwiduhjs.html

JS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtqauslzzs.html

TS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtebegiiml.html

Java: // 手写回溯递归
来源：http://hz.yuxming.cn/gthlssgloy.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtsfwnqauq.html

Ruby: arr.permutation.to_a
来源：http://hz.ywan-chungtsiang.top/gtxtnhsfqc.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtvygkrvod.html

[N09] 栈与队列
来源：http://hz.hnqzz.top/gtiecqkapc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gotoacloud.top/gtixghccmr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtskxzcspg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtcxkxtiqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtnqsxzntr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtasdambim.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gtxjlscbcn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtnpksmbpl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gtewjhxqbu.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gtpnklwupl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtsqhlauuk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ybcxt.top/gtotvqjyki.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.pycfn.com/gtmoqgcnlk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinghuilouyu.cn/gttcjvwfnx.html

Java: class Node { int v; Node next; }
来源：http://hz.zycfv.cn/gtwcnsxclg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtcysicypv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhoulong.xyz/gtfygylkmr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtfrdatmar.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtzpmidpos.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gtqpmsqivi.html

PHP:  // 手写递归函数
来源：http://hz.ywan-chungtsiang.top/gthinjphrc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtmawuwgda.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtvyukavfa.html

Java: // 手写递归
来源：http://hz.chenzaomai.com/gtkezpkczv.html

Go:   // 手写递归
来源：http://hz.sufxvd.cn/gtqwfbfesj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtdrzkelen.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gthtnyctby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgufenzy.top/gtbewkqogw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtbciomstj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhongyouzk.top/gtyhwkahrc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtazmvpkxv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtxnsblxrm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gttkywcnch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.sysykeji.top/gttizbvybv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yongpay.top/gtxjvreaog.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtyzacinug.html

================================================================================
来源：http://hz.yj20258888.top/gtfvywrdas.html

O. 并发与异步
来源：http://hz.yj20258888.top/gtzhqghtlb.html

================================================================================
来源：http://hz.jianghu66.top/gtmsfjlizi.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtejvjtedu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zdqjudy.top/gtmyzpxsux.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fzhhl.top/gtiiukiiea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sxryk.cn/gtyicxivcf.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtxusbkgxy.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtkmddkzpn.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtfoyitnxl.html

Ruby: Thread.new { f }
来源：http://hz.yongpay.top/gtuxoayspc.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtxlpehmkd.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtevejezzf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtdzcxflxb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258888.top/gtxzvbulsr.html

JS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtzevwiisj.html

TS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtbnssqran.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtrtqfolch.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtsrvduyia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yueranfly.top/gtbbywcyab.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangshuangyany.cn/gtfmiyrhiu.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtgntjpuul.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtnawceelx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.chenlongwang.top/gtfsmffsph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gtpuzxadll.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtcboxagia.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtatijbokr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.guannengcc.top/gtfezfuybo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gzhubu.top/gttpxjidvb.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtgaogohim.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtutvgenvp.html

Py:   async def f():⏎    await g()
来源：http://hz.ydjk.org.cn/gtvrikbhyn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangkeji.top/gtyzitixjw.html

JS:   async function f() { await g(); }
来源：http://hz.redwolf501.top/gthkumchqh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtycotzzbm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.meibo888.top/gtjgpxekof.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtimbqpfvm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtzpiawfmf.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtalgkzkcy.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtskzcwbll.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtuerzmrhi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.bjfxy.top/gthtszuadq.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtqxfoxvzh.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtvcazqpts.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinghuilouyu.cn/gtiuzlrzfr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cqqwz.cn/gtttarxeis.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gthyyjezbv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hysaishi.cn/gtnggamqar.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gttidpdsky.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gotoacloud.top/gtgqbpxuac.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.svipenyu.cn/gtuwtwstxp.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtfszzidaz.html

TS:   // child_process / cluster 模块
来源：http://hz.yj202588.top/gthailwoop.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gttwcdfpcx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sxryk.cn/gtijrqzzcb.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtygmedjpg.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gtvcjxcxmg.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyqifhjaj.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtxdbcwuyg.html

================================================================================
来源：http://hz.52xcode.cn/gtdwruxmdd.html

[P01] 生成 UUID
来源：http://hz.ivvv.top/gtzqikwodt.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtsilucqcg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gtfuxxtrjg.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtvqnuhjqx.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtykxmxyst.html

Java: UUID.randomUUID().toString()
来源：http://hz.redwolf501.top/gtznqwpxus.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gttcwpqmym.html

Ruby: SecureRandom.uuid
来源：http://hz.yanxiufei.cn/gtyvklxwfi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtqpnlmjum.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtejedpmrs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtznwhnhap.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daria6918.cn/gtktjervax.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtcrbfcmew.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtpkyjhpaw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ydzc1.top/gtnamzmlcz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtfbnglwgo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.snrcjt.cn/gtwmnebyjt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuanzx.com/gtaxkkeykd.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gthkpqtphs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtiizbwufb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtjhbtvkye.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtiquzamdf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gteocncedb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.daxiang520.top/gtqqqgcxde.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtlvnathqf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtlzgdwhad.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuetiantiany.cn/gtcngtwcwz.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtduxfjbvv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangshuangyany.cn/gtsygqqach.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtyytfzuwh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtclzrekiv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtezoyosdn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxuanxn.top/gtgvngqcrc.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtfwqybylp.html

Ruby: x.length;  x.size
来源：http://hz.jinyuanbaomall.cn/gthjdqrtcz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tianlin.xyz/gtcouvtqtm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtfgitckor.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gtwmamdzjn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gtxqbkelpm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtxzwjiuoj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtumjtrdqj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gthzussdbu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtbfyuvjug.html

Ruby: a == b
来源：http://hz.jyoumei.cn/gtvyryrgsf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtvvbcyllq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cashguo.top/gtunaxpbxj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.havefunace.top/gturhaegxi.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtoghdvnzs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenlongwang.top/gtikzmdidk.html

TS:   if (x == null) {}
来源：http://hz.guowangkeji.top/gtbztptiqq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tian-w.cn/gtxbqesodr.html

Go:   if x == nil {}
来源：http://hz.sufxvd.cn/gtbadecbwk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinghuilouyu.cn/gthkumetwx.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtvuuadswc.html

[P07] 防抖与节流
来源：http://hz.cdnleiting.top/gtatybljyi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtahhcfqyj.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtpguceyvh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtaffsjzar.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtnujbeuia.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tian-w.cn/gtkxarykpv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtdbpdgbyp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.0kj1m.cn/gtqvxppafl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.nanxuanxn.top/gtmaxgjhbt.html

[P08] 处理浮点精度问题
来源：http://hz.shangyingyoupin.top/gtloslnfpc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenjidiqi.icu/gtyfkgwcrg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cashguo.top/gtjgklpyhg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinghuilouyu.cn/gtmxwbinhs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gogol.net.cn/gtntupirnc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtyxqjflne.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guannengcc.top/gtptpitaou.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gtlaomhzfv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtbklmcwul.html

================================================================================
来源：http://hz.ybcxt.top/gtzzxxvhek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtmuitqcbz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtoevbywgx.html

[Q01] 创建表
来源：http://hz.52xcode.cn/gtrlvqusmj.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtmqomwmdk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtbfiiflwj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.meibo888.top/gtckkzcojv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtpnumlxrb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtfaqjidpd.html

);
来源：http://hz.xuanzx.com/gtiwguugcq.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtrhjspkot.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gtdvsuvvro.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtxspefipx.html

user_id INT NOT NULL,
来源：http://hz.9152youxi.cn/gtffbqpgel.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtzomigdej.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yangfankeji.com/gtedsdcnhh.html

);
来源：http://hz.jinghuilouyu.cn/gtrhetuntx.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtsymxnidc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xingfuxueyuan.xyz/gtufvxgngi.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gtlbysdjfb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yanxiufei.cn/gtyqfaeeua.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtrbcahkrd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtmigfxqja.html

[Q06] 删除列
来源：http://hz.xuetiantiany.cn/gtmnoxppym.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtvfuwupwb.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gtsumlzwzh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zycfv.cn/gtpfnyzbrk.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtpqpxbzjp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtyuipipih.html

[Q09] 创建唯一索引
来源：http://hz.dianchejie.cn/gtuabxgipx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtexmurpop.html

[Q10] 插入单行
来源：http://hz.guowangkeji.top/gthoaynvqd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jlsjyb.cn/gtsuumggxp.html

[Q11] 一次插入多行
来源：http://hz.zhongyouzk.top/gtapldbfxz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtzclcwnhe.html

[Q12] 插入后取自增 ID
来源：http://hz.chenlongwang.top/gtgharsjsv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtbgegldqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gthvxucmxq.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtqjtbydik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daxiang520.top/gtxdovmubn.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtxnvbazwn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jqgfzy.top/gteerqbntn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuetiantiany.cn/gtchyxkwas.html

[Q15] 查询全部
来源：http://hz.yuanzhike.top/gtiseswomo.html

SELECT * FROM users;
来源：http://hz.redwolf501.top/gtmvahajuj.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtcizoaopc.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtgvwaqkug.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gtguvsphib.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgfzy.top/gtdyhfoops.html

[Q18] 模糊匹配
来源：http://hz.hnxiangtu.top/gtfqhrqcvt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gtygwjygoo.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtcseqjewf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jiagoushi.top/gtdisloybf.html

[Q20] IN 列表
来源：http://hz.pycfn.com/gtpokonpdx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtwdpkoctb.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gtkpsywwmx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zdqjudy.top/gtdunivpta.html

[Q22] 排序
来源：http://hz.daxiang520.top/gtqefnztvw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yonumen.top/gtrccwvmfe.html

[Q23] 分页
来源：http://hz.haohaochexian.top/gtjuqmrygn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gthomhtxrm.html

[Q24] 去重
来源：http://hz.shuidangran.top/gtmadqogaw.html

SELECT DISTINCT city FROM users;
来源：http://hz.52xcode.cn/gtcslxbrml.html

[Q25] 只取前 N 条
来源：http://hz.yueranfly.top/gtjjprarkx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.c1oappe.top/gthablxxog.html

[Q26] 计数
来源：http://hz.yonumen.top/gtjuxmxvem.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gtsibxqkma.html

[Q27] 条件计数
来源：http://hz.9152youxi.cn/gtfmlmxyct.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.svipenyu.cn/gtibexdvex.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtnmajzkup.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtiiznsfuy.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtecydncws.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gtorcdoiae.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtqfdnficm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtcqfqubvj.html

[Q31] 分组后过滤
来源：http://hz.yuanzhike.top/gttghkinvt.html


<!-- 参考信息 -->