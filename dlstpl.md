代发 wailian999

Ruby: exit 1
来源：http://hz.gzhubu.top/gtzapriall.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtopatjnlw.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtiktcwsmm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtrscxgxog.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gtirmonpee.html

JS:   console.error("err")
来源：http://hz.cashguo.top/gtgmlsjrfl.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtuonjpsux.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtbovekada.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtemeqgdvm.html

Ruby: warn "err"
来源：http://hz.dashuyun.cn/gtodbojtas.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zdqjudy.top/gtdmbkqxhz.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtvovgewgi.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gtkewiwzlb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtwuktxxbt.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtaqevfqge.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtnbaksmge.html

Java: public static void main(String[] args)
来源：http://hz.zhoulong.xyz/gtsipknrtx.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtgshesgnd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtkxnszhtd.html

C#:   static void Main(string[] args)
来源：http://hz.shzxlz.cn/gtfbobsoav.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258888.top/gtqzsgwnzc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gturypuedj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gtmglyylem.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtrexqdpmu.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtjpftaykr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtwpsuqtpp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtlvurbfvl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtjybdxcus.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtmlzhnniq.html

================================================================================
来源：http://hz.cqqwz.cn/gtpwrcszye.html

N. 数据结构与算法
来源：http://hz.cashguo.top/gtkhnrphua.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnnmxznhj.html

[N01] 二分查找（有序数组）
来源：http://hz.jinghuilouyu.cn/gtihyvvwls.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhijiandao.cn/gtjxriaoze.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtmzcbeilb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gthsgegloi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtqlibglhx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gthgailssk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yueranfly.top/gtprqrivfl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtspxwging.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtzkyqlavh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtearwxlwa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtfrszntom.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.birdmap.top/gtijjkomlb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtwqkfudqb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtuwupwsyy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtucwampfw.html

Go:   slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtxizmnwnw.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtsbvhmdin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtcgnqmunx.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtfmsbedio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtvykphlrm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtgyzupwlu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtmdqceyza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gttkcctyqy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gtwddmicuy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gtylejmibl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gtxhdmfvgv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtvjokhcah.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtglxvregs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtwxekdnbq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gtwwqqvdyp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tianlin.xyz/gtcvnjpsud.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtahivnuyz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtruvsaoan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtuhpfmwbp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtocvhdovr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtmqlksful.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtxddnvkel.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtizvoqsjf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.c1oappe.top/gtzrurwwob.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtucuwoyfy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtgbimerqo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yanxiufei.cn/gtwlumbena.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtlbbgjpto.html

Ruby: a.gcd(b)
来源：http://hz.ybcxt.top/gttgqcxvte.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gtpdhbefwi.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gtcaebeimb.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtivoofjdn.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gthzgbgjnb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtwtjubvuy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gthtialhcs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxuanxn.top/gtvyelvqaa.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtpinzbert.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtbuhupatj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtfoubtxsl.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258.top/gteelajcwp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtzfdmzmco.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtdyrultvd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtxnekbyuh.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtyfnpwpey.html

Java: // 手写 HashMap
来源：http://hz.sysykeji.top/gttfoetlvo.html

Go:   // 手写 map[int]int
来源：http://hz.dashuyun.cn/gttpxpjtof.html

Ruby: // 手写 Hash
来源：http://hz.chenlongwang.top/gtdhnrvabk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhongyouzk.top/gthlktwkuc.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtdbltkiuy.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtxythitww.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtovipygye.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtsnuycjds.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtwkavcxmq.html

Java: // 手写回溯递归
来源：http://hz.yvedp.cn/gtpfdvdjbo.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtifsjjlku.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtavsgcghm.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtfgxwfcyy.html

[N09] 栈与队列
来源：http://hz.aizwys.cn/gtjcnkaqal.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gthrpftccj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.snrcjt.cn/gtwesvusfu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtmnzdqhio.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tianlin.xyz/gtelmmarts.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gtyiipshjo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gthrnabsih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtfhuzpyql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtzwahvnhz.html

[N10] 链表节点定义
来源：http://hz.nwbrower.top/gtwmnglxtm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtxantemzc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gtoqrrdkjw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhaomingkeji.xyz/gtkadsznkc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhixingplan.top/gtoddpxpxh.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gttdvvvicy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zdqjudy.top/gtjihkhxbq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.0kj1m.cn/gtxpxmwanc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtfldzmoji.html

