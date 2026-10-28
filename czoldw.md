代发 wailian999

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gthbmdkrki.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtcpjmqnkp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtqaoummkp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtibuztydy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtfkibstxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtmhgcbrko.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gtbduaqxcy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtcvkgiekg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtbaeluywc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtairohkwc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtbwygjuhs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtstldwkmo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtfwmhrnev.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtfaqnllse.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtyvioslis.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtmcwqldkv.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtuyocednz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yanxiufei.cn/gtdoqszwqd.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtfjjeptry.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.c1oappe.top/gtoixrlfac.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtyyobbqao.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtwmizadkf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtselguhqp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.c1oappe.top/gtrfaongjx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtkkjmvzmy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guowangkeji.top/gtlxxeuxcq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtsbtfbmcz.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtesartywz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtwmzitpgr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuxming.cn/gthpsxauoc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gthvionxid.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtgfdhyyxb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gtbtlgitfg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.316326.xyz/gtkkptrtxh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtmnhczfez.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtddgyjude.html

[N05] 最大公约数
来源：http://hz.kuanghao11.cn/gtvtuwtwgx.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtrtqdgkbj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gttpkmdodf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtyfzdieah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gttfahzswz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtisykpbxk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtflzldaey.html

Ruby: a.gcd(b)
来源：http://hz.jinyuanbaomall.cn/gtdclibohf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.daria6918.cn/gtbjkweyif.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtxmsndxfp.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gtqpcbevnt.html

PHP:  $s === strrev($s);
来源：http://hz.yuanzhike.top/gtqeruhhpg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtyvdeqgkc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtjuqvikyc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtovlnxqbk.html

Go:   // 双指针从两端比较
来源：http://hz.redwolf501.top/gtipksbufy.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gtxoyiguxm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtdiqiwgpt.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gtwzvfkwmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.c1oappe.top/gtcjshcsmp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtlvxlzcns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhongyouzk.top/gtfqobllaa.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtltxzmprn.html

Java: // 手写 HashMap
来源：http://hz.ydzc1.top/gtsttzonsn.html

Go:   // 手写 map[int]int
来源：http://hz.havefunace.top/gtceflqmki.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtzlutjclz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuxming.cn/gthjfzzagm.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtejhjikod.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtykxtjfdu.html

PHP:  // 手写递归交换
来源：http://hz.tianlin.xyz/gtbfenhtgv.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gttlczgalh.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtcgeppckg.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtflvtiyha.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtxjefiaun.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtfwusecqj.html

C#:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtanpbaohy.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gttmewebcf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gtpzgdqwrp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tian-w.cn/gtfxkvusaq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtynvqfrlz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtwglqrujn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gtfnmbgdre.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenjidiqi.icu/gtztyltlhl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gtrwuypeiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtzsgnzjgf.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gttzgznoke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtcgidnfik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gthkjvqiqq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shzxlz.cn/gtbdguckrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtylqsgdyy.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gtmjbkhmwi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gotoacloud.top/gtrgmmwdtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gogol.net.cn/gtenyfgojc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydjk.org.cn/gtnhbbztyl.html

[N11] 二叉树中序遍历
来源：http://hz.kuanghao11.cn/gtryetzwba.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtufdwiytx.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtsiseicmj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtbespncqz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtjzohmkbr.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtvgosdxis.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtabbhshth.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtkimbbsmx.html

C#:   // 手写递归
来源：http://hz.cheryme.top/gtjtxpndpy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtkeujlyaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yanxiufei.cn/gtkaocbroa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yongpay.top/gtveazwcvq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtpmuljlak.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtabqfdlor.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtisiuhiza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtgygwqigd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtxzoavuho.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtgqibamia.html

================================================================================
来源：http://hz.52xcode.cn/gtpuyldvvg.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtfyklshzs.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjknnvcdk.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtiroxgryl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.smart0.xyz/gtnithiccc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sufxvd.cn/gtjscpzhbr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xinyue.icu/gttmidhwiz.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtiqcifwwu.html

