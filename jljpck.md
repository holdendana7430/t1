代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtvwiqeqoa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtrzwruwus.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtykipjsvv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtddseulhu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gtnmsvvpps.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtpvxcfime.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtgxsfjlbr.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtxxywytxg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtjffkizzg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj20258888.top/gtouhblcel.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtlzoqeedu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtchlevqtw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtvdnvqerx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtwijvudvq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtvsnzkynt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhengqikj.top/gtxympvioe.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtdooihipn.html

Py:   math.gcd(a, b)
来源：http://hz.shzxlz.cn/gthntetxdh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxuanxn.top/gtacgxqdez.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtiwkzjyfj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gthmsjnsya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtlqqefyyx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuanzx.com/gtyhijgkyh.html

Ruby: a.gcd(b)
来源：http://hz.jiagoushi.top/gtkztvfwnu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtisgsgryq.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtxhzwmdsa.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtentuvmvx.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gtngaugaom.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtauelhuee.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtkugenqtj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fengsongda.top/gtjgpzjtxd.html

Go:   // 双指针从两端比较
来源：http://hz.dashuyun.cn/gtopabmxxt.html

Ruby: s == s.reverse
来源：http://hz.9152youxi.cn/gturkjspvp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gttphtszvc.html

[N07] 两数之和（返回下标）
来源：http://hz.c1oappe.top/gtzelgdfec.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtmscotcrs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtplrbjylz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtgqpiddtz.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gttfzoseua.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtckmjthtb.html

Go:   // 手写 map[int]int
来源：http://hz.fzhhl.top/gtxjxjpkql.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtzpaeyljk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.vqdsnc.cn/gtyooohpjs.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gtuyetttig.html

Py:   itertools.permutations(arr)
来源：http://hz.tanke756.top/gtrtcneigb.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtymiqvgpw.html

JS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtqoftiqen.html

TS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtbsctiozx.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtkyffomlv.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtfspdisvi.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtkklnrixm.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtpuonmxcj.html

[N09] 栈与队列
来源：http://hz.shuidangran.top/gtbpnphikv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtsilafxdf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangtech.top/gtuzjtuxyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtnhnnbqqc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtvfjadqxy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tanke756.top/gtsjfnmpzu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtgzfgwirv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenjidiqi.icu/gtfftsumua.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtsopbesyn.html

[N10] 链表节点定义
来源：http://hz.52xcode.cn/gtdjygprdk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtvhmblkbp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtaxwzixdm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ehwqpu.com/gtyruivqvu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtwieeihtx.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gttkpckiiu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtaibmwcjl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtwsunljgt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtdbiuxhqx.html

[N11] 二叉树中序遍历
来源：http://hz.xziqi.cn/gthozkmfpe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtmwxtvjfy.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtqngkhpvb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtycyersls.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtvqjldcak.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtbxqpmuty.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtxzmjbwdr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hongshengwenyu.top/gtocborswx.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtoenkmpld.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtvmoccbbt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gteqaihkpg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.c1oappe.top/gtikhlsscx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gttgssyopg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtdtqlludy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtbqknzgeg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtgxsihyqa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gogol.net.cn/gtcvwpbtpj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtjlxmlbkr.html

================================================================================
来源：http://hz.9152youxi.cn/gtszmzhefi.html

O. 并发与异步
来源：http://hz.hnqzz.top/gtnnqpxnfk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpyyhisda.html

[O01] 启动一个线程
来源：http://hz.xuanzx.com/gtriyxxiua.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yvedp.cn/gtdbszlsdu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtnaficqpr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hysaishi.cn/gtrzyvxmwm.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtvumqfgna.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gttdkoyrfi.html

Go:   go f()
来源：http://hz.fzhhl.top/gtvdsxcogl.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gtscvrxpgb.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gttxiugntw.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtqptciglj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtlcrmoezd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gtwqnthfaf.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtyplvglhc.html

TS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gttsfufohq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtldlgqwmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nanxuanxn.top/gtusbynjoh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtkutshpij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jlsjyb.cn/gtfzcvurai.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtffsjjmch.html

Py:   with lock: shared += 1
来源：http://hz.havefunace.top/gtpczmuteh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guannengcc.top/gthfzfrxrz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shzxlz.cn/gtexndsaej.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtrjisvhgz.html

Java: synchronized (this) { shared++; }
来源：http://hz.yueranfly.top/gtcypdrymx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenjidiqi.icu/gtyefjtgdy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydzc1.top/gtngsmhshj.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtagutuaxs.html

[O04] 定义异步函数并等待
来源：http://hz.xuanzx.com/gtiowxkbwr.html

