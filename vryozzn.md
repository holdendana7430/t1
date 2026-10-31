代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cf.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hr.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://is.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gp.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zh.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dw.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ik.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://kq.asd995.cn

Py:   resp.json()
来源：http://mj.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://fm.szsharing.cn

JS:   await resp.json()
来源：http://mg.wgjwhj.cn

TS:   await resp.json()
来源：http://fk.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wz.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://co.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://zp.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lt.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://wr.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://en.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qn.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://rm.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://ar.huixiangedu.cn

Java: resp.statusCode()
来源：http://dx.newstarts.cn

Go:   resp.StatusCode
来源：http://he.shxzskj.cn

Ruby: resp.code.to_i
来源：http://sb.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://cz.szsharing.cn

[L08] 并发请求多个地址
来源：http://rx.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://et.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://wf.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kc.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qc.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ub.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zs.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ap.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://bi.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://el.chemitech.net.cn

================================================================================
来源：http://ft.szsharing.cn

[M01] 读取命令行参数
来源：http://lh.nszjky.cn

Py:   sys.argv[1:]
来源：http://bj.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://ie.szsharing.cn

JS:   process.argv.slice(2)
来源：http://me.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://wd.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://dw.yuexingan06.cn

Go:   os.Args[1:]
来源：http://ha.jianghongdianzi.cn

Ruby: ARGV
来源：http://bj.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://mc.nszjky.cn

[M02] 读取环境变量
来源：http://po.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://bv.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sa.jctech888.com.cn

JS:   process.env.HOME
来源：http://gx.szsharing.cn

TS:   process.env.HOME
来源：http://je.lnxyls.cn

Java: System.getenv("HOME")
来源：http://dz.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gl.nszjky.cn

Ruby: ENV["HOME"]
来源：http://bq.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ld.gzmigu.cn

[M03] 执行外部命令
来源：http://nh.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qb.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fj.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://am.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ow.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ac.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fh.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gh.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://nq.huanxung.cn

[M04] 获取当前工作目录
来源：http://nh.nicolike.cn

Py:   os.getcwd()
来源：http://bn.haigaiapp.cn

PHP:  getcwd();
来源：http://zq.jctech888.com.cn

JS:   process.cwd()
来源：http://ab.newstarts.cn

TS:   process.cwd()
来源：http://mg.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ic.bjjhwx.cn

Go:   os.Getwd()
来源：http://pi.jctech888.com.cn

Ruby: Dir.pwd
来源：http://hz.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zo.huixiangedu.cn

[M05] 设置退出码
来源：http://pa.asd995.cn

Py:   sys.exit(1)
来源：http://eb.shtwfgs.cn

PHP:  exit(1);
来源：http://dk.shxzskj.cn

JS:   process.exit(1)
来源：http://cj.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://fp.bjjhwx.cn

Java: System.exit(1)
来源：http://tc.wgjwhj.cn

Go:   os.Exit(1)
来源：http://hq.hahajie.cn

Ruby: exit 1
来源：http://kk.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hp.hnjuh.cn

[M06] 向标准错误输出
来源：http://ln.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://ey.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vy.muxihuayi.cn

JS:   console.error("err")
来源：http://iq.nicolike.cn

TS:   console.error("err")
来源：http://ow.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://fc.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ux.muxihuayi.cn

Ruby: warn "err"
来源：http://va.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://eu.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ki.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://wd.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vr.newstarts.cn

JS:   require.main === module
来源：http://us.shxzskj.cn

TS:   require.main === module
来源：http://wh.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://wn.gzmigu.cn

Go:   func main()
来源：http://zi.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uv.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://kk.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ze.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://wk.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://ph.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://oi.gzmigu.cn

TS:   process.platform;  process.version
来源：http://sq.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oa.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hu.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rj.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bo.szxytkj.cn

================================================================================
来源：http://hv.wgjwhj.cn

N. 数据结构与算法
来源：http://rz.521024.cn

================================================================================
来源：http://fz.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://uf.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wy.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ln.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ik.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lz.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sp.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://wu.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://or.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ok.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://cd.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://cm.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://no.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fl.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sr.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sv.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://vm.wgjwhj.cn

Ruby: arr.sort
来源：http://ej.yuntaijiaju.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zw.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://co.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lb.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://qi.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yp.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jw.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uh.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ek.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lv.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://di.hahajie.cn

[N04] 斐波那契数列
来源：http://jz.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lo.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ny.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ko.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sn.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lo.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uw.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xf.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pb.gzmigu.cn

[N05] 最大公约数
来源：http://id.9csxet.cn

