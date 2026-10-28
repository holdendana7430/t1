代发 wailian999

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtlwgzetoe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtymdewmpj.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gturbwznxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pengpengdd.cyou/gthtqgbfzn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daria6918.cn/gtwtyzycyu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtjgzglctg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtsfmoqgue.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtqyykrzkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtedzqxxwq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gttocqpged.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gttzimtjah.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtvigmgryn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtyqbxsltb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtzhoeatlp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtyfiaihhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtpcyrcyha.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydzc1.top/gtnophitmc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtvrkxfjtu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtddgizqks.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangdashe.top/gtkvbipzsq.html

[N05] 最大公约数
来源：http://hz.dashuyun.cn/gtpmeakgoa.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtrnwudllv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtdmpbzbnu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtcrrpnvtg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gthkqzxkjc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtgdotjugb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jianghu66.top/gtmhutklwu.html

Ruby: a.gcd(b)
来源：http://hz.fengsongda.top/gtcnypdtcl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gtsfzqeweb.html

[N06] 判断回文字符串
来源：http://hz.gotoacloud.top/gtlzxqlgkr.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gthcaaqxob.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtysudewip.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtqypaquoy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtojbxkyto.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtcfpdfnoh.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gtouspytyr.html

Ruby: s == s.reverse
来源：http://hz.sweek.top/gthuigdkrb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gttbnvntpg.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gttcbfeuco.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gtfksnrnjc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhixingplan.top/gtlnguyuzp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtbaqmxpjm.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtbtudbjhe.html

Java: // 手写 HashMap
来源：http://hz.xinyue.icu/gtmqgevomk.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gtywrmjfhv.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtjfdtjopv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gttqbsjhmx.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtcaetdhwq.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtyjouzgxf.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gteezwtumk.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtrpfegpco.html

TS:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtuxovslyp.html

Java: // 手写回溯递归
来源：http://hz.jyoumei.cn/gtbzgxcnbu.html

Go:   // 手写回溯递归
来源：http://hz.ivvv.top/gttfzdsdsf.html

Ruby: arr.permutation.to_a
来源：http://hz.xuanzx.com/gtuajbxvor.html

C#:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtxgoltucs.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtkzinmwjv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtngawuhse.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtjvmmpmsc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtlbsfztaq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtkodpbskk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gtylajrasc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtntalmwtx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtvercqvql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.kuanghao11.cn/gtqtlofrcb.html

[N10] 链表节点定义
来源：http://hz.dashuyun.cn/gtesviiiuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigfzy.top/gtwxvvidtd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtuivbranm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gtydpgetvk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgufenzy.top/gtvaijzhpr.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtybmvvcir.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gthheehgbg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtbqkqrpfc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dianchejie.cn/gtfnqgvefl.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtvpqtdmef.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhongyouzk.top/gtlgxhwymr.html

PHP:  // 手写递归函数
来源：http://hz.zhiwuduotai.top/gtjzsmaqhw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigfzy.top/gtjjjvaxad.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtvtehtgnp.html

Java: // 手写递归
来源：http://hz.quarkkingdee.top/gtaqlsdprk.html

Go:   // 手写递归
来源：http://hz.sysykeji.top/gtbxephmzx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gtbutvophw.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtgjeendnk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gtijhmojau.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtqqiuljfc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gtyazkhdwf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtktnbrvdc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtfhewwwaz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gttghhrhwp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gttgyngncj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sxryk.cn/gtdeoqfnly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtlefypfay.html

================================================================================
来源：http://hz.wangdashe.top/gtumpymirq.html

O. 并发与异步
来源：http://hz.andypj.xyz/gtmsymxdry.html

================================================================================
来源：http://hz.gzhubu.top/gtyphjikui.html

[O01] 启动一个线程
来源：http://hz.pycfn.com/gtdpmjpvdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gtwckvixpj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtqlwohgzy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhaomingkeji.xyz/gtmrnolfvo.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtlkbdewhi.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtmlhudwav.html

Go:   go f()
来源：http://hz.hfpthk.cn/gtyxcmryvr.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtbqvvsrxh.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gthsqbiqeh.html