Py:   async def f():⏎    await g()
来源：http://hz.gotoacloud.top/gtnudujkyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gteiloajvp.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gttiasgcbh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtklrdoxvo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sxryk.cn/gtcxrpikrx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zdqjudy.top/gtqslqmckp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtuhyqpvjk.html

C#:   async Task F() { await G(); }
来源：http://hz.smart0.xyz/gtkgqmlsuq.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gttanoavpa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gthzgitkqb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtjcidspav.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gteakaykan.html

TS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtjwpckxes.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhiwuduotai.top/gtkqihkndd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cheryme.top/gtebtqetrq.html

Ruby: threads.map(&:join)
来源：http://hz.gogol.net.cn/gtvohekcne.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtuytogldv.html

[O06] 使用进程池
来源：http://hz.guannengcc.top/gtjsgbgbvq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.feifeiyinyue.top/gtcsttadyf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yongpay.top/gtgxrfsdgm.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtgnanglsn.html

TS:   // child_process / cluster 模块
来源：http://hz.guowangkeji.top/gtiekgwdmh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtqdshfuvo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xingfuxueyuan.xyz/gtatgasthp.html

Ruby: // fork 块
来源：http://hz.zhixingplan.top/gtqtmvntfq.html

C#:   Parallel.For
来源：http://hz.zhoulong.xyz/gtiiokqhwl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtevcvvlus.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtuglzxrhr.html

================================================================================
来源：http://hz.fengsongda.top/gtlnarrysn.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtkqajgvkr.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtzlbgvczp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhongyouzk.top/gtprekfnsc.html

JS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtyczxbutn.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtidkfkyzu.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtbjfktjmj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yanxiufei.cn/gtgickootp.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gtmpwrtegp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtzdfeybzo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtogjoufbs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.haohaochexian.top/gtkcgwpybt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hnxiangtu.top/gtcoybpock.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtuefvjyki.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtnscigiqs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtemdqmhlg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtodkevnfb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtvqjjsrro.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gtdyzteqsg.html

[P03] 生成短随机字符串
来源：http://hz.nanxuanxn.top/gtjmewkhon.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jiagoushi.top/gtknvxlrwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shzxlz.cn/gttazofczr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gthqzarruj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtbwggxiur.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtnyrzjwjm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhaomingkeji.xyz/gthhynweql.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fzhhl.top/gthhwsttmb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hongshengwenyu.top/gtqrxbfmnh.html

[P04] 求长度
来源：http://hz.cdnleiting.top/gtbegwmfyw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtbnrxyfto.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtrayxgbmd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gttvnjckhu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtlutcttdi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.aibaodan.cn/gtzirnhbyh.html

Go:   len(arr);  len(m)
来源：http://hz.xziqi.cn/gtlzinfdsb.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtqupdeqgi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtpeqmbgnj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xingfuxueyuan.xyz/gtjpplbpbs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gtuymebyya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cheryme.top/gtrsuxjcqn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yanxiufei.cn/gtgrorpzke.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtwosequkc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtownkumli.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtyfuhheuu.html

Ruby: a == b
来源：http://hz.zhaomingkeji.xyz/gtrmjpijrr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gogol.net.cn/gtfbeesezk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtaxwcukfa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hfpthk.cn/gtonmcnzge.html

PHP:  if (empty($x)) {}
来源：http://hz.zdqjudy.top/gtjutpahpe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhiwuduotai.top/gtsilspbmc.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gtuqzmcflf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cdnleiting.top/gthxdzkyen.html

Go:   if x == nil {}
来源：http://hz.ybcxt.top/gtdbhwluek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tianlin.xyz/gtlmhbjznl.html

C#:   if (x is null) {}
来源：http://hz.jqgfzy.top/gtpgbahdjj.html

[P07] 防抖与节流
来源：http://hz.jlsjyb.cn/gtqjgxqstf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258888.top/gtqezeiful.html

PHP:  // 手写时间戳比较
来源：http://hz.jianghu66.top/gtnmmlstub.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtzeelotjb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtetvfjamj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtjxerfeut.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhongyouzk.top/gthotnnvdp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shangyingyoupin.top/gttwsynekd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gogol.net.cn/gtxqckeffb.html

[P08] 处理浮点精度问题
来源：http://hz.fengsongda.top/gtrmlxtqfl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtgeziyfsf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangdashe.top/gtcflrgqny.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dashuyun.cn/gtxysoteyj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtlqlrbirm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gtdduhhvqh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtyfjfufzt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cucudq.cn/gtgfeeaipx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ywan-chungtsiang.top/gtwnqpifek.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwwlorexb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtnrrgbooc.html

