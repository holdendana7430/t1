代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gtkoqmlxyz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtgpmaxqqq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtradauskt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gthhjzuwjj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtcspagnfl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daxiang520.top/gtzkrzasrg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sufxvd.cn/gtfnlyqxes.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtqqhqucac.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtfrkunxai.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtbqdretyy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtajpwnaot.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtckcqhago.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtzhblxvwk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fzhhl.top/gtxoykrzdy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtwmmccryu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtyckhlhsf.html

[N05] 最大公约数
来源：http://hz.xylfe.cn/gtuaoneqyf.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtnerntekv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtzvnjmuny.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtyfqbvriq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtlxxpajuw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtdmcpqhlg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtkjhyvjai.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtzqfshpen.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gtnyrtihbw.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtlfzvtahf.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtusfukocx.html

PHP:  $s === strrev($s);
来源：http://hz.sysykeji.top/gtpbcyyoft.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtzzpmyumw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtlyfouhpb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gturkjltun.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtiacpapqc.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtzvbwvpsz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtiiffzwlq.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtmiwwuizp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yongpay.top/gtonpexntq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtcbazmwuv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gtdgvrhzux.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtajqxxtzb.html

Java: // 手写 HashMap
来源：http://hz.ydjk.org.cn/gtjqvcgdqp.html

Go:   // 手写 map[int]int
来源：http://hz.snrcjt.cn/gtcfoisyty.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtgcefkogl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangdashe.top/gtriarpihb.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gtlrjzcsjd.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gtlszblzvb.html

PHP:  // 手写递归交换
来源：http://hz.pycfn.com/gtvtlahxoz.html

JS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtyqjzfbnr.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtwbymjrxz.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtuvcrocbf.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtmhrodikj.html

Ruby: arr.permutation.to_a
来源：http://hz.cqqwz.cn/gtqedcycnr.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtqrljbtbz.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtoskefbjc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtzifvcrlt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jlsjyb.cn/gtltkcxgtr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtfwhmlzwk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gtmzagnkxi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtdiwjwoaq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtjglimpqr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtzredrgfw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtsyosfzay.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtksbbmwqs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtqxfhdapf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtnkhmhmys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhoulong.xyz/gtjznjuudd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ppjwa.cn/gtrclynscd.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtervmeqbl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gtqgdkbevq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtexzdybnt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tianlin.xyz/gtwrswmynt.html

[N11] 二叉树中序遍历
来源：http://hz.yangfankeji.com/gtuzzxcpwl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnxiangtu.top/gtwootwcyf.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtmwdwfomv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtgwejvfhr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtpeuckejb.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtxizkbtot.html

Go:   // 手写递归
来源：http://hz.ybcxt.top/gtpndjgjyy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenjidiqi.icu/gtjcjfmukz.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtfhpnwiro.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.havefunace.top/gtcgjvnjoj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gthgieznee.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gttktnrqqo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtgshpzuhb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtuipdkuif.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtnimnwnxi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtgrnhrtbs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtcfipnisy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtteddpmfm.html

================================================================================
来源：http://hz.dianchejie.cn/gtcnxutcpw.html

O. 并发与异步
来源：http://hz.daxiang520.top/gtaeqqzdtx.html

================================================================================
来源：http://hz.yonumen.top/gtnrefgagl.html

[O01] 启动一个线程
来源：http://hz.chenlongwang.top/gtabluwhtu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zycfv.cn/gtuedkjbfn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtgtpbyric.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtswpwofpu.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtufkwmotb.html

Java: new Thread(() -> f()).start()
来源：http://hz.yueranfly.top/gtveicqxjd.html

Go:   go f()
来源：http://hz.zycfv.cn/gtpbenfdqv.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtggqszrku.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtatobpeak.html

[O02] 使用线程池
来源：http://hz.c1oappe.top/gtiqodckgj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aibaodan.cn/gtvhdvrrjb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tianlin.xyz/gtjiuvxbhl.html

JS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtraejclsi.html

TS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gtfnlipsdt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtcmsoxjom.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtnnzptxzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtcfpsizwi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.svipenyu.cn/gtuivgmbnh.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtipsmnaie.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtomaaaxrv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xinyue.icu/gtizgubbyq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtcvwhxibp.html

TS:   // 同 JS
来源：http://hz.52xcode.cn/gtvwcxbfwc.html

