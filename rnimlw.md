代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtixiuului.html

================================================================================
来源：http://hz.birdmap.top/gtxoyqvkab.html

N. 数据结构与算法
来源：http://hz.cucudq.cn/gteblyhdbr.html

================================================================================
来源：http://hz.guannengcc.top/gtvcgyjgng.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtygsopbhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtahjmkmmc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtykorxpry.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtwtvniken.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtjeoomnbr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtyvmgcrzq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtpzktvelf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtdqhbhaja.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtjzvomrnz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtqsooadkr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtyecawpvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtixxfukdu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtusiegdro.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtcresllkf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtlktswuqj.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gttkodimib.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtvobujrep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtwkpzkwoe.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtueavzuyo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtfsvipvqi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtgedchjak.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtqiklgxcg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtiixuuwgf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtkklbjkwv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhaomingkeji.xyz/gthuxjvyon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtudsalguc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtrapnmsxb.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtyueergrp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtrxldvcme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtrlpotwlu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtilhdtzfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtgwgoqmkm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtcvctqfva.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtvfxztzny.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gteorvuzag.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtdcqdejdj.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtufwoeoyb.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gttdzabhgl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj202588.top/gtdlcwfbcy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtxlsnfqxq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtzgvseugf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.316326.xyz/gtdvktsasw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtrrhewnci.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gtaodutuit.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenzaomai.com/gtvlmigoqd.html

[N06] 判断回文字符串
来源：http://hz.shuidangran.top/gtocskhgxa.html

Py:   s == s[::-1]
来源：http://hz.cqqwz.cn/gtksbcopek.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtqmbkrkps.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gttqlelmjr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtgbvwgfnb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtgnjpbqbq.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtzkfddvwg.html

Ruby: s == s.reverse
来源：http://hz.smart0.xyz/gtispkxsyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtqbumqnwp.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258.top/gtkkjewhzn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yangfankeji.com/gtmzqlqker.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yangfankeji.com/gtjbazvcah.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fengsongda.top/gtwbzdnndf.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtftuyfvwt.html

Java: // 手写 HashMap
来源：http://hz.hysaishi.cn/gtrwqzldzi.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtfeyhejdu.html

Ruby: // 手写 Hash
来源：http://hz.quarkkingdee.top/gtogoujevc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fzhhl.top/gtrqpqszyx.html

[N08] 生成全排列
来源：http://hz.shzxlz.cn/gtqrxjviav.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtvwyvhjlz.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gthyioniwu.html

JS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtpypfqozi.html

TS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtvguuaaum.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtvifmcjgo.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtjcktxsfd.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtyspecxkp.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtmqswtgps.html

[N09] 栈与队列
来源：http://hz.birdmap.top/gtqijsaziq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shzxlz.cn/gtfrgfknpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtbjczobgk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtfuweaojj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gtqagjgvli.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtiistzwit.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gthfdgootk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtsnneojdg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtcairdfux.html

[N10] 链表节点定义
来源：http://hz.zycfv.cn/gtlwcadidc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtvyrlcxhl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtxqzctzqd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtwdmdpgkw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenjidiqi.icu/gtebnznhgp.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtxpzlnrbv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tianlin.xyz/gtgujffoxz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtuqpwaicu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gtxkoljsey.html

[N11] 二叉树中序遍历
来源：http://hz.0kj1m.cn/gthfvomukq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nwbrower.top/gtvfhzwfjy.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtfrqdrqrg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhengqikj.top/gtqensidkx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtahltgopj.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtxwcbbopr.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtnpnmpotg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtddpxwyde.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtrzeenbgw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hammf.cn/gtrtjwrpoj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtmbojxhkq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtsyotwwsz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtyudruizq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtrdwyeauc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtjjtasjqp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtmlrnhczc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtubogdopa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtidsuzvmc.html

================================================================================
来源：http://hz.smart0.xyz/gtktcmxowm.html

O. 并发与异步
来源：http://hz.yuxming.cn/gtkhqzxexc.html

================================================================================
来源：http://hz.xylfe.cn/gthhcichzh.html

[O01] 启动一个线程
来源：http://hz.sxryk.cn/gtcbqqljno.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.svipenyu.cn/gthgngjzef.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xingfuxueyuan.xyz/gtvwkxbfyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cheryme.top/gtvtmiohwm.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtpngzhbet.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtxklxkqnq.html

