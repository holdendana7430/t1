代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtytuzdpdw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcqqunwkw.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtzoxwbrvw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtithhhozq.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtlmmukytz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gthybuxmar.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj202588.top/gtogqgiwek.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtepssdnau.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtymkbfruc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yonumen.top/gtnhoaflpx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gtxkxappsq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtwswdnhba.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtzwwzciaw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtfpktaoxx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtohgyywqu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtdxeulexx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtjojczntw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtnqztgwtb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sufxvd.cn/gtpijvkbtx.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtrezmvaie.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtfubxvaum.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtyxanvfsg.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gtibvtkvge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gttpzufdpm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cashguo.top/gttnmcfopq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtfclcejka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtcckkrsrg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtznzumlcz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtxjyhnaih.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuanzhike.top/gtcszepozo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guannengcc.top/gtphmziqns.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtrfehhwgd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtmhqoysus.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydjk.org.cn/gtcnejtqjo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtbqysujlk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtumggfwjw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gthiyecnin.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ydzc1.top/gtdmuvmujv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtlnqaumlc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtukquiqzf.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gtziwnetmb.html

Py:   math.gcd(a, b)
来源：http://hz.havefunace.top/gtijctntii.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtwsdqytwr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gtjrgydelb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jiagoushi.top/gtglksdisq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigfzy.top/gtbufwxdip.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangtech.top/gtrbyowetp.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtczxozzgk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gthdtiddae.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtxcoecztt.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtrttxlvng.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtgidnohjs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtobsfhqbd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtiqtdwiqn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtnwsllklk.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtzkklpdxk.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtrkjiwuld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtcrbvoasw.html

[N07] 两数之和（返回下标）
来源：http://hz.gotoacloud.top/gtvajvchal.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtyntdlhak.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtvsqshyew.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtmmxylawz.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtguachbaj.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtudzsjpry.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtsipavhxr.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtzuirkeua.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ybcxt.top/gtamnsudbk.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gtyiknxzhg.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtwxmippbu.html

PHP:  // 手写递归交换
来源：http://hz.zhixingplan.top/gtyfuwwzxz.html

JS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtjjnvcprk.html

TS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gteqmkpmbb.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtqbhgbjxq.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtxhbutzln.html

Ruby: arr.permutation.to_a
来源：http://hz.dianchejie.cn/gtoktwgjed.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtmqndmokq.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gtnyrwjffu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtzdwovcko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtobmrioqv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gthuitlcly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.snrcjt.cn/gtetpypkee.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtirwejttl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shuidangran.top/gteqbrmisf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtdvwnywsr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gttltcxgmw.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtmtjkiowt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtzxnlpwkl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtlslhqjwv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.bjfxy.top/gtmgyoraye.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuanzx.com/gtavwnnvfb.html

Java: class Node { int v; Node next; }
来源：http://hz.yongpay.top/gtzogfvhnk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnqzz.top/gtxnjkofrq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtcaifweng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258.top/gtzoyeywov.html

[N11] 二叉树中序遍历
来源：http://hz.chenzaomai.com/gtjihdjqwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtxfvspdce.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtxwldshnu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtrztuznbj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtjlfvwiwz.html

Java: // 手写递归
来源：http://hz.gotoacloud.top/gtwentzeid.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gtsjbchbzi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtvmeffshy.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtpppdjfwb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtatncvwjo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtktwkcxio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenzaomai.com/gthtepgvlz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtcejejnya.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtbrrlnbzs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtzmstvnfr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtyjducwji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnxiangtu.top/gtqrfbcqzk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gaohongyu789.top/gttfonteoz.html

================================================================================
来源：http://hz.svipenyu.cn/gtdgldgvxo.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtlcnbxyod.html

================================================================================
来源：http://hz.cqqwz.cn/gtyqzdescg.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gthevzvnoj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xinyue.icu/gtjrbbnzti.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtshzjewsp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtqdybajch.html

TS:   // 同 JS
来源：http://hz.shanyushiyangtech.top/gtwlrpitjn.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtuukunkhm.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtwflaqjcd.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gttyyrshbl.html

C#:   Task.Run(() => F());
来源：http://hz.yj202588.top/gtekojpiwg.html

[O02] 使用线程池
来源：http://hz.mhx1999.top/gtgxvjlzcr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtfdrkwakh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtwxiurfav.html

