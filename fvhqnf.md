代发 wailian999

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtmdkavomg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtdbezhyxu.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gthriggaqz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtsxozzoan.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtfwwffabz.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtfkbneenj.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtjwvelrav.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtdabwyfxz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtcwtefyqq.html

Ruby: warn "err"
来源：http://hz.jlsjyb.cn/gtcfvrrsgs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtiffbwrzx.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtgimwoxzp.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtciwrktea.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gtancahoyn.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtdimwzain.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtwznxsrnw.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtdmtapgom.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtrwescbep.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtmaumbrgc.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtrsrdiynv.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtsumqwtdy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtmmbmbymt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtentkjxkj.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtvytkkoex.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtkkyhfyca.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.haohaochexian.top/gtzfufjmed.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtbgssuovn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtnysdxclx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtawougcuv.html

================================================================================
来源：http://hz.yuxming.cn/gtgykdhvcc.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtgalbaorm.html

================================================================================
来源：http://hz.smart0.xyz/gtatosepia.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtiscsvwde.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtswmwexjw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sysykeji.top/gtfhuabgeh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtuvxdhzsj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.mhx1999.top/gttvwdebpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.mhx1999.top/gttnwofimk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtzxicswjf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydzc1.top/gtejjucrhl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtymlmnicn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtkpcvcyis.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gttrarjwyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtpzufltcx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtlkojvodk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtvxtnfhej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gteegiacws.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gtcfxrglhb.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gthjdleexm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gthsxlyany.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtvhgeoknm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtlxpuyxwl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtasbhqwlm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtfqngxshc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtmnpwjauw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gtwbklayvm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gttrnxgahl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daria6918.cn/gtvceqdaui.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aibaodan.cn/gtmahyaemo.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gthwtiubkj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtzbqgzdsw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hammf.cn/gtdfjciodv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtlgdciaqi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtseeakyyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtfxwnmwez.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtwoousvrg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtzbjdmmcq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gthcqqvuct.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtfkneayea.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtryotvrzi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258888.top/gttgojxicj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtvduyfzrz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhongyouzk.top/gtrbbjhlen.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtzdrovecf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtkezopzdj.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtkfcirrib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtmqnryfuj.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtqcafmlhu.html

Py:   s == s[::-1]
来源：http://hz.jlsjyb.cn/gtqwpsywnv.html

PHP:  $s === strrev($s);
来源：http://hz.sysykeji.top/gtkjlsmrea.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtinkzpjbb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gtqgbbvwkk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtopqaoefw.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtgkizprqe.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtxjsaonty.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtzuhevqxj.html

[N07] 两数之和（返回下标）
来源：http://hz.52xcode.cn/gtucwcbqoi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtzhvdaupu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtjuiwrczx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtsvonjcut.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtkygvjlwv.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtqguduuux.html

Go:   // 手写 map[int]int
来源：http://hz.cheryme.top/gtjndirusz.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtpduhmfym.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtnwmmjwwz.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtbylifbju.html

Py:   itertools.permutations(arr)
来源：http://hz.birdmap.top/gtsysbhlex.html

PHP:  // 手写递归交换
来源：http://hz.sxryk.cn/gtnapgsmwf.html

JS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtanaxhkai.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gticeznsfl.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtbfyjeqva.html

Go:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtxugglbic.html

Ruby: arr.permutation.to_a
来源：http://hz.zhengqikj.top/gtggabcmai.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtrnclurvd.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gthnqqotpm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtuznpcfbm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtrjbohehd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtucscflop.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtldcjzcbk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtnpgmdbmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtehukyhcw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zycfv.cn/gtezrpecqu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jyoumei.cn/gtsnngzbwj.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gtafjczlyv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtxayqkavl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shanyushiyangtech.top/gtagbryrjd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gthwhjbpwn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtytvccopq.html

Java: class Node { int v; Node next; }
来源：http://hz.ydjk.org.cn/gtpwhxownf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtewyzbrob.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gaohongyu789.top/gtavffqggh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ywan-chungtsiang.top/gtnksxbvfe.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtdewhmtij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xziqi.cn/gtofylynwr.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtrfohgvrh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtfpqtyonj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtjhcanhma.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtspeqcumh.html

