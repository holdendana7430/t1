代发 wailian999

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtdojrahaq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhengqikj.top/gtibyrzdct.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtarhnmfzz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangdashe.top/gttodztwds.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtyrfceutf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtujavnagu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtcepeydre.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtoahaukhq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gthzgutkhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gtvzxifhab.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtyspppkbh.html

[N04] 斐波那契数列
来源：http://hz.feifeiyinyue.top/gtfaueldvt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtweibkzzd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.kuanghao11.cn/gtkbvzjede.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtxstikgvv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtdaebqfgd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtsbosohwm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtjakizbhn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtogjmhsdj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtfaxnkrqj.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtednncaqs.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtqwmnhfkl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtdbulkbsi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtkuvixqrp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtkopcjzor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtjrzevpyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtducdvcop.html

Ruby: a.gcd(b)
来源：http://hz.haohaochexian.top/gtzahubxmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gtkwxrxhku.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gttodpblqc.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtwwmqkrrw.html

PHP:  $s === strrev($s);
来源：http://hz.bjfxy.top/gtnccjbydm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtkdafrgxt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtjwtkkixx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtpyqaumjt.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtpfjdnjoq.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtvvgpzgxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtsbgdwjnm.html

[N07] 两数之和（返回下标）
来源：http://hz.0kj1m.cn/gtozhdrpbs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258888.top/gtobtrupgw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sufxvd.cn/gtistnbflo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtpvbqsxnt.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxuanxn.top/gthprpvmfd.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtutmetkjz.html

Go:   // 手写 map[int]int
来源：http://hz.tian-w.cn/gtgmyfuawe.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtlrzwdvqq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gtstbfogoi.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtoygpuejg.html

Py:   itertools.permutations(arr)
来源：http://hz.xylfe.cn/gtfmzuszpy.html

PHP:  // 手写递归交换
来源：http://hz.redwolf501.top/gtkghtpfoq.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtcmubrujy.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtywopjquq.html

Java: // 手写回溯递归
来源：http://hz.sxryk.cn/gtgeefmzjh.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gtyplovppq.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtpfkkswef.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtbuhubsdv.html

[N09] 栈与队列
来源：http://hz.daria6918.cn/gtyuwcepdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhiwuduotai.top/gtfncxsgmw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtalwerqbt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yvedp.cn/gttmniwshb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.iojbl.cn/gtotozmiet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xylfe.cn/gtipzmcmgv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xylfe.cn/gthmgwxjep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigufen.top/gttoypimua.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtsbqndymh.html

[N10] 链表节点定义
来源：http://hz.nwbrower.top/gthbhqkhpv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhiwuduotai.top/gttmroehfs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtgiwdsgfz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtvhmyjkkp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtyqqyzbjz.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtbcrnijbj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.0kj1m.cn/gtnsisbkzn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtqkyhabti.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtynqjrfcu.html

[N11] 二叉树中序遍历
来源：http://hz.vqdsnc.cn/gtohyhzhzc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtrbeoynbn.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtamsfwvyp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtvqmvnkce.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtkxudgwjj.html

Java: // 手写递归
来源：http://hz.hnxiangtu.top/gtoosduryp.html

Go:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtyftzwdse.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shangyingyoupin.top/gtmnvntyiz.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtwvfslnto.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ppjwa.cn/gtylnkjcva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtqwopwneb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nanxinkj.top/gtftqixptu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtshvmdurf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtipqsqkzi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtqjdryrih.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtamepqrvx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenjidiqi.icu/gtfkfbuqzb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhijiandao.cn/gtsfrfvkol.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfcmiqycz.html

O. 并发与异步
来源：http://hz.svipenyu.cn/gtueprqmyt.html

================================================================================
来源：http://hz.tian-w.cn/gtwaoyavhf.html

[O01] 启动一个线程
来源：http://hz.wangdashe.top/gtpiplyxyl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gthnzvhvxi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cdnleiting.top/gtswlgpjdc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtmijpinni.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtfmdpklvu.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtdfbaonxl.html

Go:   go f()
来源：http://hz.zhaomingkeji.xyz/gtljwnqhrv.html

Ruby: Thread.new { f }
来源：http://hz.zycfv.cn/gtnvpexqpb.html

C#:   Task.Run(() => F());
来源：http://hz.jianghu66.top/gtnpeqsisq.html

[O02] 使用线程池
来源：http://hz.yonumen.top/gthekokdvk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.birdmap.top/gtixkkouir.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenlongwang.top/gthdelvfad.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtynglmvrv.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtbeoatfab.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtjmvrpqxw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtkybgbrfo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinghuilouyu.cn/gtmajrbmou.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ybcxt.top/gtgibbgirg.html

