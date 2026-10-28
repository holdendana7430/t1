代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtakissipv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtkocifxhk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtzuztnwpd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtzuzwfbgu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtprguwzbo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gthqwsklhn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gterfjegdg.html

Go:   slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtbnugfwaw.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtyaadskmw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtdstgvbay.html

[N03] 快速排序（分治示例）
来源：http://hz.cqqwz.cn/gtfapjpomc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtggfkygno.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtnuiikrim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtxeokvgdk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gteufymdfl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.meibo888.top/gtahrgycnm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtqetkceuk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtqtxdgffb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtewcmltft.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gttuiasvnm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtcnouipdm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtxetdezfm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtjvgakjsh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtbukwzxpp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtnyypxqya.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtjcivhmkr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtftducvsc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ivvv.top/gtgpyprepp.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtwtlqisoz.html

Py:   math.gcd(a, b)
来源：http://hz.xinyue.icu/gtrxykrspw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.vqdsnc.cn/gtgugakwmh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtrhsrbjea.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtxshhtpmq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtltvjompw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gtchvhibhz.html

Ruby: a.gcd(b)
来源：http://hz.daxiang520.top/gtpvgfhpha.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guannengcc.top/gtaogxozgo.html

[N06] 判断回文字符串
来源：http://hz.nanxuanxn.top/gtbjvsmcop.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtlspobjox.html

PHP:  $s === strrev($s);
来源：http://hz.xinyue.icu/gtdcvmqhtk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtgxtyymqw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtsfvkhphm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtwqhiajwx.html

Go:   // 双指针从两端比较
来源：http://hz.snrcjt.cn/gtgpicqnmg.html

Ruby: s == s.reverse
来源：http://hz.316326.xyz/gttfqwkudp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtfhibxjar.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtqqggiulh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuanzx.com/gteruxgkuk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gttglsnzdn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtmohthkyf.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtqgqhcugg.html

Java: // 手写 HashMap
来源：http://hz.sweek.top/gtjbxfhzqq.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtifkbkkvm.html

Ruby: // 手写 Hash
来源：http://hz.jinghuilouyu.cn/gtlvidiafe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hysaishi.cn/gtefcqfqrn.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtisytlaho.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gthbzxcbzy.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gtotvpbheg.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtttaogxpp.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtpbazimtl.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtmmvqayvk.html

Go:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtdbgssxxq.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtrftgyjhu.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtdvsdhgvp.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtbwvxjzlr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtminilylv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtnopolstl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtjjrqzpqa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtgbyshykv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.quarkkingdee.top/gtwtmpzjec.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtckidcfxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtznnzmoao.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daria6918.cn/gttejqmdyb.html

[N10] 链表节点定义
来源：http://hz.yongpay.top/gtmoqxcjdu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tian-w.cn/gtntmeaolx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gtntbbabeo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangshuangyany.cn/gtnfmcfrhl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gttyoprvop.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gthivsdjjb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtxsjscckj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daria6918.cn/gtnndjcmnc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtbdknutby.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtzmkkgnru.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtcdyxmzod.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtbqafdhhw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtmwagyxql.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtzscwnaaz.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtzvsslzep.html

Go:   // 手写递归
来源：http://hz.hfpthk.cn/gtbmzdijne.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtebxyzbaj.html

C#:   // 手写递归
来源：http://hz.jiagoushi.top/gtqoybkfdv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gthrejuvcz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xylfe.cn/gtimkpkwbt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gtnhkagmhs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtcmlpsqjk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtqfebragx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtgepwfgmg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtdxdhqpwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daria6918.cn/gtxoqkpqrm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtprkwacan.html

================================================================================
来源：http://hz.dashuyun.cn/gtfnyydzky.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtjivckvnx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrzybajix.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtefyitjgw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.mhx1999.top/gtbtqtkcvp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtxcsijxfn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtnhaftfpr.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtpspwxoos.html

Java: new Thread(() -> f()).start()
来源：http://hz.hnxiangtu.top/gtcrgoncky.html