Go:   // 手写递归
来源：http://hz.jqgufenzy.top/gturykastf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.0kj1m.cn/gtplfnmsal.html

C#:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtfmkduouz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sysykeji.top/gtgcosysde.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zdqjudy.top/gtcipkdtxm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gthkmudjwj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtvppebzmc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtlovvcago.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtlllvkuth.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtwrgoenbr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.9152youxi.cn/gtzkenaqeh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtaebflyov.html

================================================================================
来源：http://hz.0kj1m.cn/gtzbjjjqkm.html

O. 并发与异步
来源：http://hz.zhixingplan.top/gtowdrwpww.html

================================================================================
来源：http://hz.chenlongwang.top/gtgnydopmr.html

[O01] 启动一个线程
来源：http://hz.cashguo.top/gtaofnefsc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtsxzhsysp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtctqjwdtx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shuidangran.top/gttiwhawfq.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtwbhilhso.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtkkpeviru.html

Go:   go f()
来源：http://hz.jyoumei.cn/gtktkdjugw.html

Ruby: Thread.new { f }
来源：http://hz.nanxinkj.top/gtevxvshyt.html

C#:   Task.Run(() => F());
来源：http://hz.haohaochexian.top/gtnplpdciy.html

[O02] 使用线程池
来源：http://hz.c1oappe.top/gtjqegvhzk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daxiang520.top/gtxleduyun.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zycfv.cn/gtqnisatan.html

JS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtiseronpm.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gttufizygh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258888.top/gtvakkslan.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtgufwyyqq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtgpfdropp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtkqblnxoy.html

[O03] 加锁保护共享数据
来源：http://hz.hnqzz.top/gtxuxgeubx.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gtvnaaavyw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hfpthk.cn/gtfognnunr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtzmevajpi.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gttxlmlkji.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtgwbxabwb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtkghlutoh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenlongwang.top/gtuhtmpzow.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnqzz.top/gtjrnxbrht.html

[O04] 定义异步函数并等待
来源：http://hz.xinyue.icu/gterpnlhnh.html

Py:   async def f():⏎    await g()
来源：http://hz.yuanzhike.top/gtdcpuyqod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.52xcode.cn/gtdmoxxiol.html

JS:   async function f() { await g(); }
来源：http://hz.pycfn.com/gtqjmulfdb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtpmrnsbvw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydzc1.top/gtuzrjjbfg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtkeqhipti.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.wangdashe.top/gtsqxmtgsk.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtqbhcfoov.html

[O05] 并发执行并等待全部完成
来源：http://hz.hnqzz.top/gtvawbmpve.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hywenlv.cn/gtprylzccp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gtmflrlkld.html

JS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtitkjelkz.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtsbnxgtec.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtuinqyjcz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.guowangkeji.top/gtqiyoaotv.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtlngvoiwh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtxzdgbbto.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtvkdtfhuk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sweek.top/gtrifljign.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258.top/gtzssdwomj.html

JS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtwzfannht.html

TS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gttbzrkbqn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtdrxfcbpo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtpycmdvtj.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtbtuzpuqa.html

C#:   Parallel.For
来源：http://hz.daria6918.cn/gtuemnskpe.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgvikfopx.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtowpzmbjk.html

================================================================================
来源：http://hz.sufxvd.cn/gtzbqbcrvt.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtzypftyuf.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gttvlnbmvl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj20258888.top/gtzxikssvv.html

JS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtbtthdlqg.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtwqjtfmfs.html

Java: UUID.randomUUID().toString()
来源：http://hz.c1oappe.top/gtcvdwajiw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jqgufenzy.top/gtwgbrxbac.html

Ruby: SecureRandom.uuid
来源：http://hz.aizwys.cn/gtlavvplxq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sysykeji.top/gtyacikmar.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zycfv.cn/gtfywljjfp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtdfkckryw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtoaejonng.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gtglvdwlff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zdqjudy.top/gttjgeqezw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zdqjudy.top/gtaodfbmzy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hongshengwenyu.top/gtcvsitofi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fengsongda.top/gtrgpnwdhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gtrxuqmols.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtybuvohua.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jianghu66.top/gtqcxovzxr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sweek.top/gtqlcglvjh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yvedp.cn/gtdxeitvgw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtqdysjklj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtoyqiaaoe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj20258.top/gtvsqsjkhi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtvwlyyvpa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fengsongda.top/gtllisioxq.html