[O03] 加锁保护共享数据
来源：http://hz.nanxinkj.top/gtbejqygni.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtmkdbehse.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shuidangran.top/gtkohcdiyu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gtehgnbjbu.html

TS:   // 同 JS
来源：http://hz.jiagoushi.top/gtupfhpzah.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gtlousztra.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtwbjtgrog.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shangyingyoupin.top/gtgkxqobke.html

C#:   lock (gate) { shared++; }
来源：http://hz.yueranfly.top/gtktpgnexo.html

[O04] 定义异步函数并等待
来源：http://hz.tianlin.xyz/gtzqhtbhbt.html

Py:   async def f():⏎    await g()
来源：http://hz.pengpengdd.cyou/gthpbswdhb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtzdkszqhs.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtiulomnds.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.guannengcc.top/gtqjmljiml.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtjluaeghk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtrsifrkjm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtlsbpenlo.html

C#:   async Task F() { await G(); }
来源：http://hz.fzhhl.top/gtdsnbrbeb.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gtbkpplvtw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtyuzrxyid.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtjtoxkinp.html

JS:   await Promise.all(tasks)
来源：http://hz.iojbl.cn/gtssmhfjnp.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtbcclkyjs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtvpsraqhf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtgdjwekgl.html

Ruby: threads.map(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtzejizdny.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gaohongyu789.top/gtyxkabiap.html

[O06] 使用进程池
来源：http://hz.smart0.xyz/gtmvciitsg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhengqikj.top/gttwtnufiu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fengsongda.top/gtridigqhn.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtkiokpvzj.html

TS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtmeivbgcj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtnnxpjzmc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtflefrzse.html

Ruby: // fork 块
来源：http://hz.yj202588.top/gttgvuwxhs.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtcpnsctbm.html

================================================================================
来源：http://hz.jqgfzy.top/gtoauljexh.html

P. 常用工具函数
来源：http://hz.hnqzz.top/gtoicpatfx.html

================================================================================
来源：http://hz.yuxming.cn/gtnqvouzjg.html

[P01] 生成 UUID
来源：http://hz.yuanzhike.top/gtpbhuzzzc.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtjlvqlpic.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yonumen.top/gthmcrbltp.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtzbmzxvyq.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtevrkuypa.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtlugcjttt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daria6918.cn/gtljecaysv.html

Ruby: SecureRandom.uuid
来源：http://hz.sweek.top/gtubtqoblq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhongyouzk.top/gtyhcpehlz.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtljrxfuhm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.bjfxy.top/gtcwaqgrvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtgfnftnzd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sufxvd.cn/gtesbiubuw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtciqkinty.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.andypj.xyz/gtcjmghhkx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtfxefqldj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cheryme.top/gthnkpazif.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tianlin.xyz/gtlxxsfghs.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtbzxuvmxg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtlzrkurnq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtcttfedip.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gthxsrclbt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtdknerapq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtrbsvanoq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtwljmnvme.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gtxjjimfnx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtwdfmethi.html

[P04] 求长度
来源：http://hz.ivvv.top/gtzvmzkocs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtwbyzlfdp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtmwyucaqz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtmimannnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtxqqtzube.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtgpprftfv.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtnpbipxts.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtowfloaao.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.guowangkeji.top/gtawdpxshl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxinkj.top/gtojwupmlb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dashuyun.cn/gtetfnvwon.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.kuanghao11.cn/gtipejdsmu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xziqi.cn/gtornzyvei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gthepmxxtz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cucudq.cn/gtviftqxot.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtwawwmrwi.html

Ruby: a == b
来源：http://hz.meibo888.top/gtikvrbvpx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gttggajumn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ywan-chungtsiang.top/gtgdwjypzr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtrlostskq.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtwdgzorlr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtdxgtkdkw.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtosmqxvfo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sweek.top/gtuquaefjc.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtepmozilv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hysaishi.cn/gtgyfclhul.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtnkqfkcka.html

[P07] 防抖与节流
来源：http://hz.sxryk.cn/gtmsrsxcmi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daria6918.cn/gtcjwxvukq.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtkynywemh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xinyue.icu/gtozcapjsj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jyoumei.cn/gtqivgpplm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj202588.top/gtsfknzemp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tianlin.xyz/gtomsnrawt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hammf.cn/gtvrxyqkua.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhijiandao.cn/gtlyxiflwr.html

[P08] 处理浮点精度问题
来源：http://hz.sysykeji.top/gtnahyxhxn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hongshengwenyu.top/gtwkoblbey.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gtehgtkkvl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtpgwvwnsa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtlurfeckz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtwvjpylof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.0kj1m.cn/gtdbarjunb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtusohjtfo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtlurehwvs.html

================================================================================
来源：http://hz.shuidangran.top/gtzncjoptx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtqsnbvlpm.html

================================================================================
来源：http://hz.hfpthk.cn/gttwaevneo.html

[Q01] 创建表
来源：http://hz.gogol.net.cn/gtsvabuowz.html

CREATE TABLE users (
来源：http://hz.nanxuanxn.top/gtqkvkvdbs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtaqrgvebo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.feifeiyinyue.top/gtqzottcpi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtybtgzrji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sweek.top/gtbasdtodg.html

);
来源：http://hz.jiagoushi.top/gtmthjyysv.html

[Q02] 创建带外键的表
来源：http://hz.ivvv.top/gtmqfnbdhx.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtugmneryu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtkhuzrjww.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gtstfadhkv.html

amount DECIMAL(10, 2),
来源：http://hz.tian-w.cn/gtkyssudwm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jianghu66.top/gtduiwzzng.html

);
来源：http://hz.redwolf501.top/gtfjugwrjl.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtybqrpudw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.dashuyun.cn/gtxzfopydh.html

