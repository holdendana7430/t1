代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtkgyxijpa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gtsomsqcby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtaklavxka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtmvqjqvee.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hysaishi.cn/gtsqybumze.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtzrrpheff.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gthvpxdmcj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtgtczfnme.html

[N05] 最大公约数
来源：http://hz.zhijiandao.cn/gtgfbwldqr.html

Py:   math.gcd(a, b)
来源：http://hz.feifeiyinyue.top/gtglshgjgk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtxzflphmb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtczlcwelr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtlvfoynrv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xziqi.cn/gtxccbrcra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtkydmgaox.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtyrbbjquo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuanzx.com/gtpmoxmnaa.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtcjgdcyqq.html

Py:   s == s[::-1]
来源：http://hz.hnqzz.top/gtkwlidlde.html

PHP:  $s === strrev($s);
来源：http://hz.feifeiyinyue.top/gtxacbmhcj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtakbtjfvk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtihdgcrwv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.316326.xyz/gtkcpjpwrq.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtnisjmqiy.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtvelleobk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtiisfhebc.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gttaldueor.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinyuanbaomall.cn/gtrljzqhwj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj202588.top/gtmrsdhoeg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.bjfxy.top/gtxsiaipla.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtuqbrmywc.html

Java: // 手写 HashMap
来源：http://hz.ydjk.org.cn/gtqryydbhy.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtowxphlea.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtdtywqyoi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtfjaabnns.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtvdawvlro.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gtpcojvtcr.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtpfuczled.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtdwobxmsm.html

TS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtrfivqytw.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtvytswjas.html

Go:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtenycqywp.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtcwaflwhr.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gthgcdiogc.html

[N09] 栈与队列
来源：http://hz.hfpthk.cn/gtpobmccue.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yanxiufei.cn/gtjfwsbimp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jiagoushi.top/gtdpjxbugy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cqqwz.cn/gtirzjslxu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtzsngypjz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtuiniqsov.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.kuanghao11.cn/gthyxsxlzr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtqgtaitmh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtzbfjkuwv.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gtlbucpmsv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydzc1.top/gtfvdejzcp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtjjgvxulm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hfpthk.cn/gtisogwnzb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ybcxt.top/gtglcagcxr.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtljcjazsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtkdntxqvw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtostusuyz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtfnfghejf.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtjralyqrs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangtech.top/gtucztujze.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtybsjxlbl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtkkbfsqci.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtbhkezmhn.html

Java: // 手写递归
来源：http://hz.haohaochexian.top/gtcdtmmwum.html

Go:   // 手写递归
来源：http://hz.xziqi.cn/gtpdgajwqm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtjzszuxyl.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtbxfwwssa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtjccccwjk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtynpypipa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gthrldmufq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtmduhhgxn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtnwgsneyv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtezxpqrnr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtmupntryp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtnhwtuhmo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtatvslpew.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcqsrteba.html

O. 并发与异步
来源：http://hz.0kj1m.cn/gtvdchspin.html

================================================================================
来源：http://hz.zycfv.cn/gtkasouzhm.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gtcybsqlzx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtwgnkokvh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtzizeqdmk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtyazlcxkl.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtfmyujqol.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtkiaackie.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtrndmrsrq.html

Ruby: Thread.new { f }
来源：http://hz.dashuyun.cn/gtfylrpsvc.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtgchkmuvw.html

[O02] 使用线程池
来源：http://hz.cdnleiting.top/gtjwrimrex.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtmizvrvnb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cucudq.cn/gtgmymjlxp.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtzqxltqer.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtzsunyhnl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ywan-chungtsiang.top/gtgzedpwtz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtcdefddco.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhixingplan.top/gtswbxtmgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gthxuoojav.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtmexgwzhw.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtlzqqiluc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gtvgzaavkp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtoaygzvoy.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtarqyhrtg.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtiopvwsdl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tianlin.xyz/gtldhlituy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.svipenyu.cn/gtdoambviq.html

C#:   lock (gate) { shared++; }
来源：http://hz.jyoumei.cn/gtpetuayvp.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtnwrplegn.html

