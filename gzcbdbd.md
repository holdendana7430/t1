代发 wailian999

Py:   resp.json()
来源：http://rb.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://lp.shxzukj.cn

JS:   await resp.json()
来源：http://ls.shxzskj.cn

TS:   await resp.json()
来源：http://ck.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ha.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ve.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://oh.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xf.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://vd.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sl.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cz.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://bv.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://hd.haigaiapp.cn

Java: resp.statusCode()
来源：http://up.gzmigu.cn

Go:   resp.StatusCode
来源：http://wl.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://iz.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://ew.nicolike.cn

[L08] 并发请求多个地址
来源：http://bn.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yj.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://vx.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://va.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oj.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vr.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mk.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fm.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ix.asd995.cn

================================================================================
来源：http://de.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://kl.huixiangedu.cn

================================================================================
来源：http://gj.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://wi.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://hp.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://yr.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://tc.hahajie.cn

TS:   process.argv.slice(2)
来源：http://hp.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://ly.lnxyls.cn

Go:   os.Args[1:]
来源：http://fw.shtwfgs.cn

Ruby: ARGV
来源：http://ka.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ze.bookmarksfly.cn

[M02] 读取环境变量
来源：http://cn.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://yx.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eo.gzmigu.cn

JS:   process.env.HOME
来源：http://zt.colortex.cn

TS:   process.env.HOME
来源：http://sr.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://zj.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tz.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://td.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ci.wgjwhj.cn

[M03] 执行外部命令
来源：http://iw.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ye.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://be.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zp.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ep.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qx.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eb.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://se.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://hf.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://bj.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://bz.jianghongdianzi.cn

PHP:  getcwd();
来源：http://bw.lnxyls.cn

JS:   process.cwd()
来源：http://xy.bjjhwx.cn

TS:   process.cwd()
来源：http://bn.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wt.9csxet.cn

Go:   os.Getwd()
来源：http://xs.nicolike.cn

Ruby: Dir.pwd
来源：http://qo.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://om.colortex.cn

[M05] 设置退出码
来源：http://gr.jctech888.com.cn

Py:   sys.exit(1)
来源：http://mv.9csxet.cn

PHP:  exit(1);
来源：http://vz.panjiajie.cn

JS:   process.exit(1)
来源：http://lk.szsharing.cn

TS:   process.exit(1)
来源：http://vm.nszjky.cn

Java: System.exit(1)
来源：http://sc.gzmigu.cn

Go:   os.Exit(1)
来源：http://vg.muxihuayi.cn

Ruby: exit 1
来源：http://ld.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pi.muxihuayi.cn

[M06] 向标准错误输出
来源：http://zs.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://am.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vb.szsharing.cn

JS:   console.error("err")
来源：http://zk.colortex.cn

TS:   console.error("err")
来源：http://pw.yuexingan06.cn

Java: System.err.println("err")
来源：http://zx.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ah.lnxyls.cn

Ruby: warn "err"
来源：http://ds.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://ur.gzmigu.cn

[M07] 判断是否为主入口
来源：http://xn.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://hk.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ru.szxytkj.cn

JS:   require.main === module
来源：http://ce.panjiajie.cn

TS:   require.main === module
来源：http://gr.asd995.cn

Java: public static void main(String[] args)
来源：http://fe.hnjuh.cn

Go:   func main()
来源：http://wy.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://us.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://re.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://eh.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://ls.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://jn.shxzukj.cn

JS:   process.platform;  process.version
来源：http://sb.521024.cn

TS:   process.platform;  process.version
来源：http://xc.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qs.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qw.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wt.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cp.muxihuayi.cn

================================================================================
来源：http://yn.szsharing.cn

N. 数据结构与算法
来源：http://dm.shxzskj.cn

================================================================================
来源：http://ky.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://ku.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gl.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jk.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tc.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tt.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://yc.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yt.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ot.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://ib.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://sm.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ck.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ps.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oa.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wh.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://gp.shxzukj.cn

Ruby: arr.sort
来源：http://hp.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yi.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://cv.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xj.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://qv.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nu.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zj.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rs.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lz.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tl.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gc.haigaiapp.cn

[N04] 斐波那契数列
来源：http://cm.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://td.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ys.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hl.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gz.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ae.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ye.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ub.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ec.chemitech.net.cn

[N05] 最大公约数
来源：http://pp.asd995.cn

Py:   math.gcd(a, b)
来源：http://jz.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sw.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fr.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xz.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bv.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://px.521024.cn

Ruby: a.gcd(b)
来源：http://at.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vr.lnxyls.cn

[N06] 判断回文字符串
来源：http://kd.shxzskj.cn

