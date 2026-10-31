代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eh.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gc.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bk.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ht.lnxyls.cn

Py:   resp.json()
来源：http://zh.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://gk.jianghongdianzi.cn

JS:   await resp.json()
来源：http://ew.colortex.cn

TS:   await resp.json()
来源：http://ew.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://px.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hj.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://fd.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fl.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://fk.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lk.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zv.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://by.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ed.asd995.cn

Java: resp.statusCode()
来源：http://de.szsharing.cn

Go:   resp.StatusCode
来源：http://ar.shxzskj.cn

Ruby: resp.code.to_i
来源：http://qu.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://za.nicolike.cn

[L08] 并发请求多个地址
来源：http://ob.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ya.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://am.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bp.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://up.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pl.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wd.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ai.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lv.shtwfgs.cn

================================================================================
来源：http://sq.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://qh.asd995.cn

================================================================================
来源：http://cm.hahajie.cn

[M01] 读取命令行参数
来源：http://km.nszjky.cn

Py:   sys.argv[1:]
来源：http://mu.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://th.9csxet.cn

JS:   process.argv.slice(2)
来源：http://wb.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://yj.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://gr.wgjwhj.cn

Go:   os.Args[1:]
来源：http://pc.gzmigu.cn

Ruby: ARGV
来源：http://dg.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://ij.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://al.colortex.cn

Py:   os.environ.get("HOME")
来源：http://qq.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uh.huixiangedu.cn

JS:   process.env.HOME
来源：http://ut.newstarts.cn

TS:   process.env.HOME
来源：http://bb.szxytkj.cn

Java: System.getenv("HOME")
来源：http://it.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eq.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://wz.newstarts.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gd.yuexingan06.cn

[M03] 执行外部命令
来源：http://rq.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wp.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://et.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zd.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gf.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://su.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nt.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hs.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://zk.panjiajie.cn

[M04] 获取当前工作目录
来源：http://jn.jctech888.com.cn

Py:   os.getcwd()
来源：http://be.huanxung.cn

PHP:  getcwd();
来源：http://sw.shxzukj.cn

JS:   process.cwd()
来源：http://kg.gzmigu.cn

TS:   process.cwd()
来源：http://hw.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://eo.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://yp.haigaiapp.cn

Ruby: Dir.pwd
来源：http://rv.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mc.panjiajie.cn

[M05] 设置退出码
来源：http://yz.colortex.cn

Py:   sys.exit(1)
来源：http://tn.haigaiapp.cn

PHP:  exit(1);
来源：http://vj.jctech888.com.cn

JS:   process.exit(1)
来源：http://rm.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ds.asd995.cn

Java: System.exit(1)
来源：http://yx.shxzskj.cn

Go:   os.Exit(1)
来源：http://ft.yuexingan06.cn

Ruby: exit 1
来源：http://pd.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ur.huanxung.cn

[M06] 向标准错误输出
来源：http://mj.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ap.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ml.wgjwhj.cn

JS:   console.error("err")
来源：http://vx.asd995.cn

TS:   console.error("err")
来源：http://eo.shxzukj.cn

Java: System.err.println("err")
来源：http://ce.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wo.yuntaijiaju.cn

Ruby: warn "err"
来源：http://sb.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ey.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://ci.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://ua.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://in.hahajie.cn

JS:   require.main === module
来源：http://rs.jctech888.com.cn

TS:   require.main === module
来源：http://bi.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://rt.shxzukj.cn

Go:   func main()
来源：http://if.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ua.9csxet.cn

C#:   static void Main(string[] args)
来源：http://gz.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://px.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://nc.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://sc.lnxyls.cn

JS:   process.platform;  process.version
来源：http://ko.szsharing.cn

TS:   process.platform;  process.version
来源：http://xv.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vm.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mk.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nm.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ms.shxzskj.cn

================================================================================
来源：http://lh.yuexingan06.cn

N. 数据结构与算法
来源：http://hm.huixiangedu.cn

================================================================================
来源：http://zf.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://xl.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wz.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rc.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dm.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ys.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wh.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://kx.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jx.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dn.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://nq.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://nh.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ue.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ll.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mr.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ku.9csxet.cn

Go:   slices.Sort(arr)
来源：http://uz.huanxung.cn

Ruby: arr.sort
来源：http://nz.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fe.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://vg.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cq.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://og.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xh.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lo.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bi.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sa.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qy.huixiangedu.cn

[N04] 斐波那契数列
来源：http://jm.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://md.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cn.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rv.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uc.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ef.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lo.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kd.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ik.bookmarksfly.cn

[N05] 最大公约数
来源：http://co.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://gt.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kx.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://li.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://np.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vl.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://ga.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://py.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://fd.bjjhwx.cn

