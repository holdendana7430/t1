代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtczlritvi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtrcvmqfnf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtbmjyxdeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtxihrgprw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtpjvrjjel.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtosuoqczq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtviqsuibw.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtnnklumlf.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtbaqsnwua.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gtoajeoskp.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtiaacykcd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtfxxgwrly.html

PHP:  // 递归实现，或用 usort
来源：http://hz.vqdsnc.cn/gtensghvlb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtzyancygr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtspuryolb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gaohongyu789.top/gthffxphjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtoxhfpsci.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgufenzy.top/gthyyfhskq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtuteugbxn.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtgziotzlf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtjfrgluji.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtikqaulmv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtapvuusyr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtlyovnjgx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtqthpgmjp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hongshengwenyu.top/gtjhmxmmoy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtpsbzlyyc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yanxiufei.cn/gtseaevhtz.html

[N05] 最大公约数
来源：http://hz.pycfn.com/gtwnvoeend.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtjdvbkdpt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtpcaxhnjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtexsupcdx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtclgvfshv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aibaodan.cn/gtldpcqozg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuxming.cn/gtrsmdnepv.html

Ruby: a.gcd(b)
来源：http://hz.zhiwuduotai.top/gtcgplsagj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtfoniqvvt.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtkgkqmsei.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtrjwuklbl.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gtyoboyvct.html

JS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtikzvmtmm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtzolbosay.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtmqoyjqam.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtsjwvnpuz.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtfeoherpt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtfeebolym.html

[N07] 两数之和（返回下标）
来源：http://hz.vqdsnc.cn/gtoizbhpib.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.bjfxy.top/gtlbdeeabw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtayrjlqrh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cheryme.top/gtimgzetkt.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gthhvqfdyj.html

Java: // 手写 HashMap
来源：http://hz.bjfxy.top/gtfwwxotzp.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtalghrloz.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtpsyfdxfz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuetiantiany.cn/gthplhevjz.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtidvkcbsz.html

Py:   itertools.permutations(arr)
来源：http://hz.gaohongyu789.top/gtnlhrtomj.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtmckjlqjv.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtniqrefit.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtxcmwbsdi.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtcjscxkay.html

Go:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtnfvnridy.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gtnrnkwvzy.html

C#:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtxsonczml.html

[N09] 栈与队列
来源：http://hz.iojbl.cn/gthnypfhzv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtdidzucei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtsatftqvm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gtxupjigjh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtjpgwpkqc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtmqhjywpz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtcsowgjwu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtpugmdfmj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnqzz.top/gtjiicrura.html

[N10] 链表节点定义
来源：http://hz.yvedp.cn/gtjllrswsf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gteldxazsx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtondtwqbo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtogaqlggq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.52xcode.cn/gtvqzzmquw.html

Java: class Node { int v; Node next; }
来源：http://hz.zhongyouzk.top/gtbhydnysd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ehwqpu.com/gtvjitcjdc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yongpay.top/gtlvtyueds.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtxsophzzt.html

[N11] 二叉树中序遍历
来源：http://hz.iojbl.cn/gturgrozcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hammf.cn/gtezhuwmhf.html

PHP:  // 手写递归函数
来源：http://hz.ydzc1.top/gtroxbqgqz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtsiziwhqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtsrdjgidq.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtckqqrxes.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtcjopbosk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtablmzeci.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtskrcofgk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjfxy.top/gtvvmfudmu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtjzylhdcn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgfzy.top/gtzrxtdjog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtjkpwhvhf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtmvjfsyoa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtbsqirqog.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtuepydofw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtiwmypuzt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtswkhawfh.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthqbffxvw.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtiypkjpqh.html

================================================================================
来源：http://hz.gogol.net.cn/gtcmyogajp.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtwjjznjop.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtdkqjibal.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gthaqrnksw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtlzvntwzl.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtcdytyqkp.html

Java: new Thread(() -> f()).start()
来源：http://hz.sxryk.cn/gtshklkkvj.html

