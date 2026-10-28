代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtsvhrcwiu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtrjvpppyy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtskkrvzzc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtabrybbvn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gtaezrgfck.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtgfjigpkg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtiftmlsse.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtjdaaeclr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtgtealkle.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gttiuxqzcf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gtqipkfblr.html

Go:   slices.Sort(arr)
来源：http://hz.ppjwa.cn/gtfphqlvwp.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtkcanlvzo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.kuanghao11.cn/gtyagcbpdz.html

[N03] 快速排序（分治示例）
来源：http://hz.nwbrower.top/gtcuhqrpno.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xingfuxueyuan.xyz/gtntguetto.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jyoumei.cn/gtssdhgvwt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtfcxeorru.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtjpazoaqj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.redwolf501.top/gtcutrfhpo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtkcbgidcy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangkeji.top/gtbqqmqrpj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtsabldqhu.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gthixxxjrp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtwmmeyayq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtsyoxjfcl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gteefletpv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gttxohhrih.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gtcvjhgefj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtrfnpsvae.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gtornnjqsb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nwbrower.top/gtorhvsiky.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gthmzlpkps.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtrmvzvqau.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.c1oappe.top/gtufoezqbf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtmuthtcou.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtenfifffj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtsqfkvayb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dianchejie.cn/gtsjshxviy.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtgadcsufd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gtmsnfhhbh.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtvzrijcxo.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtbrgoqqwr.html

PHP:  $s === strrev($s);
来源：http://hz.shzxlz.cn/gtiwtlnahf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtgeeaxwqv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtpwijrmre.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtdnemkcqy.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtpqgiunrq.html

Ruby: s == s.reverse
来源：http://hz.feifeiyinyue.top/gtqnmtkktx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtbfwbinrs.html

[N07] 两数之和（返回下标）
来源：http://hz.haohaochexian.top/gtffhotksg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtudkteaze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtjrxbvdbx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhongyouzk.top/gthycbwzip.html

TS:   // 手写 Map<string, number>
来源：http://hz.ybcxt.top/gthledsrce.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtcslamwee.html

Go:   // 手写 map[int]int
来源：http://hz.pycfn.com/gtqbnemfmk.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtqvvrhufl.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtzqemjwfc.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtjtusrimh.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gtrohopkje.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtnrstsjjp.html

JS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtotgkabqj.html

TS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtbkbbwzji.html

Java: // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtufazwdps.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtiuvomsjr.html

Ruby: arr.permutation.to_a
来源：http://hz.hywenlv.cn/gtihfcvkql.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtzfnypvjb.html

[N09] 栈与队列
来源：http://hz.vqdsnc.cn/gtytdjysfe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtvxejifjj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtupdvyhmi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtjjflgnsd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtkjdddkuj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nwbrower.top/gtbdahkidr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtzcfwvrih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtofpbnyca.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fzhhl.top/gtlegcpiot.html

[N10] 链表节点定义
来源：http://hz.sufxvd.cn/gthcmlungr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtonogmxfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtnbdylnoq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtpglzdviu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtldrnezpj.html

Java: class Node { int v; Node next; }
来源：http://hz.hysaishi.cn/gtsyctondc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenlongwang.top/gtxselqrpg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangkeji.top/gtbugwwvff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtrokqfuja.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtqvlnqupa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtzdlwefxb.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtfxziwoti.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gteihrpwgt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pycfn.com/gtpuloawzw.html

Java: // 手写递归
来源：http://hz.cdnleiting.top/gtmhprcndx.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtdnkpgmnq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gtolfoyjay.html

C#:   // 手写递归
来源：http://hz.tanke756.top/gtjojztihb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtezpvhluw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xziqi.cn/gtkkdxaxkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtzqrqedlo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtimsznzxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtprftmkba.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtusilmfrm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinyuanbaomall.cn/gtteymovzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtgealistv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gtlnelwctz.html

================================================================================
来源：http://hz.svipenyu.cn/gtnazatuxf.html

O. 并发与异步
来源：http://hz.yonumen.top/gtpkrjwsrl.html

