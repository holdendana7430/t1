代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtzohhhrnb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtueyunnxe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtckviamoy.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtpwlavdbg.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtolwdulfr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtebornhzt.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtyksocdkz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtducovmzk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtkcbqxwwm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtpjdqobek.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtejkdtugh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guannengcc.top/gtravxfysc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gttpwfvtmr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtnkkoepzi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtlsivdwbf.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gthayzwdhs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtthehoxrf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yvedp.cn/gtimhzealp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtxgqzxovl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtgyydmzki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhixingplan.top/gtufhagbui.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtfqxzvile.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtrothgcxn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtrxwyfxmj.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtffvvwcbx.html

Py:   math.gcd(a, b)
来源：http://hz.cqqwz.cn/gtqmvyhxtt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuanzx.com/gtbbdgcteq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtoazimver.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtvfwoihlc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gaohongyu789.top/gtjjlduzzh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtkoyznxao.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gtttogsbwi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtufwnjfkz.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtipwwfdqq.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gttqfnzmuj.html

PHP:  $s === strrev($s);
来源：http://hz.xuanzx.com/gtreuxuqme.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtwkmdkjul.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtmffurglr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtvgsiydcd.html

Go:   // 双指针从两端比较
来源：http://hz.hnqzz.top/gtonkkcumf.html

Ruby: s == s.reverse
来源：http://hz.pycfn.com/gtjvamaegm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtgmdrystr.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtqjnrezce.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tanke756.top/gtuncobims.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gtbdpclaca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtzimhxzgw.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtwxscdbhf.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtyefnowlf.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gtxwfgtkch.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtdyyhrsmd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtblqtcnrh.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtkmihcfmr.html

Py:   itertools.permutations(arr)
来源：http://hz.mhx1999.top/gtzvjdmgyk.html

PHP:  // 手写递归交换
来源：http://hz.haohaochexian.top/gtwooigyoi.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtftgkrdwm.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtpjnitbss.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtaviaxptp.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gtxbaaijrl.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtrlwxrzwg.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtjvksqtrr.html

[N09] 栈与队列
来源：http://hz.c1oappe.top/gtuvgetrqg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhixingplan.top/gtqjitnofl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sweek.top/gtxvgcahcl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.mhx1999.top/gtsozwwzke.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtrzejjqzn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gtivcxznel.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtlqaqohah.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ivvv.top/gtnmklvmyl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.snrcjt.cn/gtepccpygq.html

[N10] 链表节点定义
来源：http://hz.feifeiyinyue.top/gttdnejsmq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtwawqiphu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtaxrqcbzz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtcibnnlgu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtugugyctu.html

Java: class Node { int v; Node next; }
来源：http://hz.chenjidiqi.icu/gtporwqkfh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shuidangran.top/gtdzldwbja.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtzqdfhsjh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtpddzjkix.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtctlisyfw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.haohaochexian.top/gtupuvqxde.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtjiqdadep.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.mhx1999.top/gtbfakluzm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtafgqjppg.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtpoomthlr.html

Go:   // 手写递归
来源：http://hz.shzxlz.cn/gtwufeudaa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtwvdlzugc.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtiupgyeya.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtksvfistu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtmgbigyzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gtrbcgisxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtboykznrn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtjcyovqgi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aibaodan.cn/gtzkvtdiyg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gtywpplsvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gtqyadubem.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtdtthbvmz.html

================================================================================
来源：http://hz.daria6918.cn/gtxhuynuqh.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtnzevilmg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsgxrzawx.html

[O01] 启动一个线程
来源：http://hz.xinyue.icu/gtyqhgvenc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtjhdaxmnd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yueranfly.top/gtxhfokibd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jyoumei.cn/gtwpqwfyei.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtlhkgxycb.html

Java: new Thread(() -> f()).start()
来源：http://hz.pengpengdd.cyou/gtwsjulmqb.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtmnubbqsw.html

Ruby: Thread.new { f }
来源：http://hz.kuanghao11.cn/gtpbmwdmxs.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtlcudjkfz.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtlyfotfnl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gtpugchyxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258888.top/gtqgunbpao.html