Go:   go f()
来源：http://hz.hfpthk.cn/gtnroamtui.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gthieinlio.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtakceeryd.html

[O02] 使用线程池
来源：http://hz.shuidangran.top/gttdwrjryt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtkksbirrc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhijiandao.cn/gtojagllak.html

JS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtlgsyuybe.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtzazvwkvu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hywenlv.cn/gtlvmicdxt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtlklkuemr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtwdjfhliz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gtrkasebpe.html

[O03] 加锁保护共享数据
来源：http://hz.feifeiyinyue.top/gtwscxvgil.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtnjqmtyyx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gaohongyu789.top/gtbhavnbqi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinyuanbaomall.cn/gtanazaszf.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtsiczsuzk.html

Java: synchronized (this) { shared++; }
来源：http://hz.chenlongwang.top/gtxsdpzwix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtivkcsejs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtzdpgnhpq.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtvgqkldly.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtptbqptmc.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtjvthkare.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yangfankeji.com/gtrqaihxzn.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtfycejcnd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.iojbl.cn/gtyvnqvhph.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gtdzvszmyr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtmeitogso.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.0kj1m.cn/gtixljvgay.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gteoxpljzs.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtvqnpahut.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtybxmqwdf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtjhxcecxa.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtphtduuvz.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtykzuphbu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gttulsolpo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhongyouzk.top/gtafzfnqen.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtzpuihtlr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gtyubbfpay.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtxrqlenyh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gteeiafwqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aibaodan.cn/gttgolwlft.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gthefgcqfe.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtmzjmfgcv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gtmocblruc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtlpuptwgk.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtmhbzxsee.html

C#:   Parallel.For
来源：http://hz.zycfv.cn/gtcwloufjm.html

================================================================================
来源：http://hz.yj20258.top/gtehjgqpnv.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtwgqurrpi.html

================================================================================
来源：http://hz.cashguo.top/gtappglflm.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtlsfugrta.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtpfaytrea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtfdlycoka.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtmorkkbzf.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtvmcjzbqx.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtcswzpjvw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangkeji.top/gttjmhinny.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtugdoubqt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gthcjfusgr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtwvgdricl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtbuiyxmji.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtkexdfsox.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.9152youxi.cn/gtitdfrncn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zdqjudy.top/gtkimoekfx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xuetiantiany.cn/gtcezrpvrc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtabaodwny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtzwrzncbt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jlsjyb.cn/gthvlczskr.html

[P03] 生成短随机字符串
来源：http://hz.ehwqpu.com/gtsmpubjbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtomfydsom.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtgdmeqshm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtucswvqfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtgmbdtuxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtpgbjrcoo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtezxshqet.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangkeji.top/gtkcfaeslk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtzqjuwkqu.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gtcybkvmqt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gteayrpdnc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtxseczvyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtvsrzilqh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tanke756.top/gtakvnjkih.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zycfv.cn/gtvhttmjps.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtvgtylfzm.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gtzhfvrjqd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtrvxtralm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtikffzjdr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hongshengwenyu.top/gtzudnygam.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gtcmsxhovw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtbkgqlysb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtojdxdvbw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtfvtuukne.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtprhhyvdt.html

Ruby: a == b
来源：http://hz.sysykeji.top/gtzuhhaajd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtvfdazrnr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.iojbl.cn/gtfeecchen.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sufxvd.cn/gtzkrxmtyn.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgufenzy.top/gtmhrziejw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhoulong.xyz/gtrsmajzuy.html

TS:   if (x == null) {}
来源：http://hz.yuanzhike.top/gtqjtcgzcs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gtnqcovbil.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtqjyngfyh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtcupygwgy.html

C#:   if (x is null) {}
来源：http://hz.gogol.net.cn/gtyffdtxio.html