Go:   go f()
来源：http://hz.jianghu66.top/gtbqlzanhj.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gthhwvhybh.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtglxtjhpa.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtmagszylr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtpmpqjvwl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hysaishi.cn/gtamvozadq.html

JS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtgcoamtha.html

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtlxvscqvm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jqgfzy.top/gtfybcvduu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gtbihzludm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hfpthk.cn/gtnkkfopig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.mhx1999.top/gtyshcqhsm.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtmulokjto.html

Py:   with lock: shared += 1
来源：http://hz.aibaodan.cn/gtzzwmqahx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtmwxokfvi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gttulxwcrh.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gtlaivroyw.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtgtnnstgq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtcpwvqpdj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gtexmlvvjv.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtruxgliqe.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gtczsqzbsl.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtgryfkato.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shuidangran.top/gtbhvgheza.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtlyiqmtex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtlffmjshe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtenhyoxkk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtvddnxkid.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtwqveeyug.html

C#:   async Task F() { await G(); }
来源：http://hz.tian-w.cn/gtzyfwpnbm.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtzwcaqqng.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtoaugueov.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtyohdzjwa.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gttrnshuit.html

TS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtkckwtmol.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yonumen.top/gtffcmvvgz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtxxukkeco.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtglvbzhbn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yueranfly.top/gtudcwtmrn.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtulvahxvt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuetiantiany.cn/gtpvaiwxeh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ivvv.top/gtuyccswiy.html

JS:   // child_process / cluster 模块
来源：http://hz.daxiang520.top/gtmlvyzzsm.html

TS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtmzqvkdot.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hongshengwenyu.top/gtrbsnbkfj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.guannengcc.top/gtivdnwlny.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtmqtfrpgt.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtabhpoeok.html

================================================================================
来源：http://hz.ybcxt.top/gtbezpnnst.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtlcpwkwwf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvnbspogx.html

[P01] 生成 UUID
来源：http://hz.feifeiyinyue.top/gtjoscgbho.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtnoiwlqae.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.meibo888.top/gtkplwugob.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtahbcmcbk.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtmcddugqx.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtifqsrbuf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtyklyzqyp.html

Ruby: SecureRandom.uuid
来源：http://hz.9152youxi.cn/gtbfibwvga.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtfqgugevd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtvcthijxj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtlpzhiybu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.guannengcc.top/gtnyujrnix.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gtdpjqvvta.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtllepwtzk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtarpvnmwn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinyuanbaomall.cn/gtddophheo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhixingplan.top/gtawzqcwdl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgufenzy.top/gtxcmxanqv.html

[P03] 生成短随机字符串
来源：http://hz.andypj.xyz/gtejrfodvw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtcdigohcb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtltdawqle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtoozbuasl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtnnjjxhkc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhiwuduotai.top/gtmbtqqfpa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gtwibhvoyz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhijiandao.cn/gtwfzewgfj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtoymkwqzr.html

[P04] 求长度
来源：http://hz.pycfn.com/gtptmseuxo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sxryk.cn/gtzrgljjnr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtzauoeakt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtpgwbvsin.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtdvaqkhdd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtaxddiyid.html

Go:   len(arr);  len(m)
来源：http://hz.sxryk.cn/gtwgrwswzr.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtpvwyspwx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gtcmyqzqek.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydjk.org.cn/gtzcybocpl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhaomingkeji.xyz/gtrxbgrqql.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gtgwrfcvlc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtcotcrfoh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtuyyetzog.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gthjaeaayx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gttqyvjfsb.html

Ruby: a == b
来源：http://hz.sxryk.cn/gtpetjgypk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hnxiangtu.top/gtrscvxzbg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.feifeiyinyue.top/gtylgbmruv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gtkmjlzwfx.html

PHP:  if (empty($x)) {}
来源：http://hz.pycfn.com/gtshrpykyu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtqontlzqo.html

TS:   if (x == null) {}
来源：http://hz.tian-w.cn/gtqgbdkfvz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jqgufenzy.top/gtyrwsolsh.html

Go:   if x == nil {}
来源：http://hz.yonumen.top/gtjiglovwu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinghuilouyu.cn/gtsuwuigwf.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtgjvcfjji.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gtcmazzeck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtjashvjyu.html

