代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bn.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ia.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nq.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sc.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vm.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qp.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://he.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://pk.panjiajie.cn

Py:   resp.json()
来源：http://xz.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ki.huixinmuqiang.cn

JS:   await resp.json()
来源：http://qo.shxzskj.cn

TS:   await resp.json()
来源：http://hh.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jc.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qo.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://or.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ag.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://mb.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xp.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ka.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://uc.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://ye.muxihuayi.cn

Java: resp.statusCode()
来源：http://pi.gzmigu.cn

Go:   resp.StatusCode
来源：http://rt.9csxet.cn

Ruby: resp.code.to_i
来源：http://lk.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://kj.szxytkj.cn

[L08] 并发请求多个地址
来源：http://nh.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tl.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://gc.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bb.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uv.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pc.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://re.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ig.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lu.haigaiapp.cn

================================================================================
来源：http://as.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://vq.huixiangedu.cn

================================================================================
来源：http://dx.shxzskj.cn

[M01] 读取命令行参数
来源：http://lm.9csxet.cn

Py:   sys.argv[1:]
来源：http://vh.newstarts.cn

PHP:  $argv;  $argc;
来源：http://vx.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://vt.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://bw.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ju.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://ji.yuexingan06.cn

Ruby: ARGV
来源：http://fz.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://di.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://nb.asd995.cn

Py:   os.environ.get("HOME")
来源：http://om.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eg.jctech888.com.cn

JS:   process.env.HOME
来源：http://ec.haigaiapp.cn

TS:   process.env.HOME
来源：http://bh.huanxung.cn

Java: System.getenv("HOME")
来源：http://mb.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vh.521024.cn

Ruby: ENV["HOME"]
来源：http://zr.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rp.szsharing.cn

[M03] 执行外部命令
来源：http://jw.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aq.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bb.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dn.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://io.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kv.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://er.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gu.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://wc.lnxyls.cn

[M04] 获取当前工作目录
来源：http://ci.huixiangedu.cn

Py:   os.getcwd()
来源：http://tl.shxzskj.cn

PHP:  getcwd();
来源：http://yt.521024.cn

JS:   process.cwd()
来源：http://uy.szxytkj.cn

TS:   process.cwd()
来源：http://tr.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ej.haigaiapp.cn

Go:   os.Getwd()
来源：http://xo.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://ty.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gl.nszjky.cn

[M05] 设置退出码
来源：http://bj.bjjhwx.cn

Py:   sys.exit(1)
来源：http://cq.9csxet.cn

PHP:  exit(1);
来源：http://sw.muxihuayi.cn

JS:   process.exit(1)
来源：http://bb.chemitech.net.cn

TS:   process.exit(1)
来源：http://jb.gzmigu.cn

Java: System.exit(1)
来源：http://kx.521024.cn

Go:   os.Exit(1)
来源：http://ly.nszjky.cn

Ruby: exit 1
来源：http://ni.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ra.521024.cn

[M06] 向标准错误输出
来源：http://oe.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://ys.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qe.szxytkj.cn

JS:   console.error("err")
来源：http://wc.wgjwhj.cn

TS:   console.error("err")
来源：http://qz.bookmarksfly.cn

Java: System.err.println("err")
来源：http://on.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ap.huanxung.cn

Ruby: warn "err"
来源：http://ur.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://dx.asd995.cn

[M07] 判断是否为主入口
来源：http://br.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://xr.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gm.jctech888.com.cn

JS:   require.main === module
来源：http://qw.haigaiapp.cn

TS:   require.main === module
来源：http://ol.gzmigu.cn

Java: public static void main(String[] args)
来源：http://qe.szsharing.cn

Go:   func main()
来源：http://ui.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gr.hahajie.cn

C#:   static void Main(string[] args)
来源：http://pm.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://bo.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://wj.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ol.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://qz.huanxung.cn

TS:   process.platform;  process.version
来源：http://cd.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wj.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://di.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bd.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wv.haigaiapp.cn

================================================================================
来源：http://vb.bookmarksfly.cn

N. 数据结构与算法
来源：http://qr.shxzskj.cn

================================================================================
来源：http://sn.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://fk.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dx.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://et.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pt.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gg.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ps.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://vk.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zj.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fo.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://kp.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://yq.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hu.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sc.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ru.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iu.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://bg.wgjwhj.cn

Ruby: arr.sort
来源：http://cj.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jz.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://wd.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rb.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://ar.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nq.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pr.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zn.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ke.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wg.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sf.colortex.cn