JS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtjyapbjuc.html

TS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gtadqmhgjr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yanxiufei.cn/gtoibtjmre.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtxublfplw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shangyingyoupin.top/gtyvztgdrt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hongshengwenyu.top/gtclnncegw.html

[O03] 加锁保护共享数据
来源：http://hz.meibo888.top/gtwnsrstek.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtvmaglety.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ivvv.top/gtbcfkmdgu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gaohongyu789.top/gtkqpiwfjf.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtftehhmpq.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtqdjidpvp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj20258888.top/gtbnzbtoyy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtnoywikft.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtpyzfdogs.html

[O04] 定义异步函数并等待
来源：http://hz.sweek.top/gtbxamsyys.html

Py:   async def f():⏎    await g()
来源：http://hz.tian-w.cn/gtpsvnnvxy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtvuemunwi.html

JS:   async function f() { await g(); }
来源：http://hz.daxiang520.top/gtaohnfcak.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gaohongyu789.top/gtytqucdkn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cashguo.top/gtdewtyxub.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtmnahjjng.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtcvzfopoo.html

C#:   async Task F() { await G(); }
来源：http://hz.c1oappe.top/gtzlejndpm.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gtpxqzrurp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtpnouleuv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gtygfwvjvd.html

JS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtzwlkmdde.html

TS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtofzyubax.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtpnkxwphd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtzlsqzemr.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtrlrrtxff.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.meibo888.top/gtlktfgfsv.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gttzxzrrwz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtjjeniciy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtqdudcxwf.html

JS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtcttrubpe.html

TS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtwssfqnnj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ivvv.top/gtvoknflya.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.meibo888.top/gtxgmzdlcm.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtbeesoqfm.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtdjnnffne.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnfiactnh.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtyhrdipyb.html

================================================================================
来源：http://hz.ybcxt.top/gtjauhdrys.html

[P01] 生成 UUID
来源：http://hz.9152youxi.cn/gtbujflzwa.html

Py:   str(uuid.uuid4())
来源：http://hz.meibo888.top/gtoipqsbej.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.9152youxi.cn/gtprzgcphj.html

JS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtonjlviic.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtqlusuqnr.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gthzubxtfn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ivvv.top/gtdynytcfg.html

Ruby: SecureRandom.uuid
来源：http://hz.birdmap.top/gtbrqyraaf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtqtgixbth.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gtpyxhlwzd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258.top/gtwxpdwgzg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtmdnekwsi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cdnleiting.top/gtofcezawm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj202588.top/gtndvgunym.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shuidangran.top/gtggnsgwvp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtewkoxiuy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.guowangkeji.top/gtidqicpuy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xingfuxueyuan.xyz/gtykfksecz.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtsclugelv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hfpthk.cn/gtpuikdrsv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.quarkkingdee.top/gthfuibpva.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gticnmushb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gttwkbwjmb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jyoumei.cn/gtyrxmgkoq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.havefunace.top/gtqfpmenkn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dianchejie.cn/gtbochiynh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.guannengcc.top/gtkgoyhgoy.html

[P04] 求长度
来源：http://hz.vqdsnc.cn/gtwvqgzmgk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shuidangran.top/gtkqnsxmjr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtjvveuxzk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtxerjaejk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtxjotkhki.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ybcxt.top/gtuwwwosbs.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gtfuuwxmaj.html

Ruby: x.length;  x.size
来源：http://hz.gogol.net.cn/gtijionitr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gtlcgcvnyq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hysaishi.cn/gttmjjlshh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ywan-chungtsiang.top/gtsuibgonk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yueranfly.top/gtgtjmnhrq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtkfnqgwcf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtjvjwcwrz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinghuilouyu.cn/gtpjcywfti.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gogol.net.cn/gttzecpggz.html

Ruby: a == b
来源：http://hz.zhengqikj.top/gtuvstblof.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ywan-chungtsiang.top/gthjmmhqrr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtekhcquqr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinyuanbaomall.cn/gtxfagwglv.html

PHP:  if (empty($x)) {}
来源：http://hz.fzhhl.top/gtxhacuxyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtfvqvkymc.html

TS:   if (x == null) {}
来源：http://hz.gzhubu.top/gtbahepgaf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtbpjnxrss.html

Go:   if x == nil {}
来源：http://hz.bjfxy.top/gtyzdwntvs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtipatloma.html

