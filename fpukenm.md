代发 wailian999

Py:   resp.json()
来源：http://er.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://dm.wgjwhj.cn

JS:   await resp.json()
来源：http://vf.shtwfgs.cn

TS:   await resp.json()
来源：http://yl.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nb.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vs.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://jc.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qa.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://nu.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hi.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aa.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://ah.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://cu.colortex.cn

Java: resp.statusCode()
来源：http://vd.colortex.cn

Go:   resp.StatusCode
来源：http://ax.shxzskj.cn

Ruby: resp.code.to_i
来源：http://qq.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://il.shxzskj.cn

[L08] 并发请求多个地址
来源：http://rq.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mt.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://pg.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ld.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ps.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fs.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rp.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nq.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cz.szxytkj.cn

================================================================================
来源：http://dx.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://pu.hnjuh.cn

================================================================================
来源：http://bg.shtwfgs.cn

[M01] 读取命令行参数
来源：http://vj.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://wq.nicolike.cn

PHP:  $argv;  $argc;
来源：http://rt.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://pc.newstarts.cn

TS:   process.argv.slice(2)
来源：http://hg.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://ke.asd995.cn

Go:   os.Args[1:]
来源：http://of.szsharing.cn

Ruby: ARGV
来源：http://dq.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://vc.hahajie.cn

[M02] 读取环境变量
来源：http://bl.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://qx.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mh.nicolike.cn

JS:   process.env.HOME
来源：http://mt.wgjwhj.cn

TS:   process.env.HOME
来源：http://ak.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://hc.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://it.asd995.cn

Ruby: ENV["HOME"]
来源：http://ha.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hb.hnjuh.cn

[M03] 执行外部命令
来源：http://vi.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://og.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vc.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ub.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xb.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ou.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qd.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jm.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://xm.szsharing.cn

Py:   os.getcwd()
来源：http://cm.muxihuayi.cn

PHP:  getcwd();
来源：http://oa.jianghongdianzi.cn

JS:   process.cwd()
来源：http://nu.lnxyls.cn

TS:   process.cwd()
来源：http://xq.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://bl.muxihuayi.cn

Go:   os.Getwd()
来源：http://jq.szxytkj.cn

Ruby: Dir.pwd
来源：http://lx.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gg.shtwfgs.cn

[M05] 设置退出码
来源：http://pm.gzmigu.cn

Py:   sys.exit(1)
来源：http://ex.huixinmuqiang.cn

PHP:  exit(1);
来源：http://ep.lnxyls.cn

JS:   process.exit(1)
来源：http://fi.lnxyls.cn

TS:   process.exit(1)
来源：http://iu.yuntaijiaju.cn

Java: System.exit(1)
来源：http://dl.szsharing.cn

Go:   os.Exit(1)
来源：http://rs.chemitech.net.cn

Ruby: exit 1
来源：http://pw.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://za.gzmigu.cn

[M06] 向标准错误输出
来源：http://ll.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://cn.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aq.shxzskj.cn

JS:   console.error("err")
来源：http://ba.jianghongdianzi.cn

TS:   console.error("err")
来源：http://cs.bjjhwx.cn

Java: System.err.println("err")
来源：http://ml.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://la.521024.cn

Ruby: warn "err"
来源：http://kx.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://jl.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://jz.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://aa.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zo.panjiajie.cn

JS:   require.main === module
来源：http://dz.gzmigu.cn

TS:   require.main === module
来源：http://ka.newstarts.cn

Java: public static void main(String[] args)
来源：http://de.huixiangedu.cn

Go:   func main()
来源：http://ql.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://au.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://pg.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://dc.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://st.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.szxytkj.cn

JS:   process.platform;  process.version
来源：http://qu.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://bx.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zf.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yk.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dc.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.shxzukj.cn

================================================================================
来源：http://xf.panjiajie.cn

N. 数据结构与算法
来源：http://xz.nicolike.cn

================================================================================
来源：http://cj.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://lh.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://su.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sp.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yc.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oj.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ee.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://hz.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ox.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fi.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://rr.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cr.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yk.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hi.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://us.asd995.cn

Go:   slices.Sort(arr)
来源：http://lt.nicolike.cn

Ruby: arr.sort
来源：http://em.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://br.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://kj.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mk.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://qj.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pq.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rf.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ab.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ab.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://of.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tz.hnjuh.cn

[N04] 斐波那契数列
来源：http://lx.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://af.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bf.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kl.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bp.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jw.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yr.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://td.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pe.jctech888.com.cn

[N05] 最大公约数
来源：http://kw.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://kv.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vo.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vd.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://al.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nk.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wj.huanxung.cn

Ruby: a.gcd(b)
来源：http://in.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://li.szxytkj.cn

[N06] 判断回文字符串
来源：http://kd.hahajie.cn

Py:   s == s[::-1]
来源：http://km.huanxung.cn

PHP:  $s === strrev($s);
来源：http://or.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://lm.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://rj.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://za.hahajie.cn

Go:   // 双指针从两端比较
来源：http://xn.9csxet.cn