PHP:  // 手写时间戳比较
来源：http://hz.chenjidiqi.icu/gtwhryvloc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtmcrrgwsq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtpitaamuv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtksrpmkzi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gthwhfhbko.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.kuanghao11.cn/gtzvcgzifb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtvjtvaffk.html

[P08] 处理浮点精度问题
来源：http://hz.zhixingplan.top/gtvlwspesq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtmvaduqkr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sweek.top/gtuclhtvvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.0kj1m.cn/gtvbmosojd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtjjqcsfus.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtckvogufo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.birdmap.top/gtsuukctne.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sufxvd.cn/gtktgsyitf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtluqqsitm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkbwueuia.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tian-w.cn/gtnrnhdahg.html

================================================================================
来源：http://hz.andypj.xyz/gtcwqrzxes.html

[Q01] 创建表
来源：http://hz.zhoulong.xyz/gtydshvzea.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gtvqjkawud.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtudtbxbqm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cucudq.cn/gteztmafil.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtpmisyksp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtoskzdvzc.html

);
来源：http://hz.zycfv.cn/gtvwpvlmty.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtbafjeyig.html

CREATE TABLE orders (
来源：http://hz.xylfe.cn/gtzbtllbvp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtiemecmbz.html

user_id INT NOT NULL,
来源：http://hz.yj20258888.top/gttllhsrng.html

amount DECIMAL(10, 2),
来源：http://hz.havefunace.top/gtatmfyrmg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtdrisxwib.html

);
来源：http://hz.yonumen.top/gteemxxslc.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtiouqhkrb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtffskwahw.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtmrccrvpm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtxehmojmw.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtnkcvyrgv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hysaishi.cn/gtvmerxvax.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gtzqffdwex.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xylfe.cn/gtductpket.html

[Q07] 删除表
来源：http://hz.svipenyu.cn/gtuxacjjdz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.andypj.xyz/gtgwyuldpp.html

[Q08] 创建普通索引
来源：http://hz.guowangkeji.top/gtnrhoyafj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jyoumei.cn/gtlbqozpcn.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtxrauneba.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hysaishi.cn/gtfppjobsz.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gtarlnhrhg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.havefunace.top/gtmmhprdrv.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtyrwlcglp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gtvenjybgn.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgfzy.top/gttywrjxui.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtrrbndypl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hammf.cn/gttmsixmqq.html

[Q13] 忽略重复插入
来源：http://hz.guowangkeji.top/gteteamwsm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.aizwys.cn/gticacfmhj.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtsrhzlkuv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gtcuyjqkhb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shuidangran.top/gtktxngvtz.html

[Q15] 查询全部
来源：http://hz.gzhubu.top/gtivjpquuz.html

SELECT * FROM users;
来源：http://hz.cucudq.cn/gtowiuwrir.html

[Q16] 查询指定列
来源：http://hz.c1oappe.top/gtepyrksas.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtlskhjrhx.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtnmoppxbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tian-w.cn/gtsmiuuriy.html

[Q18] 模糊匹配
来源：http://hz.yongpay.top/gtfndeiwml.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gtihfgvwfk.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gtoqmitxvz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ppjwa.cn/gtcpmnemrk.html

[Q20] IN 列表
来源：http://hz.jinghuilouyu.cn/gtwnvczdiu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgfzy.top/gtpcsijdsy.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtdgzzatcn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenzaomai.com/gtohsvurtc.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gtieuddcro.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dianchejie.cn/gtckfkggpu.html

[Q23] 分页
来源：http://hz.fengsongda.top/gtnyghjamz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtgryqktor.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtjccanbtg.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gthjwxgeip.html

[Q25] 只取前 N 条
来源：http://hz.shzxlz.cn/gtaesvzfqz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj202588.top/gtvflwiluq.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtcdudzekk.html

SELECT COUNT(*) FROM users;
来源：http://hz.guannengcc.top/gtitgqibvf.html

[Q27] 条件计数
来源：http://hz.yonumen.top/gtyrydylrl.html


<!-- 参考信息 -->