[P07] 防抖与节流
来源：http://hz.hysaishi.cn/gtsnhtuscp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtguodtwpf.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtypuikzrc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtxgnmnroh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtzhhjgqnf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinqigfzy.top/gtktaylwzs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sufxvd.cn/gtiaeckwaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zdqjudy.top/gtkryaasgb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fzhhl.top/gtnkzboqxc.html

[P08] 处理浮点精度问题
来源：http://hz.yuxming.cn/gtgtvevhja.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtkowfvqqj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258888.top/gtfzmcbvzb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenjidiqi.icu/gthlymabxt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtyqbhjnht.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xuanzx.com/gtlyiavhrf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ybcxt.top/gthqmbgjkd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.birdmap.top/gtigjvhuth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtcpyazkkq.html

================================================================================
来源：http://hz.shzxlz.cn/gtqbkgyade.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shanyushiyangkeji.top/gtkjgscdtc.html

================================================================================
来源：http://hz.ybcxt.top/gtmrlntykq.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtpedavezm.html

CREATE TABLE users (
来源：http://hz.smart0.xyz/gttloalica.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtqwcwucjx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tian-w.cn/gteyqgudto.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sufxvd.cn/gtisjpeoir.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtyuxvnfgn.html

);
来源：http://hz.yueranfly.top/gtajsebkpl.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtgckioaag.html

CREATE TABLE orders (
来源：http://hz.cashguo.top/gtadtisfle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtxdyurgvf.html

user_id INT NOT NULL,
来源：http://hz.aibaodan.cn/gtycvvzztm.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtjlsxdxeu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtkcyqqvkt.html

);
来源：http://hz.nanxuanxn.top/gtkmawkjid.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtfrpeunbt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtghgkifvn.html

[Q04] 修改列类型
来源：http://hz.fzhhl.top/gtegifjufc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtlymooykj.html

[Q05] 重命名列
来源：http://hz.yj20258.top/gtqlixwlls.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtlaghsvwf.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gtiiofctpw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtzybtfpgk.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtmuonkvtg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yj20258888.top/gtejroqcoc.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtdbzgnwqv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fzhhl.top/gtuacnchqn.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtaybuoifl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinyuanbaomall.cn/gtwtucfzcd.html

[Q10] 插入单行
来源：http://hz.yonumen.top/gtneveobaq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtetfswzec.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gthoiktfmy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.guannengcc.top/gthzblcmzb.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtfsvypdcu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtblqqsztp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hywenlv.cn/gtkmfuvkdh.html

[Q13] 忽略重复插入
来源：http://hz.c1oappe.top/gtvxbvhdct.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtnvafpccy.html

[Q14] 存在则更新（upsert）
来源：http://hz.ydjk.org.cn/gtmgykegod.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yueranfly.top/gtkictrfqx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtkqfflhob.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtwsgdomuh.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gttixfvwny.html

[Q16] 查询指定列
来源：http://hz.vqdsnc.cn/gtlndhrsca.html

SELECT id, name FROM users;
来源：http://hz.gogol.net.cn/gtvoqgqfyi.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtjzodlazk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtciiidzer.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtubjatqlv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.vqdsnc.cn/gtnlwamojv.html

[Q19] 范围查询
来源：http://hz.yangfankeji.com/gthxoeaibe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtzqxkevwc.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtwmpvqjxc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jiagoushi.top/gtsarpqqjq.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtuhlghcgr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuanzx.com/gtiykgyywo.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtuicapnkh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daxiang520.top/gthvxssnir.html

[Q23] 分页
来源：http://hz.ivvv.top/gtblrxmgpz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ppjwa.cn/gtlsvbuxkf.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtnthbqbtu.html

SELECT DISTINCT city FROM users;
来源：http://hz.shuidangran.top/gtnxujqwkz.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtsyqnzlxq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtsuthuhfq.html

[Q26] 计数
来源：http://hz.haohaochexian.top/gtlisrqkrq.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gtwtgiibxv.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gteikjezyl.html


<!-- 参考信息 -->