Py:   async def f():⏎    await g()
来源：http://hz.redwolf501.top/gtmznyakwc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gthjguktvi.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangkeji.top/gtlpfmweho.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gthwuoxfxh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinyuanbaomall.cn/gtkhsaznle.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtngqjespa.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gttiqpfflb.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtnwxkvpfn.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtumxslvpo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gtopjckwzl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtwtbtotue.html

JS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtsxsvebop.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtkkjyuqhx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuanzhike.top/gtjizvzeop.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gthdvbrinr.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtbvuibijy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yvedp.cn/gtvmzfubba.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtpoglsjzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cucudq.cn/gtbklklpct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yanxiufei.cn/gtnpapjmus.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtcphrkxer.html

TS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtvouopdqp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aibaodan.cn/gtrtigrkxy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtiziwvnhj.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtzdbkbbfw.html

C#:   Parallel.For
来源：http://hz.kuanghao11.cn/gtxtouivmr.html

================================================================================
来源：http://hz.sxryk.cn/gtuwqayxqn.html

P. 常用工具函数
来源：http://hz.shangyingyoupin.top/gtjvfzqtfu.html

================================================================================
来源：http://hz.xinyue.icu/gtlvqbjsmx.html

[P01] 生成 UUID
来源：http://hz.yuanzhike.top/gtckgyupxa.html

Py:   str(uuid.uuid4())
来源：http://hz.pengpengdd.cyou/gtzjujnkto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yueranfly.top/gtmtlnrjrz.html

JS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtzzlsnyrq.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gthgbqvluw.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtggdrnsdg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jiagoushi.top/gthknxuvgq.html

Ruby: SecureRandom.uuid
来源：http://hz.cqqwz.cn/gtclifaxyv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jqgufenzy.top/gtpgkkejpj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtymvgzafh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtqbkanorr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtnxwanofn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenzaomai.com/gtarcplynl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtipfpsbie.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gtrdjdlhtt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xylfe.cn/gtbdyrntwg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.gotoacloud.top/gtbspeerrg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gthmodkzjf.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gttrsshvvd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtdpuolenc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gogol.net.cn/gtvudszldi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtgrjhwwaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtkhedltxq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zycfv.cn/gtqajbrkna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtrbrkorlz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtrjcrfoki.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.iojbl.cn/gtmuomnell.html

[P04] 求长度
来源：http://hz.jiagoushi.top/gtkataieoy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtcnvrulkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtixtrfjqq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtqjejoumy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gttmlxpmeo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtmmsxepgy.html

Go:   len(arr);  len(m)
来源：http://hz.gogol.net.cn/gthhkaxvqh.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gtwkuxzzbu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.0kj1m.cn/gtusfanmve.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtpmvxdnkr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gtfivsfzbz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgufenzy.top/gteaoklmky.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtnoahnjei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtdnknghrr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ywan-chungtsiang.top/gtrmktqdql.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.andypj.xyz/gtwnyztfpk.html

Ruby: a == b
来源：http://hz.shangyingyoupin.top/gtagceepym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhengqikj.top/gtzgmyziex.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gttyuxjovu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gtbyremfyo.html

PHP:  if (empty($x)) {}
来源：http://hz.shuidangran.top/gtvvltidda.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtrahgkvgb.html

TS:   if (x == null) {}
来源：http://hz.xuetiantiany.cn/gtrewmfzva.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.tanke756.top/gthxrpebgo.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtgjueuwrf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtufxniqxd.html

C#:   if (x is null) {}
来源：http://hz.sysykeji.top/gtlybwmlwz.html

[P07] 防抖与节流
来源：http://hz.ydjk.org.cn/gtejoqftzo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shangyingyoupin.top/gtneyxbmql.html

PHP:  // 手写时间戳比较
来源：http://hz.gogol.net.cn/gtgqydxnir.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtriogoaid.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtlzhyhmik.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daria6918.cn/gtzbhkvbfw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtonbswsqc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ybcxt.top/gtrgktubsr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.feifeiyinyue.top/gtritpreef.html

[P08] 处理浮点精度问题
来源：http://hz.svipenyu.cn/gtzzfxkoxc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtpvpfvsir.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtonwkmuus.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhengqikj.top/gtxeafgpgi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gteckipqqz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.0kj1m.cn/gtzhigvvll.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnqzz.top/gtzkpralgp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnxiangtu.top/gtvgqxthqa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258888.top/gtlnjrrctz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtshzzzbtu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtbypcxckh.html