JS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtdujzjgkc.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtpkjccpll.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenzaomai.com/gtqanwmdlz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhiwuduotai.top/gtvplvtilg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nwbrower.top/gtvvzxqvai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtvqvhyssq.html

[O03] 加锁保护共享数据
来源：http://hz.mhx1999.top/gtciussfxa.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtoeybgycq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yuanzhike.top/gtaacigmgm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gthqdfgrye.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtlkvvusdh.html

Java: synchronized (this) { shared++; }
来源：http://hz.iojbl.cn/gtchvlivqu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtiyjpcril.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtbzbltdyg.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtbjnnwmkh.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtivhijnfy.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gtakkqnagy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gtqvnqmdyc.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gtzshjnlks.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.feifeiyinyue.top/gtspluypcw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhiwuduotai.top/gtaiyaslcd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gtebcwyyhl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtkpdhpdfq.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258888.top/gtwrrtvlaw.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxinkj.top/gtprvszyxz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tianlin.xyz/gtsddbfysy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtsydonjjl.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtvuvmkcld.html

TS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtwcoqsjfc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dashuyun.cn/gtpawpgpnh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtdczycgoo.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtukqqdifd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gtipfolmuj.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtwxnieybf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgfzy.top/gtblcolvmz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtwebnmutj.html

JS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtxbxgwwuh.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtyeufqdzd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtybvkbhzq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhixingplan.top/gtnnperysb.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtaaqihjsn.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtsviqmptb.html

================================================================================
来源：http://hz.hfpthk.cn/gtrykklcjs.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtvkixdigt.html

================================================================================
来源：http://hz.c1oappe.top/gthnlexjed.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtgaathsxp.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtueiodrpo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.snrcjt.cn/gtsosckjol.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtrfoihjbr.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtdjpiwydm.html

Java: UUID.randomUUID().toString()
来源：http://hz.hongshengwenyu.top/gtycojwjyc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jianghu66.top/gthwbxlcho.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtjdsdyzzp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zycfv.cn/gtmovdmcif.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xziqi.cn/gtthgrmzje.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtlvmvlrjn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gttrhflvec.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhaomingkeji.xyz/gtufjasxgq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gaohongyu789.top/gtnqidwbch.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cheryme.top/gtzjhwukya.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtmakbuxtj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtocwlxsuz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hfpthk.cn/gtseqpmmqq.html

[P03] 生成短随机字符串
来源：http://hz.birdmap.top/gtuxyxxsfu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258888.top/gtgfpcgzod.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtnzwokexz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtvejuisyx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtkuydxqvd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtkzqwcrdr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtevzpdgwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gtwmytzkli.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sxryk.cn/gtwfhzmeuh.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtbdozinil.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gttxzposme.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gtqkadiqtz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtcmxkriua.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtxqimibsb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yongpay.top/gtoisbhbpk.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtbmxyjmyi.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtjxfhktzs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tian-w.cn/gtiboejeor.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtdudpmzpm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hnxiangtu.top/gttwitobns.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jiagoushi.top/gtivlxbnus.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.fengsongda.top/gtkzrdwltl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtlpaoaiwq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtfokylfia.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fengsongda.top/gtjcejghrv.html

Ruby: a == b
来源：http://hz.snrcjt.cn/gtudgukvku.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.wangdashe.top/gtdowtjjpy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtseybaror.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenjidiqi.icu/gtckshsvmn.html

PHP:  if (empty($x)) {}
来源：http://hz.yvedp.cn/gtirpjoqit.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuanzhike.top/gtpdkrmlqz.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gticxdifua.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aizwys.cn/gtpfwejhlq.html

Go:   if x == nil {}
来源：http://hz.ppjwa.cn/gtagtukyvk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtfrvrmfet.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtzfidiwgo.html

[P07] 防抖与节流
来源：http://hz.yj202588.top/gthwedaidh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtnlllcuhx.html

PHP:  // 手写时间戳比较
来源：http://hz.jinghuilouyu.cn/gtgslsasqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gthkncchin.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtnzsqkdyr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgfzy.top/gtvjalistj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gogol.net.cn/gtemnreaab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtwbgywlvq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtarkofndo.html