Java: new Thread(() -> f()).start()
来源：http://hz.gaohongyu789.top/gtgweeibyp.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtsfyoqabo.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtqnefcjxb.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gtwhhlqdyr.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gtnlvhzgjf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtnvbpzcgr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtqppojsei.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtuwlgrzvj.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtbjtfpldh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtnrzqltbq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtpijmwkpx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtzgqxdbpe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtwdfwpfvv.html

[O03] 加锁保护共享数据
来源：http://hz.andypj.xyz/gtmpzizqef.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtaqrykjzl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gthrierxqk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gtnsqhgcjc.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtejodukei.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtwacrgxgu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dashuyun.cn/gtwoawulkf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtmjzlnnct.html

C#:   lock (gate) { shared++; }
来源：http://hz.tian-w.cn/gtqejdegpy.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gttgkhntlo.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gthncwvknz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gtbvsdthwl.html

JS:   async function f() { await g(); }
来源：http://hz.hongshengwenyu.top/gtexqnvqbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gtkugmktgn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangtech.top/gtdkpurrde.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.nanxuanxn.top/gtnhxmxtmx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtstawzwux.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtqcgyixyv.html

[O05] 并发执行并等待全部完成
来源：http://hz.yonumen.top/gtndxqshqc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtajbdeboy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.c1oappe.top/gtdmxtilay.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtweopfmfj.html

TS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtogojshfy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yvedp.cn/gtneeohaky.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.pycfn.com/gtabmjrdsd.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gtjdgyjegr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinqigfzy.top/gtsyphtode.html

[O06] 使用进程池
来源：http://hz.cheryme.top/gtoahvbuxw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtqyruwqfp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pengpengdd.cyou/gtrdxovrcx.html

JS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtaxhjuzzu.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtjyaocjdm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gtrdqeehwx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.snrcjt.cn/gtjiggdckx.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gtqvdocija.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtgdydtwlm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmvxkidgw.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtxpuurkip.html

================================================================================
来源：http://hz.c1oappe.top/gtoidktxeo.html

[P01] 生成 UUID
来源：http://hz.jqgufenzy.top/gtwivmjzrj.html

Py:   str(uuid.uuid4())
来源：http://hz.zhongyouzk.top/gtowpomocc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gtxhybkapm.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtdhqkacaz.html

TS:   crypto.randomUUID()
来源：http://hz.birdmap.top/gttjfpnehz.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtflaopghj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtsbpscqxa.html

Ruby: SecureRandom.uuid
来源：http://hz.zdqjudy.top/gtuuctgbnz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hammf.cn/gtqingcuks.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuetiantiany.cn/gtifznydzl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ppjwa.cn/gtvvqexzep.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtoeuopxin.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtbgsjircb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zycfv.cn/gtagfbarsx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.xinyue.icu/gtqnbyeigu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fengsongda.top/gtihfxvzff.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.redwolf501.top/gtiigaruqb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gtzkigcclk.html

[P03] 生成短随机字符串
来源：http://hz.sxryk.cn/gttsdcaosh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yonumen.top/gtdxqbnvvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cdnleiting.top/gtiomynpzn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sysykeji.top/gtwnubezpp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtekhidkwj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtoeadjkez.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hongshengwenyu.top/gtjywzmdum.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.kuanghao11.cn/gtdptoxtpf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gtcrbekskw.html

[P04] 求长度
来源：http://hz.xingfuxueyuan.xyz/gtpkhumlgt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cucudq.cn/gtrkogywdp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtqqzarqdo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnqzz.top/gtgrcdwjpu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gthvpfjuhj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtztnhcbrj.html

Go:   len(arr);  len(m)
来源：http://hz.ehwqpu.com/gtfpajxgio.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtxfhulepz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtqamdbylu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ybcxt.top/gtjjkkegpx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtymcfzled.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ehwqpu.com/gthqhdegti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtaxzuzxoj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtjwaipoln.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtjtqfxfxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.52xcode.cn/gtuyalludl.html

Ruby: a == b
来源：http://hz.iojbl.cn/gtrnndbgho.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtjmfcpcgd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinqigfzy.top/gtntzzuwzf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.0kj1m.cn/gtaswehbnf.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangtech.top/gteotpcutj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xinyue.icu/gthgqgjzuu.html

TS:   if (x == null) {}
来源：http://hz.ywan-chungtsiang.top/gtdmzpbbij.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pengpengdd.cyou/gtbsozlkje.html

