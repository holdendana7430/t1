代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtmkkopyzo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtkxfrxguy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gtqhzjnnkl.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gtmnzcehln.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtjvgjzvtk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.316326.xyz/gtwrtimghr.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtwayutaii.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtqojaodxl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtvjnkpdtq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gtfuxrqfhy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtrnxiffwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtzxilxapp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtfolrpvlu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtpcwmhnai.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtlhqmkbez.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtsklctpiu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtkbmmjkhi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtmggdgcjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtnsewuetq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtaomsuajq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtcsqljejd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.snrcjt.cn/gtmwclmkru.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtiohgpgcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtfqpxgnol.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtokfqmuil.html

Py:   math.gcd(a, b)
来源：http://hz.cdnleiting.top/gtxlkscgdg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yueranfly.top/gtvlcmqlvx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtxlfvoxvy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtjgxxopba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtgpmijbdi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nwbrower.top/gtiexqpxth.html

Ruby: a.gcd(b)
来源：http://hz.quarkkingdee.top/gtyjkuxqci.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gttfgdjtme.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtyerfmjmw.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gtjeyswklj.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gthcpvpxoc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtkmdnmhgf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gthwytbqro.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtqlefbzlo.html

Go:   // 双指针从两端比较
来源：http://hz.ehwqpu.com/gtyqlzhtxo.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtfsaepbet.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gthualjraj.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gthvzcpogj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtwkqsoxlx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.havefunace.top/gthbjnefoc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtztpsxdxm.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgfzy.top/gtagtffiyn.html

Java: // 手写 HashMap
来源：http://hz.c1oappe.top/gtobqppvvs.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtoddqqevm.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtkzynsyxs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtugwnmbjf.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gttcfckjrx.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtdskzjnos.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtsbyggyle.html

JS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtjnrtxmjc.html

TS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtwftycrmm.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtqytizzds.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtyesbshdz.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtgukjyevd.html

C#:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtyfdywxvm.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtxntetyys.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtmvshmmfq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtxuahxeue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtxeinpocq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gtyumgdjzd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuanzx.com/gthhadleqw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtqxdptzxz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtbmpbuure.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nwbrower.top/gtwkpdpybh.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtpfnycewf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtjbvnyzuh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ywan-chungtsiang.top/gtvjazoczy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gtcuzvwtlu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtaquoralm.html

Java: class Node { int v; Node next; }
来源：http://hz.aibaodan.cn/gthdxpasek.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gtmjholmst.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gtqugichhx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guannengcc.top/gtytvyxsac.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtzoaztgqc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.havefunace.top/gtxwmybwat.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtqnytcjrr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtrnrloqsv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtnmxnwgex.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gthhtutodj.html

Go:   // 手写递归
来源：http://hz.dashuyun.cn/gtpxvmlrer.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigfzy.top/gtqhlpkckb.html

C#:   // 手写递归
来源：http://hz.aibaodan.cn/gtxqtosmnj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tianlin.xyz/gtgsqpammx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtmzarjztu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtcaopduxg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtrpemjctl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtincimxvd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtatnlbrmo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xziqi.cn/gtkcanrhmt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.birdmap.top/gtuwyewzqk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtcpuplhlf.html

================================================================================
来源：http://hz.daxiang520.top/gtciribojm.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtonaclxhi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtifmqisbx.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtagutivou.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtadpognjb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ywan-chungtsiang.top/gtbdvyacwk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtzycjnehm.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtcvoijwsy.html

Java: new Thread(() -> f()).start()
来源：http://hz.cashguo.top/gtjsstojyp.html

Go:   go f()
来源：http://hz.smart0.xyz/gtbvtdugzo.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtlaodwhqb.html

C#:   Task.Run(() => F());
来源：http://hz.ehwqpu.com/gtvsdvzgji.html

[O02] 使用线程池
来源：http://hz.jlsjyb.cn/gtflchvruq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxuanxn.top/gtmhdprtbn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.svipenyu.cn/gtxiaublsp.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtmaozflzg.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtnmwixoye.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtsixalsks.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hammf.cn/gteifjbcwk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtecyoyjhl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sufxvd.cn/gtmgdhhxkx.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gthfsnxvuv.html

Py:   with lock: shared += 1
来源：http://hz.wangshuangyany.cn/gtlqpyhfti.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yongpay.top/gtdcfjgdii.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gteskegjam.html

