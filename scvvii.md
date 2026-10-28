代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://hz.iojbl.cn/gtlkblckel.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtvmnuljkc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtfctmqtzi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtrkghwitw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtnloosqle.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtguaqsmga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhongyouzk.top/gtmhhophxt.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtnglkrocf.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtjzmemhdw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtmkildnsq.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtqlterobp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daxiang520.top/gtvlxynswr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtfpzotgix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtvnpjuyqz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtfrxycmhv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtwnbnjgxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtksttcqmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtwzrpmzts.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gteluepjpv.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtmrvxdybn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtzpjqcnis.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtfelqcsjo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtxmstvyaz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtkmdaprln.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sufxvd.cn/gtzphenjvm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtvejiwsob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtjbonozco.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtzwjidvqc.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gtvakxanul.html

Py:   math.gcd(a, b)
来源：http://hz.snrcjt.cn/gttjhyndtu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtgylpkdmg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtqvnbppfc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtrtsaerzq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtesxsjrso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtvcrcfsub.html

Ruby: a.gcd(b)
来源：http://hz.hnxiangtu.top/gtwygwhzow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.feifeiyinyue.top/gtwzgpjnsg.html

[N06] 判断回文字符串
来源：http://hz.meibo888.top/gtlfxdonvm.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtldltchow.html

PHP:  $s === strrev($s);
来源：http://hz.gaohongyu789.top/gtvdaqbwcu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtideefcpi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtdcyrgacx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtprnobaku.html

Go:   // 双指针从两端比较
来源：http://hz.birdmap.top/gtutykekay.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtzlwtjnui.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtjpcrmnkt.html

[N07] 两数之和（返回下标）
来源：http://hz.wangdashe.top/gtafsxring.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gtfagvtyfg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtpmszvica.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtfiepyvim.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtkrwkwqgh.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtevwokzcj.html

Go:   // 手写 map[int]int
来源：http://hz.yj202588.top/gtdgkgnrzr.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtrbscvpbe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtxirrwprz.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtzqfqalxh.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtjwfsmfls.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtombhpfuo.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtzrsxozck.html

TS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtmdbqjfic.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtxxmzzyys.html

Go:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtgckceqnx.html

Ruby: arr.permutation.to_a
来源：http://hz.gaohongyu789.top/gttgjfxnec.html

C#:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtopctyxfo.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtvykoxrlr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.snrcjt.cn/gtwuppqhwf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtsnbsadmv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gteofdjchd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtmgzgoluf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtsfedtegj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gtblbdenrc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtwbkqvgkh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtowkjopyi.html

[N10] 链表节点定义
来源：http://hz.tian-w.cn/gtpwayobrh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtyoppapzv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtohhaezmr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydjk.org.cn/gthnftyqkk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.316326.xyz/gtplfowgra.html

Java: class Node { int v; Node next; }
来源：http://hz.sxryk.cn/gtlrxntcex.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yanxiufei.cn/gtuzatgblt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cucudq.cn/gtlexlccut.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.haohaochexian.top/gtppdixyhk.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtybfojchk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtlkgglvet.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtjynqbhgd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtjrkukpjd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtjjjpzmwc.html

Java: // 手写递归
来源：http://hz.yvedp.cn/gtxvjtwwow.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtwsghojjd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtdyhdisbc.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtjdhoospw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtoteylxkd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtuvdwdcag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.birdmap.top/gtdmhrutyu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtqbayxdtk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtxeefhpnu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtiykaycfh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtvicgbbjc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtnhywyasn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtlpyulket.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnnovbuwr.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtwaxotrwg.html

================================================================================
来源：http://hz.zhengqikj.top/gtdaysdseu.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtsdaithrc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtxctcsvtn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jianghu66.top/gtjegrfham.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtjwqikiih.html

TS:   // 同 JS
来源：http://hz.gogol.net.cn/gtnqatombc.html

Java: new Thread(() -> f()).start()
来源：http://hz.sysykeji.top/gtvcscflau.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtfnmuvehm.html

Ruby: Thread.new { f }
来源：http://hz.aibaodan.cn/gttjnsydei.html

C#:   Task.Run(() => F());
来源：http://hz.yj202588.top/gtgpwlzieu.html

[O02] 使用线程池
来源：http://hz.hnxiangtu.top/gttjghwzsc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ivvv.top/gtomzbppyn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.redwolf501.top/gtmimatwkv.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtktennlpz.html