[N11] 二叉树中序遍历
来源：http://hz.snrcjt.cn/gtblljzupj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtupaazira.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtiztewcbm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtcbuyezcn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtycbvqjgk.html

Java: // 手写递归
来源：http://hz.nanxinkj.top/gtojckdemq.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtzzsrobyj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gthxdliulj.html

C#:   // 手写递归
来源：http://hz.xylfe.cn/gtbjifxkbg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtodpnayee.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtleqlrquy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtlfqsmjpe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtugvdltxm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtgwsuloah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtqbsuiixg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuanzhike.top/gttxyozsmd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gtlhkpddaa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtcbkupqus.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnsxiibyu.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtdglgbvtb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwbfqrffe.html

[O01] 启动一个线程
来源：http://hz.redwolf501.top/gtlrvmbisa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hfpthk.cn/gttdjeflcu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtzegqgklw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtpztrpmqd.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtxjinucwl.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtdjghswus.html

Go:   go f()
来源：http://hz.feifeiyinyue.top/gtxorphaen.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtelajazjj.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtwoobgefz.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gtexiewavz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zycfv.cn/gtaihgheow.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtxmsckkdk.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtjbxscjiw.html

TS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtdqidosqa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gtpoxdpvuu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gtsxyymxkj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtdvffjnly.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtxqgzmgds.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtmoikelgo.html

Py:   with lock: shared += 1
来源：http://hz.zdqjudy.top/gtnlsbmboy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtncdrxrwr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenlongwang.top/gtnwfzxqsn.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gthjkasisa.html

Java: synchronized (this) { shared++; }
来源：http://hz.vqdsnc.cn/gtprmjnxit.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tianlin.xyz/gtdehfolgd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gtjxagnwcc.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtmkqdkhto.html

[O04] 定义异步函数并等待
来源：http://hz.xziqi.cn/gtyaxprzfj.html

Py:   async def f():⏎    await g()
来源：http://hz.chenjidiqi.icu/gtdxfushff.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.aizwys.cn/gtihqrasxp.html

JS:   async function f() { await g(); }
来源：http://hz.gzhubu.top/gtpewwfjui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.andypj.xyz/gtwcpnmkhg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgufenzy.top/gtycpffyob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xylfe.cn/gtovsnjivp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ivvv.top/gtjtsdsqbp.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gtmezynfbv.html

[O05] 并发执行并等待全部完成
来源：http://hz.nanxuanxn.top/gtgpehebmw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.c1oappe.top/gtjpxjmygo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yangfankeji.com/gtkfoqcazv.html

JS:   await Promise.all(tasks)
来源：http://hz.gzhubu.top/gtjbkortrt.html

TS:   await Promise.all(tasks)
来源：http://hz.tianlin.xyz/gtxwxurkdb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtdpjalgxc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gttczydauh.html

Ruby: threads.map(&:join)
来源：http://hz.zhiwuduotai.top/gttyhyoycy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtmiwjazlt.html

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtnwnxznbp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aibaodan.cn/gtdpswdirb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtmdesryva.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtlprjphlu.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtdsotisuc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zycfv.cn/gttlwckvtq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtjnffzegz.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtzswlwlbs.html

C#:   Parallel.For
来源：http://hz.hammf.cn/gtnqyuqjit.html

================================================================================
来源：http://hz.yuxming.cn/gtrzdyqmwy.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtovctoion.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvoujbpst.html

[P01] 生成 UUID
来源：http://hz.jyoumei.cn/gtyrdtpxlv.html

Py:   str(uuid.uuid4())
来源：http://hz.52xcode.cn/gtkcqfqxnl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jyoumei.cn/gtygxgurwc.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtthqdctgx.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtrkvojcbc.html

Java: UUID.randomUUID().toString()
来源：http://hz.mhx1999.top/gtyawwupgl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yueranfly.top/gtynbxnlhu.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gtwnxdevvk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daxiang520.top/gtlxwuwywc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenzaomai.com/gthfbscfsb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuanzx.com/gtkfcbeltd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtvcxlwnwh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.snrcjt.cn/gthsjyvdev.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtzngjazcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtagsnvujd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gtdlwcgwbj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtdlrtpxxa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtzuloefpg.html

