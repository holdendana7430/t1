代发 wailian999

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtjiyflpia.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtewpgmfad.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtwgkgqzev.html

JS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtvnuahtpg.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtqesqzdls.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtajfuxgyi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtbowjuhsb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtlujyzxjl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgufenzy.top/gtncccmmmz.html

================================================================================
来源：http://hz.tanke756.top/gtrtitbvwp.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gthomunzix.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqfwagwef.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtrpnsoust.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtoplkxvef.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtnwifhofi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtnnhqgcex.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtgolgtgse.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gtycolbpvp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtvaveoarz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.feifeiyinyue.top/gtnaizujkl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtyceysnqt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtdvjrzrwn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtllrdirhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtwnmkyvvx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtfgdoarww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtornxoypm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtqrucvcop.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gthdrbewef.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gthpvxwogh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtxfffdgcc.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtdpmdpuhs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuanzhike.top/gtvvdhtqgo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtbargxumd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtlapjxeqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtrqhnduwi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtukhkxfjl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtbkdgczxw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtpzgsvdxc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtozejxcmc.html

[N04] 斐波那契数列
来源：http://hz.meibo888.top/gtmwshgbbv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtmcweollr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shzxlz.cn/gtnlzgmcqb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtgoryvddj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtfimwgxyj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtsuqpveen.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtovchazft.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtukexkbjm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydjk.org.cn/gtcgkdaaav.html

[N05] 最大公约数
来源：http://hz.meibo888.top/gttxvbbqef.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtbtdnaeyb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtyciwkzqx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtulnosfwo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.snrcjt.cn/gtpoiikzdy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtqeztwpoi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xziqi.cn/gtaqxrdhkk.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gtkdaijwbd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.52xcode.cn/gtupeyecqr.html

[N06] 判断回文字符串
来源：http://hz.hnqzz.top/gtulnffhri.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtuzohnurg.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gttmioszyi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtohyqwxbn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtrazkentd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtmnmadbpo.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtdwiaewnc.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gtllupzszy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtddfymvuw.html

[N07] 两数之和（返回下标）
来源：http://hz.jinyuanbaomall.cn/gtswfqcalj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtxhwshzue.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gaohongyu789.top/gtvqubqcej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtunjipdde.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gttspckfqi.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtmphytnnv.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtjqnztont.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtnccldtgv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtqrxroctt.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gthzxdjtoe.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gtxdrjhlto.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtmohljbed.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtnywwxphd.html

TS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtuujxankg.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtmgrboblu.html

Go:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtrhephovy.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gttlgnthyq.html

C#:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtbkmbyeon.html

[N09] 栈与队列
来源：http://hz.hammf.cn/gtquytabjx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.feifeiyinyue.top/gteuwoccjw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gtlnisakmu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cucudq.cn/gtrgkwtddh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gttjvgljwo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtibooeggt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtvrnsazch.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xziqi.cn/gtcuhkqxzf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtfafowqfr.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtqzchrffb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.bjfxy.top/gtupmplxms.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtozdtslcw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtgokwjqfg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtdzsrzvyq.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtjbthydjd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gthzhrloxb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tian-w.cn/gtrzquauuc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtqztjkwyl.html

[N11] 二叉树中序遍历
来源：http://hz.guowangkeji.top/gtedxvirqb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtewlororb.html

PHP:  // 手写递归函数
来源：http://hz.chenjidiqi.icu/gticvhsfcj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gtheoofdjj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtyajuqbzg.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtkdmnnily.html

Go:   // 手写递归
来源：http://hz.pycfn.com/gtpttvjrht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtrcuuzvpy.html

C#:   // 手写递归
来源：http://hz.chenjidiqi.icu/gteftpwcof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tian-w.cn/gtxnznbfua.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtoakromfh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gttqwrrtfh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtcktpuopq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtwdypvjpe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gttalggdws.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtuymkgrds.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gzhubu.top/gtkpxbgryh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtguropcmn.html

================================================================================
来源：http://hz.ybcxt.top/gtnpdfaiww.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtuqkststa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtugsltmeh.html