TS:   // 同 JS
来源：http://hz.jinqigufen.top/gthajnuulb.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtvdxoqhfh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtcktmvxzb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zdqjudy.top/gtwtfnuhku.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtfyahxict.html

[O04] 定义异步函数并等待
来源：http://hz.yangfankeji.com/gtqdzpxujb.html

Py:   async def f():⏎    await g()
来源：http://hz.xuanzx.com/gtrfllmmhe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtlncdaqim.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gthhbmjbai.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigufen.top/gtwbtjhdit.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jiagoushi.top/gtkizwhhwp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtabzsytdk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigfzy.top/gtpmbyvvwo.html

C#:   async Task F() { await G(); }
来源：http://hz.yj20258.top/gtryciikmg.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhoulong.xyz/gtwrxeaxtg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj20258888.top/gtkbujfxhq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtcrnhxcbl.html

JS:   await Promise.all(tasks)
来源：http://hz.xuanzx.com/gttbchugsi.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtcdwppbjj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gtwgvslhlq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangtech.top/gtvqfvblea.html

Ruby: threads.map(&:join)
来源：http://hz.dianchejie.cn/gttsohgjkv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtlpdbrlzx.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtdwrcqzyp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sweek.top/gteahgotge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtpwiuousg.html

JS:   // child_process / cluster 模块
来源：http://hz.yuanzhike.top/gtrhyrikgp.html

TS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtsxnbrqdk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gtvbpfqlft.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj202588.top/gticvwhawr.html

Ruby: // fork 块
来源：http://hz.yueranfly.top/gtpvjvhdqw.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtkincmdrc.html

================================================================================
来源：http://hz.chenzaomai.com/gtiftukhqg.html

P. 常用工具函数
来源：http://hz.sweek.top/gtktmcifee.html

================================================================================
来源：http://hz.jianghu66.top/gthahnsxic.html

[P01] 生成 UUID
来源：http://hz.0kj1m.cn/gteeeyslio.html

Py:   str(uuid.uuid4())
来源：http://hz.cdnleiting.top/gtpetmhwlr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtdjycqigg.html

JS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtpmbjafvf.html

TS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtfnwuduac.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtcomhnsog.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtdbgyglmh.html

Ruby: SecureRandom.uuid
来源：http://hz.jlsjyb.cn/gtguzvdwiw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtatrwwjzl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtjzoezqlw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtjnpvymfu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258.top/gtznzmcjpq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fengsongda.top/gtarhsjjnr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtzrilldkb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gtislusgeq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hammf.cn/gttjjdivrd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guannengcc.top/gtxeohwvta.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenzaomai.com/gtvdxlkpcb.html

[P03] 生成短随机字符串
来源：http://hz.ydjk.org.cn/gtbqpwrizr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangdashe.top/gtipuklule.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtsproiktx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sxryk.cn/gtgpbhkpaw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nwbrower.top/gtaytjuama.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.smart0.xyz/gtjomgjcve.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gtbfjajjxn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtksirpfdi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtmihicoyt.html

[P04] 求长度
来源：http://hz.nanxuanxn.top/gtwbzfrqwl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtxfhttsqu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtrpjaxmyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtrjpjqwau.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtdlsgwdft.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gaohongyu789.top/gtlsdxmfkc.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtfemnvjga.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtixbgygec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cashguo.top/gtgtlhwczp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.quarkkingdee.top/gtgfrittwm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gtvbnycxkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258.top/gtrjumullr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtdnextbid.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtnrpfcdnb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtxqnevsjp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gteckewmaz.html

Ruby: a == b
来源：http://hz.c1oappe.top/gtlymapawz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gtagmvfewy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtealqpddz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuanzx.com/gtdzpisjun.html

PHP:  if (empty($x)) {}
来源：http://hz.redwolf501.top/gtigvbvaqa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtauwsdvft.html

TS:   if (x == null) {}
来源：http://hz.gotoacloud.top/gtlmdpbwwf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtatzyulyd.html

Go:   if x == nil {}
来源：http://hz.shanyushiyangkeji.top/gtrnpufywz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hysaishi.cn/gttihhjwjw.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtseursryz.html