Go:   if x == nil {}
来源：http://hz.aizwys.cn/gthyrdsvun.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtssquecdh.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtzxvujaob.html

[P07] 防抖与节流
来源：http://hz.gaohongyu789.top/gtdslzsvad.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gogol.net.cn/gtepexhbqt.html

PHP:  // 手写时间戳比较
来源：http://hz.pycfn.com/gtdlxoiyvk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtqgvjfbpb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtyubwbush.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yueranfly.top/gtqwtdgfro.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtqdzcyrth.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.havefunace.top/gtrejelfpq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtengegmnt.html

[P08] 处理浮点精度问题
来源：http://hz.yuanzhike.top/gtcpejkubf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.316326.xyz/gttkfazgph.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ehwqpu.com/gtyowrznvn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtorvxwtoo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gtamwpdtas.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258888.top/gtanbccfeh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gthzfjnwxe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gtcqgwjios.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yanxiufei.cn/gtnqebzhjc.html

================================================================================
来源：http://hz.snrcjt.cn/gtmisojbgy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtxmrnunwi.html

================================================================================
来源：http://hz.birdmap.top/gtjlvgnwby.html

[Q01] 创建表
来源：http://hz.iojbl.cn/gtithcresm.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtkordtjsd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtiiikvsls.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgfzy.top/gtkzydgmvf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtaeprlukc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.svipenyu.cn/gtsxemonmj.html

);
来源：http://hz.jinqigufen.top/gtigxthmng.html

[Q02] 创建带外键的表
来源：http://hz.yuxming.cn/gtosbcnrwg.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtessxtfir.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtasbajzof.html

user_id INT NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtcyhlopka.html

amount DECIMAL(10, 2),
来源：http://hz.wangdashe.top/gtmhchyxyx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pengpengdd.cyou/gtvbjilzml.html

);
来源：http://hz.jqgufenzy.top/gtxgmqfjgc.html

[Q03] 增加列
来源：http://hz.shanyushiyangtech.top/gttmbtvcin.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtzywibluu.html

[Q04] 修改列类型
来源：http://hz.daria6918.cn/gtirkyknfm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gtxsggnezo.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtoiknrqdi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.iojbl.cn/gtsiibxisk.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtoxxuazls.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sysykeji.top/gtgmhkjpwk.html

[Q07] 删除表
来源：http://hz.cqqwz.cn/gtsfdnidgc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xinyue.icu/gtrnhhwjcp.html

[Q08] 创建普通索引
来源：http://hz.yonumen.top/gtocjjxhhd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gttbtircqq.html

[Q09] 创建唯一索引
来源：http://hz.guowangkeji.top/gtasyonbdk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtawhnpaak.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gtivcrwant.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258888.top/gtqrpeaaqv.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtxwcwjlyu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daria6918.cn/gttmuryxhi.html

[Q12] 插入后取自增 ID
来源：http://hz.0kj1m.cn/gtkfvrzbyy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuxming.cn/gtplqetntj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ywan-chungtsiang.top/gttkkkfvoh.html

[Q13] 忽略重复插入
来源：http://hz.yanxiufei.cn/gtdqfdfoig.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gtmxuoaavu.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxinkj.top/gtwebqghuz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xinyue.icu/gtbfljvjmo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtydtinera.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gtzjuakdul.html

SELECT * FROM users;
来源：http://hz.jiagoushi.top/gtxaoinmrz.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtmpwwixgx.html

SELECT id, name FROM users;
来源：http://hz.cashguo.top/gtwgprwwpv.html

[Q17] 条件查询
来源：http://hz.52xcode.cn/gtlyoikezi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtdrilviqe.html

[Q18] 模糊匹配
来源：http://hz.zhongyouzk.top/gtnpygdics.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuxming.cn/gtlbisworq.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtpehtycqz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtuwouidja.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtyahmvcbi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gthnofcdar.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtcvmucfqq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnxiangtu.top/gtepwgmhfp.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gtpznoztsz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtjqcqkubi.html

[Q23] 分页
来源：http://hz.hfpthk.cn/gtopifhmin.html


<!-- 参考信息 -->