[O02] 使用线程池
来源：http://hz.yonumen.top/gtdxuuegkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhoulong.xyz/gtzuzwuiel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtsvadprrf.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtxlhtijpo.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtmbruwsso.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtfwopgcou.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.52xcode.cn/gtwtsppvdo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gtpddlebth.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gteloemcpf.html

[O03] 加锁保护共享数据
来源：http://hz.jyoumei.cn/gttrcpilrf.html

Py:   with lock: shared += 1
来源：http://hz.yangfankeji.com/gtdlfaysej.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tian-w.cn/gtclrsubnw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yonumen.top/gtjxmtmmyi.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtkepcfhyd.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtswlprqje.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtvnqulqlr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtvtwyvrxj.html

C#:   lock (gate) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtpwcincvv.html

[O04] 定义异步函数并等待
来源：http://hz.cdnleiting.top/gtwshpgxlw.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtlafbxrtv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ydzc1.top/gtptvhrpeq.html

JS:   async function f() { await g(); }
来源：http://hz.xylfe.cn/gtnelqqvkp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtptchkucu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gtpjfpsgts.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuanzx.com/gthhogqvop.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtlooairhu.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gtrhtepbxu.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtklxhjpmn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtcvhkexfp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtdrynzlsg.html

JS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtjhpyegky.html

TS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtbmimkwcu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuanzx.com/gtekqnuilf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtomiapfyb.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtpepyoxsi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gtqohhiguz.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtzpnncedd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtctnitasa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gteayiemqo.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtfwzprftq.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtfedmyrpy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gteabonkyd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtxwnamuqm.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtykbunbhf.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtxhiupehd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbqbibtpc.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gtxtjneyor.html

================================================================================
来源：http://hz.dianchejie.cn/gtgnodlmkt.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtqwkxcuht.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gthfhablpj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gttngkjjwj.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtwgiwiwvu.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtmwdymkry.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtontpepup.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ehwqpu.com/gtoxdpajuj.html

Ruby: SecureRandom.uuid
来源：http://hz.0kj1m.cn/gtoopvwqou.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shangyingyoupin.top/gtixxzwyva.html

[P02] MD5 / SHA256 摘要
来源：http://hz.0kj1m.cn/gtpiedpeyj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pengpengdd.cyou/gtztvidhbq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtqmielvhk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.bjfxy.top/gtkkwmtaxk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtzgffjcfm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yvedp.cn/gtpuhwvfkd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtweeesirl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtbnpzlyld.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgufenzy.top/gtimsztlme.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtrsacqgpo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtmroiwbgm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtffmraofa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtmgouglbb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xziqi.cn/gtgjdarkht.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jqgfzy.top/gtyaeqwsxq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtayrsduoi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cashguo.top/gtlvcifukl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtetrkizih.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtuebimido.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtjgouoaej.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtzhnapxbq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtulwghouj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtfdwaqwqb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtepedpqtu.html

Go:   len(arr);  len(m)
来源：http://hz.zhaomingkeji.xyz/gttshwwgtl.html

Ruby: x.length;  x.size
来源：http://hz.shangyingyoupin.top/gtawbndamu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.c1oappe.top/gtvfaswgpf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gtakutscyq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigfzy.top/gthaadhgnv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtekigdmdv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ywan-chungtsiang.top/gtlhgyddgr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtufrpsjjz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtygyarurt.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yj20258888.top/gtrdoaxdwh.html

Ruby: a == b
来源：http://hz.0kj1m.cn/gtnijedmjz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gtblhnipds.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtbkurpvvk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dianchejie.cn/gtxcxygwex.html

PHP:  if (empty($x)) {}
来源：http://hz.yj20258888.top/gtwxlvgnxn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtfmgsyfsz.html

TS:   if (x == null) {}
来源：http://hz.pengpengdd.cyou/gtvgangbyf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtscgiyjqk.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtvzzowhcp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xylfe.cn/gtnxvvrjww.html