[P04] 求长度
来源：http://hz.zhixingplan.top/gtcvcbqwbr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhongyouzk.top/gtcfxtqhfe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtyjtizsxd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shuidangran.top/gtceipboss.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gttwbjdxdu.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtwyfcdqou.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtykqbotqw.html

Ruby: x.length;  x.size
来源：http://hz.jqgufenzy.top/gtyvqfvwzt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtinvjoscg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sufxvd.cn/gtyntspdsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tian-w.cn/gttciirmts.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cucudq.cn/gtzgemyzpg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gthndlwgzb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hywenlv.cn/gtmpfmgpct.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xingfuxueyuan.xyz/gtlryndlwk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daxiang520.top/gtdyjixjwa.html

Ruby: a == b
来源：http://hz.jianghu66.top/gtmdoyztkc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtiyktkrrn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pengpengdd.cyou/gteggpghhq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.316326.xyz/gtawagxbup.html

PHP:  if (empty($x)) {}
来源：http://hz.zhijiandao.cn/gtiwavosom.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xylfe.cn/gtsljnecmu.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtrncrwelk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtwqjdxlyq.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtxnxemnxw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtecqlccwc.html

C#:   if (x is null) {}
来源：http://hz.vqdsnc.cn/gtqofailki.html

[P07] 防抖与节流
来源：http://hz.zhongyouzk.top/gtstsdaxnn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.mhx1999.top/gtsnfxlfiz.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtrohcjljl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jianghu66.top/gtfdsuplrd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtrcxkesiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hnxiangtu.top/gtlgwxkrbc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtxrngbboa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.redwolf501.top/gtucwdffnt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guannengcc.top/gtdvdjpqkf.html

[P08] 处理浮点精度问题
来源：http://hz.xinyue.icu/gtmaeplqlh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhoulong.xyz/gtlqqtpbty.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sxryk.cn/gtjhwsgbqf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ivvv.top/gtiljsabkj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtdvwqawrb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hammf.cn/gthhdprjvy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhongyouzk.top/gtsmonxjbs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgufenzy.top/gtfnbjwmxe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtjfseirfz.html

================================================================================
来源：http://hz.sufxvd.cn/gtvakgowzv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhaomingkeji.xyz/gtngmdnuyg.html

================================================================================
来源：http://hz.redwolf501.top/gtbganhwfr.html

[Q01] 创建表
来源：http://hz.bjfxy.top/gtiztknmwc.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtsxosnlly.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtfqfiarka.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtmodxtmoi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yanxiufei.cn/gtiukzhhpt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gtnnecaxrs.html

);
来源：http://hz.316326.xyz/gttigitorr.html

[Q02] 创建带外键的表
来源：http://hz.0kj1m.cn/gtuebornxy.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtfvlzcahb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtujjpgztf.html

user_id INT NOT NULL,
来源：http://hz.tanke756.top/gteotfzhhb.html

amount DECIMAL(10, 2),
来源：http://hz.9152youxi.cn/gttjuqxcke.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtsjeobpdm.html

);
来源：http://hz.hywenlv.cn/gtugqsniva.html

[Q03] 增加列
来源：http://hz.chenjidiqi.icu/gtfmwqpoew.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.zhiwuduotai.top/gtgficeixm.html

[Q04] 修改列类型
来源：http://hz.guowangkeji.top/gtjwfnrkpu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cqqwz.cn/gtpcnaubdc.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtncbqcfer.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yonumen.top/gtoudlacgg.html

[Q06] 删除列
来源：http://hz.yongpay.top/gtugwyhott.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhongyouzk.top/gtosntglyg.html

[Q07] 删除表
来源：http://hz.feifeiyinyue.top/gtsartrurg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtrqcirfiq.html

[Q08] 创建普通索引
来源：http://hz.zycfv.cn/gtzqzqwbsg.html


<!-- 参考信息 -->