Py:   math.gcd(a, b)
来源：http://em.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mt.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nw.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oh.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bf.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xw.huanxung.cn

Ruby: a.gcd(b)
来源：http://cv.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gj.muxihuayi.cn

[N06] 判断回文字符串
来源：http://uy.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://wi.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://km.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://wq.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://nt.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xz.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://ih.shxzskj.cn

Ruby: s == s.reverse
来源：http://mf.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://au.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://vd.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://te.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aa.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xw.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://rn.huanxung.cn

Java: // 手写 HashMap
来源：http://iz.newstarts.cn

Go:   // 手写 map[int]int
来源：http://rj.huanxung.cn

Ruby: // 手写 Hash
来源：http://zo.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ss.yuexingan06.cn

[N08] 生成全排列
来源：http://eg.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://fv.shxzukj.cn

PHP:  // 手写递归交换
来源：http://rc.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://qf.shxzskj.cn

TS:   // 手写回溯递归
来源：http://id.bjjhwx.cn

Java: // 手写回溯递归
来源：http://je.gzmigu.cn

Go:   // 手写回溯递归
来源：http://gq.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://ra.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://jb.asd995.cn

[N09] 栈与队列
来源：http://je.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dm.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://me.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qm.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ru.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ec.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ny.huixiangedu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yb.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ru.szxytkj.cn

[N10] 链表节点定义
来源：http://kl.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qz.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://np.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yw.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eq.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://kn.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iy.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://za.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gq.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://sm.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wd.9csxet.cn

PHP:  // 手写递归函数
来源：http://dy.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fn.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cq.lnxyls.cn

Java: // 手写递归
来源：http://aa.gzmigu.cn

Go:   // 手写递归
来源：http://ig.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ma.colortex.cn

C#:   // 手写递归
来源：http://qu.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wt.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lf.yuntaijiaju.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cb.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kp.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mg.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nv.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hp.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jz.hahajie.cn

================================================================================
来源：http://az.huixinmuqiang.cn

O. 并发与异步
来源：http://jq.colortex.cn

================================================================================
来源：http://ne.colortex.cn

[O01] 启动一个线程
来源：http://ne.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jo.hnjuh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ta.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sq.muxihuayi.cn

TS:   // 同 JS
来源：http://jw.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://ve.gzmigu.cn

Go:   go f()
来源：http://xr.newstarts.cn

Ruby: Thread.new { f }
来源：http://dd.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://rg.chemitech.net.cn

[O02] 使用线程池
来源：http://uy.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fr.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ks.huanxung.cn

JS:   // worker_threads 线程池
来源：http://sb.szsharing.cn

TS:   // worker_threads 线程池
来源：http://ae.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zv.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://re.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xt.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qg.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://id.521024.cn

Py:   with lock: shared += 1
来源：http://dk.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://vn.jctech888.com.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xy.jctech888.com.cn

TS:   // 同 JS
来源：http://rj.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://vp.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ey.yuexingan06.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://am.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://yy.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://yr.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://sf.shxzskj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xe.bookmarksfly.cn

JS:   async function f() { await g(); }
来源：http://bp.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wv.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ro.521024.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fa.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uq.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://ny.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://kn.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://ln.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ck.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://ix.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://fx.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ft.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vn.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://sg.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rl.shtwfgs.cn

[O06] 使用进程池
来源：http://uh.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dm.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rg.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://jn.muxihuayi.cn

TS:   // child_process / cluster 模块
来源：http://hs.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qk.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qz.lnxyls.cn

Ruby: // fork 块
来源：http://ud.wgjwhj.cn

C#:   Parallel.For
来源：http://ji.wgjwhj.cn

================================================================================
来源：http://xk.jianghongdianzi.cn

P. 常用工具函数
来源：http://aw.nicolike.cn

================================================================================
来源：http://br.newstarts.cn

[P01] 生成 UUID
来源：http://dp.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://ut.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kd.nszjky.cn

JS:   crypto.randomUUID()
来源：http://rr.muxihuayi.cn

TS:   crypto.randomUUID()
来源：http://gk.nicolike.cn

Java: UUID.randomUUID().toString()
来源：http://vd.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://ux.szsharing.cn

Ruby: SecureRandom.uuid
来源：http://fc.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://na.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://sv.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hw.wgjwhj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hh.newstarts.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bc.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://an.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tu.yuexingan06.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ew.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://av.asd995.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ws.9csxet.cn

[P03] 生成短随机字符串
来源：http://fl.shxzskj.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gb.panjiajie.cn


<!-- 参考信息 -->