TS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtjcfsbaju.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtkrmtsqsg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.daria6918.cn/gtvkolrwnp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtmpcjaxgt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuanzx.com/gthyysrmtu.html

[O03] 加锁保护共享数据
来源：http://hz.hnxiangtu.top/gtvmpyldxf.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtotifvutz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtapwphone.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtzowcgyhq.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtcmixfekg.html

Java: synchronized (this) { shared++; }
来源：http://hz.316326.xyz/gtadjilcqp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.quarkkingdee.top/gtynvekgsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.feifeiyinyue.top/gtvornesap.html

C#:   lock (gate) { shared++; }
来源：http://hz.redwolf501.top/gtccfvnrby.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtcvvbxfdz.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gtkuzntrpf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtxfofnxfi.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtpniwbkzi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtdbnxixql.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtqbunvghn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtiqdmwmvn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhoulong.xyz/gtnftpomoe.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtkvmraohe.html

[O05] 并发执行并等待全部完成
来源：http://hz.haohaochexian.top/gthgunnvob.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guowangkeji.top/gtsafrwgaq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtcwayljhw.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtpdjvjuxu.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtlpqpbwmc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtnrzjzxpw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gthaamtgdp.html

Ruby: threads.map(&:join)
来源：http://hz.zycfv.cn/gtjsfuniyf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gaohongyu789.top/gtrwdrffgy.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gtcolqkmau.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtxqzweptg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtgietiiii.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtnckvjcof.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtuspqiclr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtzsyainws.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtdinteoeo.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtibnudffh.html

C#:   Parallel.For
来源：http://hz.jqgufenzy.top/gtiavvhjso.html

================================================================================
来源：http://hz.fengsongda.top/gturrepnxn.html

P. 常用工具函数
来源：http://hz.nwbrower.top/gtfvpfigej.html

================================================================================
来源：http://hz.cqqwz.cn/gtlxplsnns.html

[P01] 生成 UUID
来源：http://hz.redwolf501.top/gtekqyyfhe.html

Py:   str(uuid.uuid4())
来源：http://hz.daxiang520.top/gtxvbcvjsz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtzfjgqhpp.html

JS:   crypto.randomUUID()
来源：http://hz.yangfankeji.com/gtvddqqomi.html

TS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtdmudtldg.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtxwjkklpm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ybcxt.top/gtbqfrflfp.html

Ruby: SecureRandom.uuid
来源：http://hz.gaohongyu789.top/gtzylctgkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gthwmnjgjp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xinyue.icu/gtukbdveka.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtunwglmfu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nwbrower.top/gtogyemzlw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtrfsosoih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenlongwang.top/gtdjubkeet.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtqiodusuw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtwqjtvrpf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.mhx1999.top/gtzkieviqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtgwxiypqj.html

[P03] 生成短随机字符串
来源：http://hz.yueranfly.top/gtiyfkvftg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtnuerngzo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gtasuzsdcw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtskmjtulr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtzfprxewx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jyoumei.cn/gtkkaeqpxx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtocswlyoe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtyfndrvun.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgfzy.top/gtnppsboyn.html

[P04] 求长度
来源：http://hz.zhaomingkeji.xyz/gtuqxwsduq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtanrbgboa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtxrryunfv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtoegiartr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtwizmsmsk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtqwupdmry.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtcjkzrxyz.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtlowobnfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtcnkroghb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gthijaixtu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtnjiwefjo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cucudq.cn/gtsmmmxjxh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhongyouzk.top/gtlajlyxya.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtzjqccquz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guannengcc.top/gtezqdoojl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtlpketonu.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtaxlszcgq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtudtsawrj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtinvcvadv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtwerxwslv.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgfzy.top/gttfbwrmsf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258.top/gtphrtfcdf.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtwiyjmgef.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtrcrtmbwk.html

Go:   if x == nil {}
来源：http://hz.c1oappe.top/gtfyfljele.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtxtptknvy.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtpeihjsdc.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtzryngtoo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtusyxhyrc.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtpstijohf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtudhyhvbf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtwwqjctas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtausnzahi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tianlin.xyz/gtgubqxmvi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.chenlongwang.top/gtiexsqknv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtrjbbzubk.html