Go:   go f()
来源：http://hz.yanxiufei.cn/gteieeaqzc.html

Ruby: Thread.new { f }
来源：http://hz.jqgfzy.top/gtpruhiniq.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gteumbvbdc.html

[O02] 使用线程池
来源：http://hz.smart0.xyz/gttogocgeo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cqqwz.cn/gtowgyqoyf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gotoacloud.top/gtpfiabxny.html

JS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtkaxbbawc.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtfopqlfcz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtotgrsdhp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gthtqcgdxj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.quarkkingdee.top/gtbpqexzmt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gterynmhso.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtjnfsribb.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtqyhdezzh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtchgibsrr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuanzhike.top/gtqjzwkygt.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtczykawlw.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuanzx.com/gtrhaglrcv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xinyue.icu/gtmzvfikyl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangkeji.top/gtxzivsvrc.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtwboumcpi.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtaynmkkji.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtflclbfkt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gtcuqshjen.html

JS:   async function f() { await g(); }
来源：http://hz.cqqwz.cn/gtbhssuiel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtcuuyinwl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.quarkkingdee.top/gtfqdddldo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tianlin.xyz/gtfuknvtda.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtlzgukhds.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtiympcirc.html

[O05] 并发执行并等待全部完成
来源：http://hz.sxryk.cn/gthvtosxsb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gttnfnczvs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtlckkqxdn.html

JS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtpfjoqbeq.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtamkcavbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gtitreaunr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtiywbxpfj.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtxxvgxajd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtpvogjsqb.html

[O06] 使用进程池
来源：http://hz.shanyushiyangtech.top/gtdwxzmrqp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuanzhike.top/gtsadmeqxf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtkbsekaju.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtzldqrfgm.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtvsppexqk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gttpxrrujm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtwtiojcxr.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtzwdtnqva.html

C#:   Parallel.For
来源：http://hz.jinghuilouyu.cn/gtggbxegqt.html

================================================================================
来源：http://hz.dashuyun.cn/gtgahwzcnj.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtnxfodpqu.html

================================================================================
来源：http://hz.snrcjt.cn/gtmgfuxdrx.html

[P01] 生成 UUID
来源：http://hz.hysaishi.cn/gtafkpouum.html

Py:   str(uuid.uuid4())
来源：http://hz.316326.xyz/gtzmegqpev.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gtjkgvxtzq.html

JS:   crypto.randomUUID()
来源：http://hz.gogol.net.cn/gtbfidbjzt.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtucbiqoak.html

Java: UUID.randomUUID().toString()
来源：http://hz.yanxiufei.cn/gtoegabxea.html

Go:   // 用 github.com/google/uuid
来源：http://hz.iojbl.cn/gtpnwcdnch.html

Ruby: SecureRandom.uuid
来源：http://hz.xylfe.cn/gtbvttvtsm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtgbywtbnl.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtyfhxxklh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinghuilouyu.cn/gtxpamvjve.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtptjaithn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtcxpcrpxl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zycfv.cn/gtpwqqkwxv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nwbrower.top/gtehlteytf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fengsongda.top/gtzowkcciq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.redwolf501.top/gtzzpqtubx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jiagoushi.top/gtthrsvdtp.html

[P03] 生成短随机字符串
来源：http://hz.sufxvd.cn/gtkcbybrmq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtbczkbiyz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.smart0.xyz/gtkfktjixk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtfimktzoj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtvusylncu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hongshengwenyu.top/gtlecvorzy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuanzx.com/gtfsjeepay.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.c1oappe.top/gtlxqzszvq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtbhzjjjtb.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gthdpdbhzq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gttgtdxicv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtypebdbfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtjenztney.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtrhknktrk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgufenzy.top/gtbqakbozl.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtaxujrpcz.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtywqypdaf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtltrhiaie.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtwfqnzoul.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gttkramfkf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gaohongyu789.top/gtcmqqmymv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinqigfzy.top/gtatfawquy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gtqdyoimqw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pengpengdd.cyou/gtqydsawxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtomyipcic.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtcpgcvila.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shzxlz.cn/gtyablsvcu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gtbcitgnqd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gtnfomlsvc.html