Py:   s == s[::-1]
来源：http://tg.9csxet.cn

PHP:  $s === strrev($s);
来源：http://qb.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://wb.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://eb.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ze.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://yg.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://kz.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hv.colortex.cn

[N07] 两数之和（返回下标）
来源：http://wc.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pp.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://my.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://we.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://bf.haigaiapp.cn

Java: // 手写 HashMap
来源：http://jv.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://sg.lnxyls.cn

Ruby: // 手写 Hash
来源：http://ls.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mn.nicolike.cn

[N08] 生成全排列
来源：http://ge.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://rn.521024.cn

PHP:  // 手写递归交换
来源：http://rz.asd995.cn

JS:   // 手写回溯递归
来源：http://mz.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://us.shtwfgs.cn

Java: // 手写回溯递归
来源：http://kh.hnjuh.cn

Go:   // 手写回溯递归
来源：http://xb.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://yb.shxzskj.cn

C#:   // 手写回溯递归
来源：http://on.haigaiapp.cn

[N09] 栈与队列
来源：http://vi.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yb.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ii.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yd.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lo.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://av.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bu.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ze.wgjwhj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sy.9csxet.cn

[N10] 链表节点定义
来源：http://br.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sm.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wy.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fs.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://or.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://dd.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xj.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zr.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vc.asd995.cn

[N11] 二叉树中序遍历
来源：http://jd.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qh.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://qu.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gy.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gv.shxzskj.cn

Java: // 手写递归
来源：http://gt.huanxung.cn

Go:   // 手写递归
来源：http://dg.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qf.nszjky.cn

C#:   // 手写递归
来源：http://tp.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vd.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ut.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nr.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ey.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kl.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mo.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fz.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eo.asd995.cn

================================================================================
来源：http://hb.szsharing.cn

O. 并发与异步
来源：http://xp.yuexingan06.cn

================================================================================
来源：http://qm.haigaiapp.cn

[O01] 启动一个线程
来源：http://rx.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zo.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xg.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kd.colortex.cn

TS:   // 同 JS
来源：http://tn.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://xi.muxihuayi.cn

Go:   go f()
来源：http://ut.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ms.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://bg.jctech888.com.cn

[O02] 使用线程池
来源：http://jb.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fp.yuexingan06.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gh.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://wd.9csxet.cn

TS:   // worker_threads 线程池
来源：http://xy.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dt.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xa.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qy.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://st.nszjky.cn

[O03] 加锁保护共享数据
来源：http://nj.huanxung.cn

Py:   with lock: shared += 1
来源：http://kq.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://kg.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ps.shxzukj.cn

TS:   // 同 JS
来源：http://mh.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://rd.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yk.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://td.panjiajie.cn

C#:   lock (gate) { shared++; }
来源：http://ti.newstarts.cn

[O04] 定义异步函数并等待
来源：http://el.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://wb.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kq.9csxet.cn

JS:   async function f() { await g(); }
来源：http://zs.nicolike.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zj.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yz.wgjwhj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tl.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ny.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://gk.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://tw.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://la.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tq.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://es.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://qg.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ps.nicolike.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pu.szsharing.cn

Ruby: threads.map(&:join)
来源：http://dz.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xe.wgjwhj.cn

[O06] 使用进程池
来源：http://gc.huixiangedu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://br.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ik.asd995.cn

JS:   // child_process / cluster 模块
来源：http://ae.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://tf.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ox.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jr.wgjwhj.cn

Ruby: // fork 块
来源：http://gk.muxihuayi.cn

C#:   Parallel.For
来源：http://xg.bookmarksfly.cn

================================================================================
来源：http://cf.jianghongdianzi.cn

P. 常用工具函数
来源：http://zx.panjiajie.cn

================================================================================
来源：http://mt.colortex.cn

[P01] 生成 UUID
来源：http://ji.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://na.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xx.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://ls.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://hz.shxzukj.cn

Java: UUID.randomUUID().toString()
来源：http://hu.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://az.muxihuayi.cn

Ruby: SecureRandom.uuid
来源：http://pc.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://gz.colortex.cn

[P02] MD5 / SHA256 摘要
来源：http://fp.hnjuh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uj.muxihuayi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hg.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ay.huixinmuqiang.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fn.jctech888.com.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zv.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dr.shxzukj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://va.newstarts.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yr.jctech888.com.cn

[P03] 生成短随机字符串
来源：http://tf.huixiangedu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wh.hnjuh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jp.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ad.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hi.bjjhwx.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tg.panjiajie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rc.yuntaijiaju.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://og.9csxet.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zk.bjjhwx.cn

[P04] 求长度
来源：http://pz.shxzukj.cn


<!-- 参考信息 -->