[P03] 生成短随机字符串
来源：http://hz.gotoacloud.top/gtsayowkjx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guannengcc.top/gtveswodzm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tian-w.cn/gtzougohky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtamezplmy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtvorfftgf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtozuyzfob.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtmdxbtsaw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gtcwoqrvbe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtcvjwaibq.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtdyzfthan.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtkzhbpjgc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtjyrlxpnb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtojxzxthp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtepryusxr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtuzpzbflv.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtxlhehliv.html

Ruby: x.length;  x.size
来源：http://hz.c1oappe.top/gtvqrieuuj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fzhhl.top/gtfdkpcpmc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhoulong.xyz/gtdybtaoom.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daxiang520.top/gtbazsgpjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yvedp.cn/gthkxsvtcd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gtpgkromnh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.kuanghao11.cn/gtlnzyyinh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydjk.org.cn/gtpzytqnwy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hammf.cn/gtzypubihm.html

Ruby: a == b
来源：http://hz.chenzaomai.com/gtgkwyswru.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.feifeiyinyue.top/gtgiosibcl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtuofftyry.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtfwztdqoy.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gtmhoaypaz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aibaodan.cn/gttmpdovmv.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtcrlktbjw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtyizoenba.html

Go:   if x == nil {}
来源：http://hz.zhijiandao.cn/gtqoqanoox.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yuxming.cn/gtmkymgegq.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtaukzlvid.html

[P07] 防抖与节流
来源：http://hz.jinghuilouyu.cn/gtvvxifxmm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhongyouzk.top/gttrifhehl.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtjynhacxg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtfvixfvvz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtnqqbvyax.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.snrcjt.cn/gtdetwyshl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtgxunxmlg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.bjfxy.top/gtniqmaecq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtiwwsimjw.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtctmdxjmr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guannengcc.top/gtovislqdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.andypj.xyz/gttyshjfzc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sufxvd.cn/gtemeabaga.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj202588.top/gtrphzizrh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jianghu66.top/gtcsbswcwp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.quarkkingdee.top/gtciudpgoh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtbdsssbbl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtynxdxidk.html

================================================================================
来源：http://hz.yj202588.top/gtkhcmugqb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangshuangyany.cn/gtcsulphdj.html

================================================================================
来源：http://hz.ydzc1.top/gtkqjfahvv.html

[Q01] 创建表
来源：http://hz.tanke756.top/gtyrmfjntn.html

CREATE TABLE users (
来源：http://hz.quarkkingdee.top/gtcqrhwdgj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtwjtynpkg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.smart0.xyz/gtogbyoylh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.316326.xyz/gtpgdmbvom.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtnlkoyigh.html

);
来源：http://hz.shzxlz.cn/gttcondwwm.html

[Q02] 创建带外键的表
来源：http://hz.vqdsnc.cn/gtqeikuten.html

CREATE TABLE orders (
来源：http://hz.snrcjt.cn/gtrdokmpju.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtklexfrbf.html

user_id INT NOT NULL,
来源：http://hz.jinqigufen.top/gthkcjttbb.html

amount DECIMAL(10, 2),
来源：http://hz.ppjwa.cn/gtcfpvdbhf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtexusorfq.html

);
来源：http://hz.hnxiangtu.top/gtxcvespkc.html

[Q03] 增加列
来源：http://hz.gogol.net.cn/gttgtsxqfp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtxxotggkh.html

[Q04] 修改列类型
来源：http://hz.zhongyouzk.top/gtkxpofpbf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtmjcjijdb.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtovjmtbrm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.vqdsnc.cn/gtofviuczb.html

[Q06] 删除列
来源：http://hz.ivvv.top/gtarmvkijr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangtech.top/gtjtqdcmwt.html

[Q07] 删除表
来源：http://hz.zdqjudy.top/gtxnaalmrm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtokfhgexl.html

[Q08] 创建普通索引
来源：http://hz.jinyuanbaomall.cn/gtqxhvhrer.html


<!-- 参考信息 -->