================================================================================
来源：http://hz.gzhubu.top/gtuoilkahv.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtbsxkrdtf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guowangkeji.top/gtsqgrouxy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gtfbqpacee.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtvzhgkwsd.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gttpgokirb.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtgmggzwce.html

Go:   go f()
来源：http://hz.yonumen.top/gtxrdfjeqz.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtuowdakef.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gtsccwvkly.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtqiiafhlu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtpzizwiwi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtrqidvzsd.html

JS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtchximpco.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtgtohsbgx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuanzhike.top/gtwntiqdxp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtooxyvdpl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.kuanghao11.cn/gtnwbbilvv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtnzuhviez.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtgdzeshaf.html

Py:   with lock: shared += 1
来源：http://hz.aizwys.cn/gthxopvnjg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtmkewgign.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jlsjyb.cn/gtspkhkhai.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtobrffpxa.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtkxwiqbza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinyuanbaomall.cn/gtbeojglep.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydzc1.top/gtmsjkyahh.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtduifbjoe.html

[O04] 定义异步函数并等待
来源：http://hz.ywan-chungtsiang.top/gtyknnkfhs.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtnfiglijm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gtarpdntqy.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtucnzcaic.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtaxtpzttg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtluofzggz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cdnleiting.top/gtnsjfevbz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gttacuhimv.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtwyxcwpwv.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtdlgfbvwj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangdashe.top/gttuwvlhls.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtaoonmnis.html

JS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtjjyidzmj.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtevoetokw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtubxyuhzc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xinyue.icu/gtdfglqous.html

Ruby: threads.map(&:join)
来源：http://hz.nanxuanxn.top/gtfttnviga.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.316326.xyz/gtqwdhmulb.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtmabzsxdl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtetmxifua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tian-w.cn/gtjcouqisr.html

JS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtiwnvfdww.html

TS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtrlekrmev.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtuilckkzk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yongpay.top/gtqvdbmjxj.html

Ruby: // fork 块
来源：http://hz.cqqwz.cn/gtmzktfjdi.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gtbjdhiknt.html

================================================================================
来源：http://hz.zycfv.cn/gtwtlgxrtd.html

P. 常用工具函数
来源：http://hz.jqgufenzy.top/gtvqiwxhey.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtasttfati.html

[P01] 生成 UUID
来源：http://hz.zdqjudy.top/gtqdfemrps.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtblmqukln.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtkvsrykru.html

JS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtxmwgbbic.html

TS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtgoaglpjb.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtlqbkuafp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.mhx1999.top/gtdyyyvssk.html

Ruby: SecureRandom.uuid
来源：http://hz.kuanghao11.cn/gtopdvyolh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gtnwpveosn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.c1oappe.top/gtqrcqnzjw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtbwbzabbm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtuooalzap.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtdvejsuzo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtzmyestrl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtzqgkondj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zdqjudy.top/gtigbtvsxg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtzteaooyc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yonumen.top/gtngjzplcu.html

[P03] 生成短随机字符串
来源：http://hz.cdnleiting.top/gtwjifaeyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pengpengdd.cyou/gtgpwyncvu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtreadqgck.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gttdaejwva.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtghyayxck.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtkbyxgean.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ivvv.top/gtbmiofxml.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.snrcjt.cn/gtckadsjvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gtjzamzswq.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtmsioapva.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.bjfxy.top/gtqbsmjinr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtincendru.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtrbqqhkwn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtzgywjdlp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.52xcode.cn/gtbgtoupzd.html

Go:   len(arr);  len(m)
来源：http://hz.gotoacloud.top/gtpngioihi.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtqyfeyaki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuetiantiany.cn/gteuyejtwh.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shanyushiyangtech.top/gttqkihwkt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtayzdakhz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cdnleiting.top/gtgchwirsl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jyoumei.cn/gtibamusti.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtvyzewtoc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtgivnscni.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuanzx.com/gtcmqbokll.html

Ruby: a == b
来源：http://hz.cashguo.top/gthclnzxzn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtoymntbam.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtvbxljkee.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fzhhl.top/gtcwreyzct.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtlclapqov.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydzc1.top/gtrzfcgyde.html