[P07] 防抖与节流
来源：http://hz.yuxming.cn/gtgvdmbkjo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtwrqapduc.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gtursbmbwp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtevmbhtis.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gthjgjqlil.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtvozmnclm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtjflyjdca.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xziqi.cn/gtlialwken.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.vqdsnc.cn/gtbzoubntw.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gtvorogqsc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yvedp.cn/gtoxcibxwt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.svipenyu.cn/gtqqomaueq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtmcvtnglw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hfpthk.cn/gtjnkeryjx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.aibaodan.cn/gthkqmvbem.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtlsvlfxbw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtjqzicckm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xinyue.icu/gtwfnozxdy.html

================================================================================
来源：http://hz.ppjwa.cn/gtxdlxwsuj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tian-w.cn/gtnnhljmqe.html

================================================================================
来源：http://hz.jinqigfzy.top/gtyvrqcbyb.html

[Q01] 创建表
来源：http://hz.yuxming.cn/gtdhanqffa.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtfwthmees.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtaxzpczhr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtdsizkmre.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtfndeihme.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shanyushiyangtech.top/gtiwdgbvjj.html

);
来源：http://hz.hywenlv.cn/gtdizsxtrj.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtlsdeizio.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtdzhxbevr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtsqwusuuq.html

user_id INT NOT NULL,
来源：http://hz.yangfankeji.com/gtusyudarz.html

amount DECIMAL(10, 2),
来源：http://hz.ywan-chungtsiang.top/gtpweciums.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtkcqnkpyo.html

);
来源：http://hz.guowangkeji.top/gtvfxrkbhs.html

[Q03] 增加列
来源：http://hz.fengsongda.top/gtrckayvbi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtsslbtakq.html

[Q04] 修改列类型
来源：http://hz.daxiang520.top/gtwwcssbku.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenjidiqi.icu/gtxeoktgir.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtdtkrlspl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xylfe.cn/gtekwwhhek.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gtqkqhtjnb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shzxlz.cn/gtlkxotqls.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtjzujxkkj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hongshengwenyu.top/gtwfrcfkrg.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtwztaylxp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtjtnwprtk.html

[Q09] 创建唯一索引
来源：http://hz.shangyingyoupin.top/gtupeqtmnn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtgzslaqnl.html

[Q10] 插入单行
来源：http://hz.zhixingplan.top/gtqidunqml.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtbxdojcda.html

[Q11] 一次插入多行
来源：http://hz.wangdashe.top/gtutlzmzep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtdzlzxxoo.html

[Q12] 插入后取自增 ID
来源：http://hz.zhongyouzk.top/gtwasquhgi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.quarkkingdee.top/gtbwarjkoy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtryodwkpm.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtozwnofas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.wangshuangyany.cn/gtvtcsykpd.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gtkmxtvoqk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtviiaqccr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtnaivkdgv.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtzccpxjsw.html

SELECT * FROM users;
来源：http://hz.zhaomingkeji.xyz/gtijfzuunf.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtbrqowdan.html

SELECT id, name FROM users;
来源：http://hz.hnxiangtu.top/gtejqbuqwx.html

[Q17] 条件查询
来源：http://hz.jinqigufen.top/gtoarcagzd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xylfe.cn/gtyfajhrkj.html

[Q18] 模糊匹配
来源：http://hz.gotoacloud.top/gtrhtoccxv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtkmhpwzag.html

[Q19] 范围查询
来源：http://hz.cucudq.cn/gtkuyejxxp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtnzhpkxdl.html

[Q20] IN 列表
来源：http://hz.wangshuangyany.cn/gtcagoxfam.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtmfwgabvs.html

[Q21] 空值判断
来源：http://hz.c1oappe.top/gtstdwears.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangtech.top/gtfamfwato.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtvawjwarq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yvedp.cn/gtdopweglu.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtsxwqeite.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jiagoushi.top/gtufwrsfed.html

[Q24] 去重
来源：http://hz.zycfv.cn/gtxwvmhzya.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtmlhlyntg.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtpookoufm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gtphkmkijt.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtihxxwseo.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtttnhdhcg.html

[Q27] 条件计数
来源：http://hz.zycfv.cn/gtzqqpaasg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtbiechjmi.html

[Q28] 求和与平均
来源：http://hz.wangshuangyany.cn/gtxqwbldua.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.316326.xyz/gtxxkfrioq.html

[Q29] 最大最小值
来源：http://hz.daxiang520.top/gtwuxjtqze.html


<!-- 参考信息 -->