[O01] 启动一个线程
来源：http://hz.zhongyouzk.top/gtgupekjiz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gttmqjcqrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.vqdsnc.cn/gtmyguerau.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.wangdashe.top/gtlhvwhtgb.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtflcyzdkf.html

Java: new Thread(() -> f()).start()
来源：http://hz.gogol.net.cn/gtjvrqgcis.html

Go:   go f()
来源：http://hz.jinyuanbaomall.cn/gtzxclsnkz.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtpdcohdus.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtsvcjupll.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtuxsamerj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gtvszmykby.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtjezqzvzw.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtqqmwybvo.html

TS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtntsbvzbj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hywenlv.cn/gthkytusvz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtpnetzonf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sufxvd.cn/gtfykexnid.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jianghu66.top/gtsmpktbmw.html

[O03] 加锁保护共享数据
来源：http://hz.svipenyu.cn/gtxzrhkuts.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtmqyyjhkb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtsbpxdavd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtwppggfgj.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtykazhrkt.html

Java: synchronized (this) { shared++; }
来源：http://hz.gotoacloud.top/gtszkariik.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gtsipfznxq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangtech.top/gtjnnkncdj.html

C#:   lock (gate) { shared++; }
来源：http://hz.wangshuangyany.cn/gtakxjougu.html

[O04] 定义异步函数并等待
来源：http://hz.hysaishi.cn/gtoixmgdde.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtrxbzpoej.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtksnqnphx.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gtwcagodlo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtxbfjgiai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gtpbmcuals.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yanxiufei.cn/gtimlsubde.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.xziqi.cn/gtljrpqjbd.html

C#:   async Task F() { await G(); }
来源：http://hz.zhengqikj.top/gtpuutuvid.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtfriuyzeo.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtmysirenx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhoulong.xyz/gtpuunwnqq.html

JS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtvrodjbak.html

TS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gttapcfmfb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtmnijwxwj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtoqehvdyx.html

Ruby: threads.map(&:join)
来源：http://hz.xziqi.cn/gtnocflgcw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.316326.xyz/gtdvfgwtfv.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gtopfkxaxp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtsdemwldv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtuhgikupf.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtxibzuzpo.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtjvebvoib.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.snrcjt.cn/gtgnijfeij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtumsobrpx.html

Ruby: // fork 块
来源：http://hz.gaohongyu789.top/gtdcqfripy.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtgepcmnla.html

================================================================================
来源：http://hz.gotoacloud.top/gtchityobe.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gttjrhxevr.html

================================================================================
来源：http://hz.hywenlv.cn/gtfupqdfeq.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gtzebwjtbv.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gtswahxljy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtbiooepqf.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtdrhqwfko.html

TS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtbbhotnlj.html

Java: UUID.randomUUID().toString()
来源：http://hz.tanke756.top/gtxtszxqsb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xuetiantiany.cn/gtmfdjnflp.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtxnjzbaiw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.haohaochexian.top/gtopwqdsop.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtsbfnqhvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtsssxbejc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtrkqjoems.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hongshengwenyu.top/gtxywheavp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtyhlhjxfy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yvedp.cn/gtsifaejob.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gthryeqqca.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258.top/gtdscqashg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jyoumei.cn/gtsqqinkcw.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangkeji.top/gtjuquitxa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtqaioggbm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tianlin.xyz/gtryxzfcwq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtnllptqyp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtyfxusjpn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhijiandao.cn/gtbsbuqyhq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtawqmsczd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtdgstsfpg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtuczxtomf.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gtkezpkhib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangtech.top/gtluilwrix.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gtjucugkwf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gtniikwlri.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtvlahmrpb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgfzy.top/gtqdunjfmt.html

Go:   len(arr);  len(m)
来源：http://hz.nanxinkj.top/gtdxmrdlyz.html

Ruby: x.length;  x.size
来源：http://hz.hfpthk.cn/gtkvpgjlxv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zdqjudy.top/gtlnyspycp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtllexqwmw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gteyifqdxa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zycfv.cn/gtcnqximnn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtgqqgoeuq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtiupczbaj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtwhfdaelr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gtfqsqmblz.html