================================================================================
来源：http://hz.yj20258888.top/gtoalfioqc.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtzttwlisv.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtnjfpjjvd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinyuanbaomall.cn/gtyletwogi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guannengcc.top/gtqrlzzbrd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtuusbcdxj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gthyzbazvh.html

);
来源：http://hz.meibo888.top/gttkbnjnpl.html

[Q02] 创建带外键的表
来源：http://hz.hongshengwenyu.top/gttoxaqlbu.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gtrlslfeqa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhoulong.xyz/gtaaptroww.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gtsrcefpml.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gthadyigvh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtuwuiodsk.html

);
来源：http://hz.ppjwa.cn/gtzxhjuxlt.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtygpljgoe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hongshengwenyu.top/gtefhiiouc.html

[Q04] 修改列类型
来源：http://hz.snrcjt.cn/gtwswhzfby.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtgddkepak.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtezxhynrh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtwngzpsxs.html

[Q06] 删除列
来源：http://hz.chenjidiqi.icu/gtdiwpcprg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sysykeji.top/gtlttsrrlu.html

[Q07] 删除表
来源：http://hz.gotoacloud.top/gtgfbahlmz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gthdznjrts.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtejszykak.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtctnoiutb.html

[Q09] 创建唯一索引
来源：http://hz.guannengcc.top/gtzkstqqpm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtlkgefqwa.html

[Q10] 插入单行
来源：http://hz.quarkkingdee.top/gtojquppvd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guowangkeji.top/gtzzagqvnl.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtxwmxqkit.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sufxvd.cn/gtebpkihzk.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtwpvgfyqa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgfzy.top/gtcqyigppp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gtqnrdzlxp.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtiusehiae.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yongpay.top/gtxkmulpvy.html

[Q14] 存在则更新（upsert）
来源：http://hz.snrcjt.cn/gtmzmeqizy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtgsvduqfm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xinyue.icu/gtfstnskpg.html

[Q15] 查询全部
来源：http://hz.hnxiangtu.top/gtfnrbvbct.html

SELECT * FROM users;
来源：http://hz.svipenyu.cn/gtllsjkxfe.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtcyadwbzc.html

SELECT id, name FROM users;
来源：http://hz.nanxinkj.top/gtbfknojha.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtyooeruor.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gtogqgtilg.html

[Q18] 模糊匹配
来源：http://hz.yangfankeji.com/gtarqweifr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtrlrkvifa.html

[Q19] 范围查询
来源：http://hz.yongpay.top/gtpiozzgit.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtkayffswp.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtadppsohc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhoulong.xyz/gttwnypnaa.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtqsmqehiz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yonumen.top/gtiekhacgt.html

[Q22] 排序
来源：http://hz.sufxvd.cn/gtaghriwbe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gttnhlcvbp.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtsczehipk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtfqbxitym.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtexifiete.html

SELECT DISTINCT city FROM users;
来源：http://hz.pycfn.com/gtinqamaoe.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtmwnzymxn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.havefunace.top/gtbekorikr.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtozrtxchn.html

SELECT COUNT(*) FROM users;
来源：http://hz.0kj1m.cn/gtsuuguhyq.html

[Q27] 条件计数
来源：http://hz.zhoulong.xyz/gtbmvagcel.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtldnlodky.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtvkzathmf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtzclyhtpj.html

[Q29] 最大最小值
来源：http://hz.gzhubu.top/gtspskxauh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtdhcnekrk.html

[Q30] 分组统计
来源：http://hz.quarkkingdee.top/gtlwpbtwaj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtsflorlgu.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gtdovpxkqn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.redwolf501.top/gtdrxxgxto.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gtlbhzlwwl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtgldklgjm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenzaomai.com/gtbjkriixt.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtmvmskcfw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtuylyvbfe.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtgvbpgylv.html

SELECT * FROM (
来源：http://hz.cqqwz.cn/gtwtnpmgon.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtbjsyoezn.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtjdscmuzi.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtbyvuhwnz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dianchejie.cn/gtahvckmys.html


<!-- 参考信息 -->