[N04] 斐波那契数列
来源：http://xo.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kk.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://he.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bw.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mr.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ig.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://um.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ov.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://np.haigaiapp.cn

[N05] 最大公约数
来源：http://hi.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://ka.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qk.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yy.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qo.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dl.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://we.521024.cn

Ruby: a.gcd(b)
来源：http://ab.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mi.shxzskj.cn

[N06] 判断回文字符串
来源：http://aa.szxytkj.cn

Py:   s == s[::-1]
来源：http://gs.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://kh.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://vl.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://uz.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://np.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://uo.shxzskj.cn

Ruby: s == s.reverse
来源：http://gy.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pi.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://kx.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wu.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mq.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://io.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://qg.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://ce.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://iq.newstarts.cn

Ruby: // 手写 Hash
来源：http://uh.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sy.yuntaijiaju.cn

[N08] 生成全排列
来源：http://dr.521024.cn

Py:   itertools.permutations(arr)
来源：http://ns.shxzskj.cn

PHP:  // 手写递归交换
来源：http://wl.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://vc.gzmigu.cn

TS:   // 手写回溯递归
来源：http://is.newstarts.cn

Java: // 手写回溯递归
来源：http://hd.nicolike.cn

Go:   // 手写回溯递归
来源：http://xw.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://pj.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://id.gzmigu.cn

[N09] 栈与队列
来源：http://xh.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ez.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bj.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vi.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sm.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jz.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nx.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://im.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lz.szsharing.cn

[N10] 链表节点定义
来源：http://yc.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eg.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ig.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hi.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zh.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://pw.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zs.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sw.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ev.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://kd.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://li.szsharing.cn

PHP:  // 手写递归函数
来源：http://tu.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xr.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rz.colortex.cn

Java: // 手写递归
来源：http://no.panjiajie.cn

Go:   // 手写递归
来源：http://pd.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eh.huanxung.cn

C#:   // 手写递归
来源：http://wv.huixiangedu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qf.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ig.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pb.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bw.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xs.haigaiapp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jv.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://op.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jw.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qf.haigaiapp.cn

================================================================================
来源：http://hj.hnjuh.cn

O. 并发与异步
来源：http://ol.yuntaijiaju.cn

================================================================================
来源：http://bl.jctech888.com.cn

[O01] 启动一个线程
来源：http://nj.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://or.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mb.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lj.haigaiapp.cn

TS:   // 同 JS
来源：http://cj.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://ha.wgjwhj.cn

Go:   go f()
来源：http://aa.hnjuh.cn

Ruby: Thread.new { f }
来源：http://ce.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://na.panjiajie.cn

[O02] 使用线程池
来源：http://to.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xu.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wb.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://xt.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://hi.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vf.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zd.szsharing.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uz.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ui.huanxung.cn

[O03] 加锁保护共享数据
来源：http://gc.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hb.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://rw.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yc.chemitech.net.cn

TS:   // 同 JS
来源：http://mz.huanxung.cn

Java: synchronized (this) { shared++; }
来源：http://uo.huanxung.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ah.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ow.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://py.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://mo.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://dw.huixiangedu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aw.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://as.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ln.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mr.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dy.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://py.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://me.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://hd.huixiangedu.cn

Py:   asyncio.gather(*tasks)
来源：http://xp.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cx.bjjhwx.cn

JS:   await Promise.all(tasks)
来源：http://ny.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://xu.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vk.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hx.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://ns.9csxet.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ts.gzmigu.cn

[O06] 使用进程池
来源：http://fe.shtwfgs.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wb.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fc.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://am.huixiangedu.cn

TS:   // child_process / cluster 模块
来源：http://ow.gzmigu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vf.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://if.shxzskj.cn

Ruby: // fork 块
来源：http://cy.shtwfgs.cn

C#:   Parallel.For
来源：http://aq.asd995.cn

================================================================================
来源：http://vx.colortex.cn

P. 常用工具函数
来源：http://qz.jianghongdianzi.cn

================================================================================
来源：http://my.bookmarksfly.cn

[P01] 生成 UUID
来源：http://yq.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://sr.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hh.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://fy.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://tp.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://pm.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://qb.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://xy.yuntaijiaju.cn

C#:   Guid.NewGuid().ToString()
来源：http://ym.hahajie.cn

[P02] MD5 / SHA256 摘要
来源：http://of.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bl.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yh.gzmigu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qz.shxzukj.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ez.9csxet.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xl.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ub.jianghongdianzi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bf.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pc.nicolike.cn

[P03] 生成短随机字符串
来源：http://ix.yuntaijiaju.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tl.jianghongdianzi.cn


<!-- 参考信息 -->