[Q04] 修改列类型
来源：http://hz.mhx1999.top/gtutomrgmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gtqwogbdrb.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtyoupjsok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhongyouzk.top/gtujltyqak.html

[Q06] 删除列
来源：http://hz.svipenyu.cn/gttujkxjcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtclkyoerk.html

[Q07] 删除表
来源：http://hz.yongpay.top/gtuwmocjal.html

DROP TABLE IF EXISTS orders;
来源：http://hz.iojbl.cn/gtetsmtbtt.html

[Q08] 创建普通索引
来源：http://hz.nwbrower.top/gtwxtgzytb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigfzy.top/gtrrvrbqas.html

[Q09] 创建唯一索引
来源：http://hz.iojbl.cn/gtefspyqyt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shzxlz.cn/gttsegncmc.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtckldhwkk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.iojbl.cn/gtgrioctah.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtzcjcezjl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtoqbxceju.html

[Q12] 插入后取自增 ID
来源：http://hz.aibaodan.cn/gtyfjldlnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yj20258888.top/gtovpeuxgx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenzaomai.com/gtmbmhxrpb.html

[Q13] 忽略重复插入
来源：http://hz.yj20258888.top/gtbvydxypu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gotoacloud.top/gtxwdxfdst.html

[Q14] 存在则更新（upsert）
来源：http://hz.shzxlz.cn/gtcxnrfyee.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jlsjyb.cn/gtqhtayxyd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guannengcc.top/gtlsixmjhq.html

[Q15] 查询全部
来源：http://hz.zhongyouzk.top/gtbajtcaec.html

SELECT * FROM users;
来源：http://hz.xuetiantiany.cn/gtdbrfisyj.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtalajgtvb.html

SELECT id, name FROM users;
来源：http://hz.quarkkingdee.top/gtsfaqadcf.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gthckbtgws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sxryk.cn/gtrhdlbfnn.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtgghbazzk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gtimhsasfd.html

[Q19] 范围查询
来源：http://hz.sxryk.cn/gtjdxgaisa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtdofvxlxp.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtqjwadygz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtzrmhpehd.html

[Q21] 空值判断
来源：http://hz.0kj1m.cn/gtugpcwpah.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cashguo.top/gtokwhxoks.html

[Q22] 排序
来源：http://hz.yonumen.top/gtskobtinb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangdashe.top/gtzjblacjg.html

[Q23] 分页
来源：http://hz.jqgufenzy.top/gtndunoiid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtpvdsqlka.html

[Q24] 去重
来源：http://hz.nanxinkj.top/gttxoasfsi.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gttqtmqhmp.html

[Q25] 只取前 N 条
来源：http://hz.redwolf501.top/gtpcesicfl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gthlegimdq.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtnhqwilkj.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtzchayytx.html

[Q27] 条件计数
来源：http://hz.vqdsnc.cn/gtcdusvykq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gtfcxvqpwc.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtfguwbmey.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtgkoeowgq.html

[Q29] 最大最小值
来源：http://hz.hfpthk.cn/gtwghovwil.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtskablabo.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtosuzigbv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtshfmsxyv.html

[Q31] 分组后过滤
来源：http://hz.xuanzx.com/gtyrlphcmh.html


<!-- 参考信息 -->