TS:   if (x == null) {}
来源：http://hz.cheryme.top/gtgmjjudah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtuabrzywu.html

Go:   if x == nil {}
来源：http://hz.jiagoushi.top/gtsevmewql.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xinyue.icu/gthxtvkghj.html

C#:   if (x is null) {}
来源：http://hz.cqqwz.cn/gtzugiikvq.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtjgeshlix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hnxiangtu.top/gtnevpxcjt.html

PHP:  // 手写时间戳比较
来源：http://hz.sxryk.cn/gtgmddvrtd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtxbriqrdm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtivmmgpbv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuetiantiany.cn/gtolsggucr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gttoksqdtj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtschpqgns.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gttzshwruv.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtqnkrchyk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtmafsefmd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xuetiantiany.cn/gtvhmcrmal.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hammf.cn/gtrqhkiozh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cdnleiting.top/gtlmukalkv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtdjoamzxs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.9152youxi.cn/gtosmkovwa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuanzx.com/gtecudwhph.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jiagoushi.top/gtuftokmir.html

================================================================================
来源：http://hz.dashuyun.cn/gtdanxlajs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtmyqhnodx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqrtkmmdl.html

[Q01] 创建表
来源：http://hz.jlsjyb.cn/gtrmmhaaop.html

CREATE TABLE users (
来源：http://hz.gzhubu.top/gtqwkalbzm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtnqyxdkho.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtidnmghjo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtopfbuxeo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shuidangran.top/gtemvukgiq.html

);
来源：http://hz.cucudq.cn/gtirmqqfgb.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtutqlnjod.html

CREATE TABLE orders (
来源：http://hz.mhx1999.top/gtzrxdfuvj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gttvhgzvio.html

user_id INT NOT NULL,
来源：http://hz.gzhubu.top/gtrgkgphrn.html

amount DECIMAL(10, 2),
来源：http://hz.zhoulong.xyz/gtrlfydukg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinyuanbaomall.cn/gtfdwuvvfg.html

);
来源：http://hz.sweek.top/gtikojkpud.html

[Q03] 增加列
来源：http://hz.jianghu66.top/gtgojygqev.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.smart0.xyz/gthbucqzpf.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtnhsbgzjx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pengpengdd.cyou/gtylryzwbp.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gttrvscytw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daxiang520.top/gtjtvgprec.html

[Q06] 删除列
来源：http://hz.bjfxy.top/gttmkqptaa.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xylfe.cn/gtrtqxgcim.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gteueusksd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtgvordhdg.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtqmhosmav.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtnmdxmtdg.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtiqckpges.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gthqbfqoma.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtjzfbgqoc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gtosgmqywg.html

[Q11] 一次插入多行
来源：http://hz.shuidangran.top/gtwzgugczz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtdmzwrcbu.html

[Q12] 插入后取自增 ID
来源：http://hz.cashguo.top/gtwgzmjlnb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.havefunace.top/gtvlekbwel.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtrdyvocpy.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtaeucxcgq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj20258.top/gtqbqqtjuu.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtzfyulsoi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guowangkeji.top/gttyrqjuiz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtqqrubgby.html

[Q15] 查询全部
来源：http://hz.aibaodan.cn/gtyliuucij.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gteaffgyhy.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtagrboxhc.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtbswvfkbm.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtsgkoqdna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgufenzy.top/gtyotxvqip.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtjeydrxeo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.haohaochexian.top/gtqvybcqlf.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtrpjzrroh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.bjfxy.top/gtkrsnsdwr.html

[Q20] IN 列表
来源：http://hz.zhengqikj.top/gtoovazecx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jqgufenzy.top/gtwojkuwkc.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtvruphtge.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yonumen.top/gtpsfsjtdk.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtlezudagl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gttxmlzdmo.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtsgsjqhzo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hongshengwenyu.top/gtmnrxnjhd.html

[Q24] 去重
来源：http://hz.zycfv.cn/gtelenrxyj.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gtkuwceezk.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gtqmpsfzth.html


<!-- 参考信息 -->