Java: synchronized (this) { shared++; }
来源：http://hz.gzhubu.top/gtahepbktu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtiuwtjcxc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.fengsongda.top/gthxjhnutw.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxinkj.top/gtilvymysv.html

[O04] 定义异步函数并等待
来源：http://hz.yuanzhike.top/gtyslfzqmb.html

Py:   async def f():⏎    await g()
来源：http://hz.aizwys.cn/gtviiplmxv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gttgdeukip.html

JS:   async function f() { await g(); }
来源：http://hz.316326.xyz/gtsoznzpbm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.316326.xyz/gtnkvsqdsq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtjkmwqdsh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gtkrsyjjlf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnqzz.top/gtcqoqkyut.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtkwcvgcij.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtujieqyjs.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtnizatcjj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenzaomai.com/gttwrklhll.html

JS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gtiiyeqtyx.html

TS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtcvquvfal.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gaohongyu789.top/gtgixkpqoe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aizwys.cn/gtscnedidd.html

Ruby: threads.map(&:join)
来源：http://hz.fzhhl.top/gtzvugjilv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangdashe.top/gtjnvtocjz.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtexefgnwc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtawwhkyti.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cqqwz.cn/gtkoezvgyz.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtycabzzdj.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtdkcnaakd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hnxiangtu.top/gtpdadmqdg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenzaomai.com/gtukkzxxce.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtprycotrd.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gtcwfhgbdw.html

================================================================================
来源：http://hz.hywenlv.cn/gtwermaxbl.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtazdkrkac.html

================================================================================
来源：http://hz.sxryk.cn/gtzqndaaab.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangtech.top/gtnatiiupl.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtwplgkapm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtclbcepzl.html

JS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtpdrueicn.html

TS:   crypto.randomUUID()
来源：http://hz.316326.xyz/gtvxhehujl.html

Java: UUID.randomUUID().toString()
来源：http://hz.gotoacloud.top/gtbqzknhhr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtcompstyp.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgfzy.top/gtprwnxhfh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258888.top/gttpcyzoih.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gtzitkvsby.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtthajkgrc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtfnwgjelk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtagriadhp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fengsongda.top/gtefanorka.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tian-w.cn/gtummiaolp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fzhhl.top/gtvcsutoxh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258888.top/gtsqlvegaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gtrrtpqkte.html

[P03] 生成短随机字符串
来源：http://hz.jiagoushi.top/gtrufqoxfo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtzqpihqhu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtpzguaure.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtanjkqghi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtymnyftvm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtbbtvvkit.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhixingplan.top/gtexdjpjqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtzougqscd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtakflozez.html

[P04] 求长度
来源：http://hz.haohaochexian.top/gtuyvgtexi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtrzfoxcrg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xziqi.cn/gtomsrilwk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtlxagtihc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guowangkeji.top/gtssljagaf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtcxrvirej.html

Go:   len(arr);  len(m)
来源：http://hz.meibo888.top/gtntizxcfp.html

Ruby: x.length;  x.size
来源：http://hz.yongpay.top/gtwgnfvoqa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtndmdqcis.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gtchkxymtn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhongyouzk.top/gtmddaivex.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yonumen.top/gtqximqoot.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtquscihmk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sysykeji.top/gteqkanbxc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gtkhqwuill.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtvcqrnnph.html

Ruby: a == b
来源：http://hz.yj20258888.top/gtohwssdgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtjggmixmd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuanzhike.top/gtjngdwpra.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cdnleiting.top/gtotqighrg.html

PHP:  if (empty($x)) {}
来源：http://hz.pycfn.com/gtcfydlvch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtcbehzstp.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtlxageyid.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtizaqakzn.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtvgkpicav.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtxvmwoafh.html

C#:   if (x is null) {}
来源：http://hz.zhaomingkeji.xyz/gtggwlxizp.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtdjtogbcm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gttzmsinqo.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtvarpthzx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtgnokazxm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtharsgbnm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtauprhbhu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtqpnhescj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.9152youxi.cn/gtkuoxgmwj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zdqjudy.top/gtupupqvbw.html

[P08] 处理浮点精度问题
来源：http://hz.hysaishi.cn/gtbuepoouv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dashuyun.cn/gtjjhtctke.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hongshengwenyu.top/gtotwqcuhx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.haohaochexian.top/gtuunvuown.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtyrckjxim.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gtpihsppeq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shanyushiyangkeji.top/gtrvwhuoka.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtpexqjoes.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gotoacloud.top/gtbrxsossg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpyswaljp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.snrcjt.cn/gtcidkoufv.html