PHP:  if (empty($x)) {}
来源：http://hz.ybcxt.top/gtenbswzei.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gteiufybfm.html

TS:   if (x == null) {}
来源：http://hz.zycfv.cn/gtdqktyfcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hammf.cn/gtlldfivzb.html

Go:   if x == nil {}
来源：http://hz.gaohongyu789.top/gtjwbmdclw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtunykarlf.html

C#:   if (x is null) {}
来源：http://hz.dianchejie.cn/gtiyyvupgf.html

[P07] 防抖与节流
来源：http://hz.gogol.net.cn/gturuqhtov.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gthqqehezb.html

PHP:  // 手写时间戳比较
来源：http://hz.zhoulong.xyz/gtclayzopq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtltjdtwrz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtpyivqxut.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhongyouzk.top/gtkecswpas.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtyebmsuxe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jqgfzy.top/gtgcocfvzz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jlsjyb.cn/gthbqycnws.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtltzijuds.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hfpthk.cn/gtwiwzydzn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.birdmap.top/gtrsjodykt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.tanke756.top/gtqiqdqgnf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gtgetzyjax.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtmztjhhoz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cheryme.top/gtwcadewgb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258.top/gtcbmrpkdy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gttkrzpubv.html

================================================================================
来源：http://hz.haohaochexian.top/gtulblrxgs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cucudq.cn/gttjjgndxs.html

================================================================================
来源：http://hz.ppjwa.cn/gtyboztrda.html

[Q01] 创建表
来源：http://hz.jiagoushi.top/gtqypgskur.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtqgymbonv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtxdqaxjhu.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnqzz.top/gtxuhowrxt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtxyvgdghu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtuyqasbfj.html

);
来源：http://hz.sweek.top/gtkplyfriq.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtcyanalqz.html

CREATE TABLE orders (
来源：http://hz.shuidangran.top/gtsomhnxtl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtbnelrbza.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtsayzeicz.html

amount DECIMAL(10, 2),
来源：http://hz.zhengqikj.top/gtqhzprcsn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.nanxinkj.top/gtbamqdarx.html

);
来源：http://hz.zycfv.cn/gtlxtqxpyk.html

[Q03] 增加列
来源：http://hz.shuidangran.top/gtvdiqlcdg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhaomingkeji.xyz/gtozeymlyj.html

[Q04] 修改列类型
来源：http://hz.guannengcc.top/gtynphhfbh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtpmavlqhx.html

[Q05] 重命名列
来源：http://hz.gogol.net.cn/gtijbdyfnz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nwbrower.top/gthgdonrhi.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtpvvzjaim.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtegaprcnp.html

[Q07] 删除表
来源：http://hz.ppjwa.cn/gtsezgixhd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yanxiufei.cn/gtnqpclsar.html

[Q08] 创建普通索引
来源：http://hz.shuidangran.top/gtpixwqrlo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtvkrzhgkj.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtqyzzkiac.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hammf.cn/gtgbrtzycp.html

[Q10] 插入单行
来源：http://hz.cashguo.top/gtcugloolt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydjk.org.cn/gtwseutdqq.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtwdqfsdxa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.havefunace.top/gtuthurrwn.html

[Q12] 插入后取自增 ID
来源：http://hz.vqdsnc.cn/gtdstgkveu.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtnusaecrv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yanxiufei.cn/gtbqstlnon.html

[Q13] 忽略重复插入
来源：http://hz.guannengcc.top/gtmutppznh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.daria6918.cn/gtlkbqsmrn.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuxming.cn/gtnlvgixpi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.bjfxy.top/gtltmhyjks.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtoglslrmw.html

[Q15] 查询全部
来源：http://hz.birdmap.top/gtqyzvnbjz.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtttcntxpr.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtwurapdag.html

SELECT id, name FROM users;
来源：http://hz.jinghuilouyu.cn/gtnqptybow.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtocdbrlmr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.52xcode.cn/gtvgxbppqi.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtmwqmoard.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.sweek.top/gtiatuuzcb.html

[Q19] 范围查询
来源：http://hz.shuidangran.top/gtsjlawwyf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtpjcrgxvf.html

[Q20] IN 列表
来源：http://hz.hongshengwenyu.top/gtgkjdtetm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtyarwokng.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gtjeedumqb.html


<!-- 参考信息 -->