Ruby: s == s.reverse
来源：http://vk.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uj.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://gc.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dj.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fj.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jr.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://gx.lnxyls.cn

Java: // 手写 HashMap
来源：http://il.huanxung.cn

Go:   // 手写 map[int]int
来源：http://ib.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://rf.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://my.shxzukj.cn

[N08] 生成全排列
来源：http://yl.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://qa.shxzskj.cn

PHP:  // 手写递归交换
来源：http://cl.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://sh.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ca.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://sv.szsharing.cn

Go:   // 手写回溯递归
来源：http://ja.colortex.cn

Ruby: arr.permutation.to_a
来源：http://cg.newstarts.cn

C#:   // 手写回溯递归
来源：http://qf.bookmarksfly.cn

[N09] 栈与队列
来源：http://kd.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wo.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pf.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ak.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rc.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uw.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ht.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ys.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://od.bookmarksfly.cn

[N10] 链表节点定义
来源：http://vs.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ar.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cb.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dd.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ai.colortex.cn

Java: class Node { int v; Node next; }
来源：http://lx.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zi.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yz.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sz.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://qb.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ej.panjiajie.cn

PHP:  // 手写递归函数
来源：http://em.gzmigu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fm.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ka.muxihuayi.cn

Java: // 手写递归
来源：http://on.szsharing.cn

Go:   // 手写递归
来源：http://ea.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nn.lnxyls.cn

C#:   // 手写递归
来源：http://lk.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ym.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yb.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jx.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://io.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ld.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cd.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ma.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mb.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ym.szxytkj.cn

================================================================================
来源：http://jw.jctech888.com.cn

O. 并发与异步
来源：http://qh.hnjuh.cn

================================================================================
来源：http://ag.hahajie.cn

[O01] 启动一个线程
来源：http://pk.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zl.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://du.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gs.hahajie.cn

TS:   // 同 JS
来源：http://sa.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://ns.newstarts.cn

Go:   go f()
来源：http://mv.colortex.cn

Ruby: Thread.new { f }
来源：http://px.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://vy.huanxung.cn

[O02] 使用线程池
来源：http://tf.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zq.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sx.hahajie.cn

JS:   // worker_threads 线程池
来源：http://lq.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://tm.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lm.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sx.wgjwhj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vs.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yl.9csxet.cn

[O03] 加锁保护共享数据
来源：http://oo.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://cw.colortex.cn

PHP:  // 用 flock() 做文件锁
来源：http://tb.shxzskj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mg.asd995.cn

TS:   // 同 JS
来源：http://eg.wgjwhj.cn

Java: synchronized (this) { shared++; }
来源：http://in.lnxyls.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rq.szsharing.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lz.shxzukj.cn

C#:   lock (gate) { shared++; }
来源：http://dq.colortex.cn

[O04] 定义异步函数并等待
来源：http://oj.hnjuh.cn

Py:   async def f():⏎    await g()
来源：http://ge.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shxzskj.cn

JS:   async function f() { await g(); }
来源：http://pu.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qc.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xy.nszjky.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ro.jctech888.com.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hu.newstarts.cn

C#:   async Task F() { await G(); }
来源：http://yr.gzmigu.cn

[O05] 并发执行并等待全部完成
来源：http://uv.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://uv.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://en.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://zm.huanxung.cn

TS:   await Promise.all(tasks)
来源：http://zl.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ol.521024.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pg.chemitech.net.cn

Ruby: threads.map(&:join)
来源：http://qi.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tr.jctech888.com.cn

[O06] 使用进程池
来源：http://py.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://st.muxihuayi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uj.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://vy.521024.cn

TS:   // child_process / cluster 模块
来源：http://bl.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sm.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lt.yuntaijiaju.cn

Ruby: // fork 块
来源：http://uh.muxihuayi.cn

C#:   Parallel.For
来源：http://id.muxihuayi.cn

================================================================================
来源：http://jk.jctech888.com.cn

P. 常用工具函数
来源：http://br.chemitech.net.cn

================================================================================
来源：http://vj.hahajie.cn

[P01] 生成 UUID
来源：http://kj.nszjky.cn

Py:   str(uuid.uuid4())
来源：http://bj.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xp.huanxung.cn

JS:   crypto.randomUUID()
来源：http://zj.wgjwhj.cn

TS:   crypto.randomUUID()
来源：http://ux.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://pi.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://ww.jctech888.com.cn

Ruby: SecureRandom.uuid
来源：http://mc.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://hb.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://yc.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ii.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ax.muxihuayi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bc.panjiajie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ha.lnxyls.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wj.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bc.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qh.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lq.huixinmuqiang.cn

[P03] 生成短随机字符串
来源：http://ld.lnxyls.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lw.colortex.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qd.jctech888.com.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wj.szsharing.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cp.yuntaijiaju.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ki.haigaiapp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gm.muxihuayi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zi.szxytkj.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mi.szxytkj.cn

[P04] 求长度
来源：http://rs.jctech888.com.cn


<!-- 参考信息 -->