Ruby: a == b
来源：http://hz.jiagoushi.top/gtkwytzqpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtivmcwonu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhijiandao.cn/gtyhuyfpxb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinyuanbaomall.cn/gtupxycqlo.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtcmdyhdpu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gthhqwsetq.html

TS:   if (x == null) {}
来源：http://hz.jianghu66.top/gtqgogkgui.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnqzz.top/gtmgjuogop.html

Go:   if x == nil {}
来源：http://hz.cqqwz.cn/gtomrqxfts.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gtdzcfamzw.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gthellkgjp.html

[P07] 防抖与节流
来源：http://hz.hongshengwenyu.top/gtlieatmvl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtiyjcuaze.html

PHP:  // 手写时间戳比较
来源：http://hz.fengsongda.top/gtunfocbpa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtwjocrfdg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtpgherlow.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jianghu66.top/gtookjqgnq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.c1oappe.top/gtpitwiwwi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtnirjpzfc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hywenlv.cn/gtowrmgpgc.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangtech.top/gttzfxijpz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tianlin.xyz/gtanrkeqbj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jyoumei.cn/gtvtfwuxqm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jlsjyb.cn/gtmzgrfmsb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.bjfxy.top/gtklsetrnq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnxiangtu.top/gtyrxvzgkn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtsvlriyim.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.havefunace.top/gtgaejgcez.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ybcxt.top/gtotefxtzh.html

================================================================================
来源：http://hz.jqgfzy.top/gtjammsitk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.iojbl.cn/gtopoctqen.html

================================================================================
来源：http://hz.sufxvd.cn/gtbgzozzve.html

[Q01] 创建表
来源：http://hz.fengsongda.top/gtcsloksyt.html

CREATE TABLE users (
来源：http://hz.shanyushiyangtech.top/gtidgdactt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtmdvqerxo.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jianghu66.top/gtahbqgmbv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtpcehqmvy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gtsevnpqzw.html

);
来源：http://hz.zhoulong.xyz/gtsnijuadu.html

[Q02] 创建带外键的表
来源：http://hz.ybcxt.top/gtiihfdxwq.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtmswwdbga.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.bjfxy.top/gtnehhrvlu.html

user_id INT NOT NULL,
来源：http://hz.xinyue.icu/gtmdrjncyo.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtgdjrbqlz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhiwuduotai.top/gtwkzovkub.html

);
来源：http://hz.jinqigfzy.top/gtlgruiszf.html

[Q03] 增加列
来源：http://hz.xuanzx.com/gtbrdbadto.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtkjbaandu.html

[Q04] 修改列类型
来源：http://hz.yuxming.cn/gteqotuwls.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yueranfly.top/gtjtjstxat.html

[Q05] 重命名列
来源：http://hz.yj20258888.top/gtkmzrsvfx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenzaomai.com/gtlccflmtr.html

[Q06] 删除列
来源：http://hz.ydzc1.top/gtoyblfkfg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtqtoghtqi.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtcarnugrn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtyyrbpovr.html

[Q08] 创建普通索引
来源：http://hz.zhaomingkeji.xyz/gtjbabxirm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtvvplxpxy.html

[Q09] 创建唯一索引
来源：http://hz.cashguo.top/gtehdnwkhc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.mhx1999.top/gtnysozwxl.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtidmptjzd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ywan-chungtsiang.top/gtikudftio.html

[Q11] 一次插入多行
来源：http://hz.dashuyun.cn/gtjixqyibc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtspqvwnac.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtzjtdoywe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtovkmtgbm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gaohongyu789.top/gtlyzyilwh.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtjwgdyahr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yuanzhike.top/gthhatmxqb.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtjlqpbkfr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gtdctbgqoj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yongpay.top/gtepekrnlt.html

[Q15] 查询全部
来源：http://hz.shzxlz.cn/gtkfdmqedb.html

SELECT * FROM users;
来源：http://hz.nanxuanxn.top/gtuhuheaml.html

[Q16] 查询指定列
来源：http://hz.xuanzx.com/gtciwkrsry.html

SELECT id, name FROM users;
来源：http://hz.guannengcc.top/gtbmueieic.html

[Q17] 条件查询
来源：http://hz.andypj.xyz/gteoyopepn.html


<!-- 参考信息 -->