================================================================================
来源：http://hz.guannengcc.top/gtwvhedxhf.html

[Q01] 创建表
来源：http://hz.zhijiandao.cn/gtfkbmygjm.html

CREATE TABLE users (
来源：http://hz.gotoacloud.top/gtskkwtbso.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtvxknmoav.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xziqi.cn/gtiaeztdee.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shangyingyoupin.top/gtbsawbzsm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fengsongda.top/gtagwbgvcy.html

);
来源：http://hz.hammf.cn/gtcgbliywk.html

[Q02] 创建带外键的表
来源：http://hz.daxiang520.top/gtrvzwdtdc.html

CREATE TABLE orders (
来源：http://hz.xinyue.icu/gtwukwoqfo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtysxuiali.html

user_id INT NOT NULL,
来源：http://hz.yanxiufei.cn/gtknrkavrn.html

amount DECIMAL(10, 2),
来源：http://hz.zhaomingkeji.xyz/gtyclxqxig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.0kj1m.cn/gtuvpffegc.html

);
来源：http://hz.shuidangran.top/gtgdzuddpz.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtbnkqladv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinyuanbaomall.cn/gtgcckvynf.html

[Q04] 修改列类型
来源：http://hz.cheryme.top/gtztazdvpr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.dianchejie.cn/gtuboyfksy.html

[Q05] 重命名列
来源：http://hz.hfpthk.cn/gtxhfsvdms.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangdashe.top/gtjkvqwcds.html

[Q06] 删除列
来源：http://hz.xziqi.cn/gtrffzshmx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.mhx1999.top/gtqawdziqk.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtlegqyjjf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtlkmdykui.html

[Q08] 创建普通索引
来源：http://hz.feifeiyinyue.top/gtjcggvdxp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtowxtjzff.html

[Q09] 创建唯一索引
来源：http://hz.fzhhl.top/gtviatnaqd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtffizgldv.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtydpndfei.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgfzy.top/gtvtkgtgur.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtpyaecmtf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtijilqprp.html

[Q12] 插入后取自增 ID
来源：http://hz.wangdashe.top/gtxdzxqlbm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigufen.top/gtdpyjwtyw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtlqlnmzmy.html

[Q13] 忽略重复插入
来源：http://hz.yuxming.cn/gtzdufqlrd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gthmhrjnjt.html

[Q14] 存在则更新（upsert）
来源：http://hz.sweek.top/gtjyxnkifx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtvkwqwafx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sweek.top/gtkirxmbcf.html

[Q15] 查询全部
来源：http://hz.chenzaomai.com/gteqceeztz.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gttxiufvdy.html

[Q16] 查询指定列
来源：http://hz.yuanzhike.top/gtbbbcomaj.html

SELECT id, name FROM users;
来源：http://hz.cashguo.top/gthtwaygpb.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtnkfayawc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shangyingyoupin.top/gtgfzrsiap.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtoiguwlvb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gtgxbgxncx.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtbjwwukfq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtagernnfy.html

[Q20] IN 列表
来源：http://hz.yuxming.cn/gtcfhqofcd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gaohongyu789.top/gttxmhzbmx.html

[Q21] 空值判断
来源：http://hz.andypj.xyz/gtbusxcjty.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.pengpengdd.cyou/gtumrprkqa.html

[Q22] 排序
来源：http://hz.xuanzx.com/gthfbtqmwi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinghuilouyu.cn/gtsfzuigqt.html

[Q23] 分页
来源：http://hz.jianghu66.top/gtawylpmlk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtpycboyhh.html

[Q24] 去重
来源：http://hz.yj202588.top/gtjbeqszox.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gthwblmfav.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtzmuzyfaq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtkqgkhcpy.html

[Q26] 计数
来源：http://hz.jianghu66.top/gthuqbzejj.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtegbmseuo.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtryshyhvf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtyrckriqx.html

[Q28] 求和与平均
来源：http://hz.jinqigfzy.top/gtjcelnmbo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ydjk.org.cn/gthmzsjfwq.html

[Q29] 最大最小值
来源：http://hz.yanxiufei.cn/gtoojvgsfx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtalrbfzbe.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtwrvwhvpe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtsivfjnbn.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtsjhfvjoy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtvxzetwvq.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtgnqplypk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gtvjsmyjff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ehwqpu.com/gtediqtukf.html


<!-- 参考信息 -->