[P08] 处理浮点精度问题
来源：http://hz.hfpthk.cn/gtaekealas.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtooljhwmj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtezlazyvh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtxetwrtnz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yueranfly.top/gtpilbxpqi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.gotoacloud.top/gtnqjwqdog.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gthunehnwb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.316326.xyz/gtqijuoosd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gtuzcdeubc.html

================================================================================
来源：http://hz.birdmap.top/gtjywdptus.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj202588.top/gtguosjqpk.html

================================================================================
来源：http://hz.jyoumei.cn/gtrghngasz.html

[Q01] 创建表
来源：http://hz.birdmap.top/gttsprnegj.html

CREATE TABLE users (
来源：http://hz.ydzc1.top/gtymqeqdpz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtpyhljqlo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gtzlsopwln.html

email VARCHAR(100) UNIQUE,
来源：http://hz.quarkkingdee.top/gtttfexavb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gtzalsirpe.html

);
来源：http://hz.fzhhl.top/gtoirysnpv.html

[Q02] 创建带外键的表
来源：http://hz.xuetiantiany.cn/gtaxpfupkn.html

CREATE TABLE orders (
来源：http://hz.feifeiyinyue.top/gtqwlmtxnj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtvpcphtga.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtccvzastt.html

amount DECIMAL(10, 2),
来源：http://hz.shangyingyoupin.top/gtucvbpfuj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gtqkdrensx.html

);
来源：http://hz.fzhhl.top/gtnhsbnzym.html

[Q03] 增加列
来源：http://hz.c1oappe.top/gtifaskuqm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sweek.top/gtvkzuynme.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gtmnjukphk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gttfaguspr.html

[Q05] 重命名列
来源：http://hz.meibo888.top/gtrpryvjjs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hnqzz.top/gtjswvqdww.html

[Q06] 删除列
来源：http://hz.hysaishi.cn/gtoqbxvtli.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.birdmap.top/gtzcxhgtfk.html

[Q07] 删除表
来源：http://hz.xuanzx.com/gtgxelusor.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtgkqrgsgp.html

[Q08] 创建普通索引
来源：http://hz.jiagoushi.top/gtstxdngfj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtimozguqg.html

[Q09] 创建唯一索引
来源：http://hz.yueranfly.top/gttaouecqp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.wangshuangyany.cn/gtgvjugxze.html

[Q10] 插入单行
来源：http://hz.cashguo.top/gtuomuxzqp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtzdmpvfny.html

[Q11] 一次插入多行
来源：http://hz.chenzaomai.com/gtjpqapjcv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.cheryme.top/gtkvfixdwg.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258888.top/gtlbjcmhgn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shanyushiyangtech.top/gtokdxhubn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtpnftnyjb.html

[Q13] 忽略重复插入
来源：http://hz.svipenyu.cn/gtnpaklpkd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtzjpwngdh.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtlaikcjgt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtcmycccge.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.daxiang520.top/gtqvcnsres.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtugwifxkt.html

SELECT * FROM users;
来源：http://hz.yanxiufei.cn/gtibhacqny.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtsqbgxjyo.html

SELECT id, name FROM users;
来源：http://hz.sysykeji.top/gtdjrchjad.html

[Q17] 条件查询
来源：http://hz.cdnleiting.top/gtiprywvdt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtqhieczkg.html

[Q18] 模糊匹配
来源：http://hz.snrcjt.cn/gtsmaozgcd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhengqikj.top/gtsbwbatve.html

[Q19] 范围查询
来源：http://hz.aizwys.cn/gtkekwjuzb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.guannengcc.top/gtyqqpyrjo.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtxjdnblon.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xuetiantiany.cn/gtsiaqalac.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtibzcxdtg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.haohaochexian.top/gtkegoesrx.html

[Q22] 排序
来源：http://hz.pycfn.com/gtfiapyppr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shzxlz.cn/gthibyavoj.html

[Q23] 分页
来源：http://hz.redwolf501.top/gtepzfjvad.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.meibo888.top/gtadveecjy.html

[Q24] 去重
来源：http://hz.sysykeji.top/gtxtuhrxjj.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtoxtwekbo.html

[Q25] 只取前 N 条
来源：http://hz.yj20258.top/gtxsfwwzyg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtmvtnfdzv.html

[Q26] 计数
来源：http://hz.yueranfly.top/gtuzrsmqpy.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtgnvebtxa.html

[Q27] 条件计数
来源：http://hz.cucudq.cn/gtjjiamldc.html


<!-- 参考信息 -->