================================================================================
来源：http://hz.jqgfzy.top/gtgpfjwdgf.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtdpkgztzb.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtiyroprqr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtamupjqbs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gttqafxhar.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtoxankphg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtgzcalplv.html

);
来源：http://hz.hysaishi.cn/gtqlmshokz.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtiwrzervu.html

CREATE TABLE orders (
来源：http://hz.c1oappe.top/gtnywundrd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinghuilouyu.cn/gtbwdalnoo.html

user_id INT NOT NULL,
来源：http://hz.feifeiyinyue.top/gtbtfzdlrv.html

amount DECIMAL(10, 2),
来源：http://hz.chenjidiqi.icu/gtccizqxwz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gtrxrnlpqe.html

);
来源：http://hz.jianghu66.top/gtyxxvjbnj.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gtqmkvbnym.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gtdcmodbol.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtfnakfayt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ywan-chungtsiang.top/gtbejytvdx.html

[Q05] 重命名列
来源：http://hz.zhijiandao.cn/gtahrgbvbg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aibaodan.cn/gtbdwphuxn.html

[Q06] 删除列
来源：http://hz.xylfe.cn/gtbmbffvbj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtvdcrxkbx.html

[Q07] 删除表
来源：http://hz.dianchejie.cn/gtxlooiqyt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtdmkaudlf.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtcxqdwkdr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gtpqbspqkv.html

[Q09] 创建唯一索引
来源：http://hz.zycfv.cn/gtglmyaemc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtezbecmhb.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtbnlbjlgn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.9152youxi.cn/gtesqmradt.html

[Q11] 一次插入多行
来源：http://hz.feifeiyinyue.top/gtutdrkzwv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtfmmqqmiv.html

[Q12] 插入后取自增 ID
来源：http://hz.hammf.cn/gtmgtkkumh.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtclraotbz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtsuooftdr.html

[Q13] 忽略重复插入
来源：http://hz.aibaodan.cn/gtpzapfgcl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtxolacgib.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gtfujpqaiv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinyuanbaomall.cn/gtihedjsik.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.redwolf501.top/gtqsfprybs.html

[Q15] 查询全部
来源：http://hz.mhx1999.top/gtfqjardcc.html

SELECT * FROM users;
来源：http://hz.zhiwuduotai.top/gtmhgsauac.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtxcqcejok.html

SELECT id, name FROM users;
来源：http://hz.xylfe.cn/gtahonjgxv.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtkpeagrxk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtqoiqqymh.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtmssuhphs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gtaonlaink.html

[Q19] 范围查询
来源：http://hz.zhoulong.xyz/gtlgbjlebv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ybcxt.top/gtijnmdado.html

[Q20] IN 列表
来源：http://hz.yuanzhike.top/gtgnffxsqz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zycfv.cn/gtmunqogsi.html

[Q21] 空值判断
来源：http://hz.jianghu66.top/gtkbjdvhbo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangdashe.top/gtsgerjmkt.html

[Q22] 排序
来源：http://hz.wangdashe.top/gtnqixresw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtpmrmarpx.html

[Q23] 分页
来源：http://hz.aizwys.cn/gtkuheqsxh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtngqpupev.html

[Q24] 去重
来源：http://hz.yvedp.cn/gtablhjhje.html

SELECT DISTINCT city FROM users;
来源：http://hz.ybcxt.top/gtdhvvdfhq.html

[Q25] 只取前 N 条
来源：http://hz.xingfuxueyuan.xyz/gtgblqunja.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtlgxbklwg.html

[Q26] 计数
来源：http://hz.snrcjt.cn/gtctpibdqa.html

SELECT COUNT(*) FROM users;
来源：http://hz.xinyue.icu/gttwcqvspj.html

[Q27] 条件计数
来源：http://hz.hysaishi.cn/gthuatywla.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shuidangran.top/gtqunvklhc.html

[Q28] 求和与平均
来源：http://hz.sxryk.cn/gtcimhaapf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gtoemlakco.html

[Q29] 最大最小值
来源：http://hz.sxryk.cn/gtmuufvaik.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtstrkygyn.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtvdtrayma.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtzrhjlrde.html

[Q31] 分组后过滤
来源：http://hz.zhiwuduotai.top/gtmpnanjba.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtpvkmtrxr.html

[Q32] 分组拼接字符串
来源：http://hz.aizwys.cn/gtwealklsp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtfknxzbic.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtpiikcyiz.html


<!-- 参考信息 -->