C#:   if (x is null) {}
来源：http://hz.meibo888.top/gtdrownhak.html

[P07] 防抖与节流
来源：http://hz.wangdashe.top/gtevkuoeax.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenzaomai.com/gtlylobzer.html

PHP:  // 手写时间戳比较
来源：http://hz.ehwqpu.com/gtyaamlpdw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtqsdzxvro.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtjmkojoji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yangfankeji.com/gthcfsnzeh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cheryme.top/gtjgvefbdh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.svipenyu.cn/gtbfyitwhw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinyuanbaomall.cn/gtzukkflml.html

[P08] 处理浮点精度问题
来源：http://hz.mhx1999.top/gtzrxmbczr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guannengcc.top/gtsvqspxad.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinghuilouyu.cn/gtgxvoumjr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtbuqwuaop.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnqzz.top/gtvdejnlgc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.quarkkingdee.top/gtbtmdqdnb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtufdekwsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenzaomai.com/gtzxkvyjvz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.svipenyu.cn/gtjddksqdv.html

================================================================================
来源：http://hz.aizwys.cn/gtbkjjsmja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtmfbdzfgc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtofdeoxrl.html

[Q01] 创建表
来源：http://hz.mhx1999.top/gtbwqrmhgj.html

CREATE TABLE users (
来源：http://hz.fengsongda.top/gtlsbushfw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtxlcmjvis.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtejjqtejm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gterlgbcde.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.meibo888.top/gtpygbrtdz.html

);
来源：http://hz.ywan-chungtsiang.top/gtnznsmuol.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtyehnfruq.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtizqwdguw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shangyingyoupin.top/gtwmzkbanv.html

user_id INT NOT NULL,
来源：http://hz.hnqzz.top/gtcucpzubv.html

amount DECIMAL(10, 2),
来源：http://hz.sufxvd.cn/gtpuhmrwix.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guannengcc.top/gttjiibyqh.html

);
来源：http://hz.zdqjudy.top/gtdutoskxg.html

[Q03] 增加列
来源：http://hz.kuanghao11.cn/gtxvakwvqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtwxdjvooo.html

[Q04] 修改列类型
来源：http://hz.birdmap.top/gtnegosygo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtaxntixgy.html

[Q05] 重命名列
来源：http://hz.tian-w.cn/gtbcbkkcqv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ivvv.top/gtpnacrldf.html

[Q06] 删除列
来源：http://hz.smart0.xyz/gtwwqdislr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtocprfceu.html

[Q07] 删除表
来源：http://hz.tanke756.top/gtmpxhlgct.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtuvsvhteu.html

[Q08] 创建普通索引
来源：http://hz.ybcxt.top/gthieekfka.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gttzkczdbs.html

[Q09] 创建唯一索引
来源：http://hz.yangfankeji.com/gtcariijos.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtxiwqwuxm.html

[Q10] 插入单行
来源：http://hz.gogol.net.cn/gthcqjshhu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.vqdsnc.cn/gtrkagrfdc.html

[Q11] 一次插入多行
来源：http://hz.yuanzhike.top/gtcrragjjl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtffkjuqno.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gthuylatgi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.dashuyun.cn/gtpbntorgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.aibaodan.cn/gtgpuyprxs.html

[Q13] 忽略重复插入
来源：http://hz.gaohongyu789.top/gtcxddxkcw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtjfzmvuyg.html

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtbcvpvalt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gotoacloud.top/gtovtqwohn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenzaomai.com/gtgnjdvokv.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtrlzpgrcz.html

SELECT * FROM users;
来源：http://hz.xuanzx.com/gtnoqgalpr.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtgatfnneb.html

SELECT id, name FROM users;
来源：http://hz.jinqigfzy.top/gtbuenydco.html

[Q17] 条件查询
来源：http://hz.feifeiyinyue.top/gtndqflcnw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhaomingkeji.xyz/gtbfyfzlxg.html

[Q18] 模糊匹配
来源：http://hz.zhengqikj.top/gtjhodesbl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gtgtxbnnsw.html

[Q19] 范围查询
来源：http://hz.ydzc1.top/gtfqppicrr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cdnleiting.top/gttwrzbogf.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtqsyannzd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtpqflozqj.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gtzjcgdegn.html


<!-- 参考信息 -->