Py:   s == s[::-1]
来源：http://do.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://ab.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://mc.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://lb.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lm.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://od.huanxung.cn

Ruby: s == s.reverse
来源：http://vh.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bt.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://zp.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nd.jianghongdianzi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yc.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ds.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://hd.hahajie.cn

Java: // 手写 HashMap
来源：http://om.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://ub.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://qb.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xi.yuntaijiaju.cn

[N08] 生成全排列
来源：http://ml.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://rj.newstarts.cn

PHP:  // 手写递归交换
来源：http://cd.szxytkj.cn

JS:   // 手写回溯递归
来源：http://xi.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://jz.hahajie.cn

Java: // 手写回溯递归
来源：http://ir.huanxung.cn

Go:   // 手写回溯递归
来源：http://lc.521024.cn

Ruby: arr.permutation.to_a
来源：http://og.9csxet.cn

C#:   // 手写回溯递归
来源：http://ga.hnjuh.cn

[N09] 栈与队列
来源：http://mo.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rz.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://so.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tj.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://il.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pu.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cr.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gg.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kq.panjiajie.cn

[N10] 链表节点定义
来源：http://fp.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fg.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sq.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tu.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ve.bookmarksfly.cn

Java: class Node { int v; Node next; }
来源：http://hj.nicolike.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lv.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fr.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ob.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://nt.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nu.gzmigu.cn

PHP:  // 手写递归函数
来源：http://jx.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wx.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cu.nszjky.cn

Java: // 手写递归
来源：http://vm.521024.cn

Go:   // 手写递归
来源：http://ya.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gj.shxzskj.cn

C#:   // 手写递归
来源：http://jc.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xi.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ty.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hh.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://za.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tj.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://au.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nm.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aq.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gv.nszjky.cn

================================================================================
来源：http://jv.panjiajie.cn

O. 并发与异步
来源：http://rx.jctech888.com.cn

================================================================================
来源：http://he.bjjhwx.cn

[O01] 启动一个线程
来源：http://gx.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iu.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ig.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yw.jianghongdianzi.cn

TS:   // 同 JS
来源：http://xg.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://yj.yuntaijiaju.cn

Go:   go f()
来源：http://lj.9csxet.cn

Ruby: Thread.new { f }
来源：http://mn.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://fb.9csxet.cn

[O02] 使用线程池
来源：http://sh.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oo.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wb.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://vg.newstarts.cn

TS:   // worker_threads 线程池
来源：http://jy.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bu.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xj.gzmigu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sj.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://sb.jianghongdianzi.cn

Py:   with lock: shared += 1
来源：http://jw.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://sg.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fv.newstarts.cn

TS:   // 同 JS
来源：http://vu.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://aq.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ps.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://me.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://rd.yuntaijiaju.cn

[O04] 定义异步函数并等待
来源：http://km.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://ud.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tl.szsharing.cn

JS:   async function f() { await g(); }
来源：http://ju.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hk.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pa.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zd.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vy.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://yg.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://xd.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://xv.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://al.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://sy.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://ak.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qq.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hc.huixinmuqiang.cn

Ruby: threads.map(&:join)
来源：http://zc.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://il.yuntaijiaju.cn

[O06] 使用进程池
来源：http://fk.jctech888.com.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rv.huixinmuqiang.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gf.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://jj.521024.cn

TS:   // child_process / cluster 模块
来源：http://bl.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://se.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ib.colortex.cn

Ruby: // fork 块
来源：http://yn.colortex.cn

C#:   Parallel.For
来源：http://wa.521024.cn

================================================================================
来源：http://kb.huanxung.cn

P. 常用工具函数
来源：http://rh.jianghongdianzi.cn

================================================================================
来源：http://vt.asd995.cn

[P01] 生成 UUID
来源：http://bk.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://yk.panjiajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pg.szsharing.cn

JS:   crypto.randomUUID()
来源：http://lc.newstarts.cn

TS:   crypto.randomUUID()
来源：http://sa.shxzskj.cn

Java: UUID.randomUUID().toString()
来源：http://lq.colortex.cn

Go:   // 用 github.com/google/uuid
来源：http://cs.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://sb.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://vq.nicolike.cn

[P02] MD5 / SHA256 摘要
来源：http://ye.asd995.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://js.asd995.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ht.yuexingan06.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ct.newstarts.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ny.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kk.nszjky.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gl.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jp.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yp.wgjwhj.cn

[P03] 生成短随机字符串
来源：http://ul.huanxung.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ms.nszjky.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://er.newstarts.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cn.jctech888.com.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iy.szsharing.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vu.shtwfgs.cn


<!-- 参考信息 -->