[P08] 处理浮点精度问题
来源：http://hz.c1oappe.top/gtgjiufrav.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gttwwsxhkp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenjidiqi.icu/gtvvkshjbp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtxeymstei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.redwolf501.top/gtyhyitzop.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shzxlz.cn/gtyymuqixl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zdqjudy.top/gtwwvggikv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtyowlivhx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtijzarbvi.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmfpkxhom.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtbnvnqjcm.html

================================================================================
来源：http://hz.daria6918.cn/gtrasiohwq.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtenbpojlz.html

CREATE TABLE users (
来源：http://hz.cheryme.top/gtfndlsonf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnxiangtu.top/gtvezfdqxn.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj202588.top/gtvwlzszyg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dianchejie.cn/gtvzchnoaw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gtjklybyno.html

);
来源：http://hz.zhongyouzk.top/gtfpzcdpdm.html

[Q02] 创建带外键的表
来源：http://hz.svipenyu.cn/gtytqguatm.html

CREATE TABLE orders (
来源：http://hz.nwbrower.top/gtdovuneif.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtttnqslbn.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtmscktpmo.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtgrzvpjnt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gotoacloud.top/gtrkmrhigd.html

);
来源：http://hz.hongshengwenyu.top/gtilnektlg.html

[Q03] 增加列
来源：http://hz.tian-w.cn/gtvygvalyz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ivvv.top/gtodqoyoch.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtjrjbcsdz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigfzy.top/gtvcvkkamo.html

[Q05] 重命名列
来源：http://hz.iojbl.cn/gtdoynfsmm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tanke756.top/gtvkromdok.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtdxzaczbw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnxiangtu.top/gtxgqxtvtd.html

[Q07] 删除表
来源：http://hz.yonumen.top/gtjlsrdfrr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgfzy.top/gtpaxbxhge.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtqpkcpphb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtlozdqklt.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gtqeupdccb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtfbsucqkr.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtwjvncafv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.wangshuangyany.cn/gtgzrqjhwa.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtnpapufnh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtkmlgolje.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtmoasiorf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.feifeiyinyue.top/gtqfwokcdc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gtpzpxbdxq.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtyrsromhq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtgcojkqes.html

[Q14] 存在则更新（upsert）
来源：http://hz.xylfe.cn/gttfisllxx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtncrtible.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guowangkeji.top/gtcjqathep.html

[Q15] 查询全部
来源：http://hz.aizwys.cn/gtcrpeqpdp.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtvuseafpa.html

[Q16] 查询指定列
来源：http://hz.guowangkeji.top/gtfkvnyzzr.html

SELECT id, name FROM users;
来源：http://hz.smart0.xyz/gtwkioabov.html

[Q17] 条件查询
来源：http://hz.haohaochexian.top/gtcvcbvlug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtniwgzhwd.html

[Q18] 模糊匹配
来源：http://hz.hammf.cn/gtxhgydhyj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtofuvjdqw.html

[Q19] 范围查询
来源：http://hz.0kj1m.cn/gtpsxxnuhn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtjcszdgyi.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtrcwziizn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtdicwvkpi.html

[Q21] 空值判断
来源：http://hz.cheryme.top/gtpflqdhzy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ivvv.top/gtcdxwvnfa.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtrvpzhgkq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtgrxjjpuj.html

[Q23] 分页
来源：http://hz.ydzc1.top/gtqfqlopep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hysaishi.cn/gtgufojxds.html

[Q24] 去重
来源：http://hz.jianghu66.top/gtwfmxpmzf.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gtgzbojhlb.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtdpzwczvp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yanxiufei.cn/gtnphmudjh.html

[Q26] 计数
来源：http://hz.nwbrower.top/gtkkckuefc.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinghuilouyu.cn/gtzvvdgofn.html

[Q27] 条件计数
来源：http://hz.iojbl.cn/gtrpxriuob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tian-w.cn/gteltxfmoa.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtclgthjlr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.aizwys.cn/gtaxkmkvji.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtnnidrtas.html


<!-- 参考信息 -->