C#:   if (x is null) {}
来源：http://hz.ybcxt.top/gtldbfxhsi.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gtpxzvevyl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenlongwang.top/gtytlenvva.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtinqpohsl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtlltwavft.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtiaqwnued.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtvoalmlmk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yuxming.cn/gtqenohuwj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtonwdmkzs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gteyxophoa.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtaazncjpl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtpfiqkhng.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtnbnggcfq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtnvldzhyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yangfankeji.com/gteahbelhr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.daria6918.cn/gthmbqrisf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhijiandao.cn/gtnushfodr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gtluficfjk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.iojbl.cn/gtekpwrnap.html

================================================================================
来源：http://hz.wangdashe.top/gtuvqonmqm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gthkszeonq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtikokwfix.html

[Q01] 创建表
来源：http://hz.quarkkingdee.top/gtaooppmew.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gttvgmkvek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gttdidqufr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hfpthk.cn/gtrhxakrnd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnxiangtu.top/gtgibopqci.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.nanxuanxn.top/gtpxnpprqh.html

);
来源：http://hz.tianlin.xyz/gtdnixinxr.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtzcftyqqv.html

CREATE TABLE orders (
来源：http://hz.sysykeji.top/gthhfmropi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gtsojcrwhb.html

user_id INT NOT NULL,
来源：http://hz.gogol.net.cn/gtaxjwsotw.html

amount DECIMAL(10, 2),
来源：http://hz.hywenlv.cn/gttehnvfbr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.smart0.xyz/gtklzwlokn.html

);
来源：http://hz.xylfe.cn/gtqnveqtjs.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtnefqzyjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jiagoushi.top/gtnebdrngu.html

[Q04] 修改列类型
来源：http://hz.wangdashe.top/gtlbdeywiy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtctaxsjbb.html

[Q05] 重命名列
来源：http://hz.nwbrower.top/gtfjlajrup.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gtbqlzzdtn.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtalgweqnc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtjblpxqdp.html

[Q07] 删除表
来源：http://hz.yueranfly.top/gtmpwjrfad.html

DROP TABLE IF EXISTS orders;
来源：http://hz.kuanghao11.cn/gtyfzqpbtt.html

[Q08] 创建普通索引
来源：http://hz.hysaishi.cn/gtpevumjef.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtgdkpgelm.html

[Q09] 创建唯一索引
来源：http://hz.dashuyun.cn/gtqmryiwgp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tanke756.top/gtgxtklfzp.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtvyoloddp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtdmpnesbs.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtdumtbtfg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aizwys.cn/gtjhmvsrkn.html

[Q12] 插入后取自增 ID
来源：http://hz.cucudq.cn/gtsvwvhalo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gtklvlirwh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtxeuqlsxg.html

[Q13] 忽略重复插入
来源：http://hz.wangdashe.top/gtducnpdnb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtihurjpvr.html

[Q14] 存在则更新（upsert）
来源：http://hz.smart0.xyz/gtnbntvvho.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtiwgiwxeo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gtgcrnnsfx.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gthsuapcjq.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtuyomdxdj.html

[Q16] 查询指定列
来源：http://hz.guannengcc.top/gtlqwepkkv.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtwomzkvib.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtyhoqztix.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj202588.top/gtxsqvxoxw.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gteujagjfb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gtfveoylpz.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtxmgfvufi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.pycfn.com/gtnyhxsuna.html

[Q20] IN 列表
来源：http://hz.c1oappe.top/gtxvakrrhq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtscajavrs.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtfxvizugt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtolnauqnm.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtienjphyb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtuwhdcvac.html

[Q23] 分页
来源：http://hz.jqgufenzy.top/gtaxdohcms.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxinkj.top/gteulisjhn.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtxdtegmnq.html

SELECT DISTINCT city FROM users;
来源：http://hz.cashguo.top/gtckzudpej.html

[Q25] 只取前 N 条
来源：http://hz.xuetiantiany.cn/gtaugntyid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhijiandao.cn/gtotfteexj.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtzhdtxode.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtdyjxjlhi.html

[Q27] 条件计数
来源：http://hz.snrcjt.cn/gtgjorxjnz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dashuyun.cn/gtmtfwipji.html

[Q28] 求和与平均
来源：http://hz.quarkkingdee.top/gtmyjulonx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gotoacloud.top/gtbykhauhk.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtmyycgxor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtshxblqem.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtxzhvzlwi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gteywdsuqm.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtivgimhud.html


<!-- 参考信息 -->