代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ok.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kr.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://oo.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kr.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mg.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xm.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nu.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://im.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pj.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sn.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ae.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://bm.panjiajie.cn

Py:   resp.json()
来源：http://pc.nszjky.cn

PHP:  json_decode($body, true);
来源：http://pg.bookmarksfly.cn

JS:   await resp.json()
来源：http://gd.shxzskj.cn

TS:   await resp.json()
来源：http://ro.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://df.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fn.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://iw.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kg.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://io.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hf.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zs.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://wo.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://fy.chemitech.net.cn

Java: resp.statusCode()
来源：http://sd.jctech888.com.cn

Go:   resp.StatusCode
来源：http://vc.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://vf.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://hy.asd995.cn

[L08] 并发请求多个地址
来源：http://zp.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bb.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://fm.lnxyls.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qy.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qo.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bp.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mo.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ru.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ib.shxzskj.cn

================================================================================
来源：http://le.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://xb.wgjwhj.cn

================================================================================
来源：http://ba.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://yw.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://vl.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://hw.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://db.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://zg.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://nv.lnxyls.cn

Go:   os.Args[1:]
来源：http://jf.jianghongdianzi.cn

Ruby: ARGV
来源：http://gu.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://ni.haigaiapp.cn

[M02] 读取环境变量
来源：http://sz.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://xc.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xp.haigaiapp.cn

JS:   process.env.HOME
来源：http://on.wgjwhj.cn

TS:   process.env.HOME
来源：http://dx.huanxung.cn

Java: System.getenv("HOME")
来源：http://ls.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hc.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://en.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ye.hahajie.cn

[M03] 执行外部命令
来源：http://nq.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jy.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ko.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dp.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hh.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bo.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gd.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lq.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://id.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://la.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://fo.shxzskj.cn

PHP:  getcwd();
来源：http://ub.9csxet.cn

JS:   process.cwd()
来源：http://fq.yuntaijiaju.cn

TS:   process.cwd()
来源：http://zb.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://jh.asd995.cn

Go:   os.Getwd()
来源：http://hx.9csxet.cn

Ruby: Dir.pwd
来源：http://zz.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oy.yuexingan06.cn

[M05] 设置退出码
来源：http://dk.hnjuh.cn

Py:   sys.exit(1)
来源：http://pu.colortex.cn

PHP:  exit(1);
来源：http://do.chemitech.net.cn

JS:   process.exit(1)
来源：http://lu.szxytkj.cn

TS:   process.exit(1)
来源：http://gt.yuntaijiaju.cn

Java: System.exit(1)
来源：http://rd.hnjuh.cn

Go:   os.Exit(1)
来源：http://uk.hnjuh.cn

Ruby: exit 1
来源：http://wu.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://on.chemitech.net.cn

[M06] 向标准错误输出
来源：http://wg.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://fc.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://as.yuntaijiaju.cn

JS:   console.error("err")
来源：http://rz.jctech888.com.cn

TS:   console.error("err")
来源：http://sg.newstarts.cn

Java: System.err.println("err")
来源：http://zx.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fh.bookmarksfly.cn

Ruby: warn "err"
来源：http://kq.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://tg.hnjuh.cn

[M07] 判断是否为主入口
来源：http://vq.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://fi.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fn.muxihuayi.cn

JS:   require.main === module
来源：http://lw.szsharing.cn

TS:   require.main === module
来源：http://pl.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://xl.521024.cn

Go:   func main()
来源：http://ni.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oy.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://cl.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://qj.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://vx.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://zc.huanxung.cn

JS:   process.platform;  process.version
来源：http://up.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://uc.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kh.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gl.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sb.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://at.nicolike.cn

================================================================================
来源：http://kv.hnjuh.cn

N. 数据结构与算法
来源：http://ft.jianghongdianzi.cn

================================================================================
来源：http://hd.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://rc.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yx.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nh.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tp.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vz.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gu.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ct.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mp.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aa.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://ye.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://zx.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lo.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ht.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pk.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://mr.muxihuayi.cn

Ruby: arr.sort
来源：http://mb.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://as.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://zn.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fb.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://yg.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gd.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ay.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tz.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gd.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dh.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yp.shxzukj.cn

[N04] 斐波那契数列
来源：http://no.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://df.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rz.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gl.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cn.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://le.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://of.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nh.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cu.hnjuh.cn

[N05] 最大公约数
来源：http://mn.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ye.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ws.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ze.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hq.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qe.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ns.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ul.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pg.shxzukj.cn

[N06] 判断回文字符串
来源：http://el.hnjuh.cn

Py:   s == s[::-1]
来源：http://rw.chemitech.net.cn

PHP:  $s === strrev($s);
来源：http://ht.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://xz.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://yi.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wt.521024.cn

Go:   // 双指针从两端比较
来源：http://uc.jctech888.com.cn

Ruby: s == s.reverse
来源：http://vo.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nl.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://zu.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rf.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eb.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ms.lnxyls.cn

TS:   // 手写 Map<string, number>
来源：http://yb.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://ou.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://hu.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://xu.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fb.asd995.cn

[N08] 生成全排列
来源：http://gh.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://et.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://ou.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://sk.521024.cn

TS:   // 手写回溯递归
来源：http://ao.panjiajie.cn

Java: // 手写回溯递归
来源：http://ye.newstarts.cn

Go:   // 手写回溯递归
来源：http://yg.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://sj.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://qf.bookmarksfly.cn

[N09] 栈与队列
来源：http://zn.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mw.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bx.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nx.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://re.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ws.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yz.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pk.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ec.shtwfgs.cn

[N10] 链表节点定义
来源：http://yn.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nv.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zd.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://le.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mr.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ds.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ty.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fe.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ku.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://kx.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hx.colortex.cn

PHP:  // 手写递归函数
来源：http://ag.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://py.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://is.hnjuh.cn

Java: // 手写递归
来源：http://rv.bookmarksfly.cn

Go:   // 手写递归
来源：http://ag.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://li.panjiajie.cn

C#:   // 手写递归
来源：http://rh.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ac.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://go.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nf.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lq.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tm.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ie.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fy.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vi.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fh.haigaiapp.cn

================================================================================
来源：http://dc.jctech888.com.cn

O. 并发与异步
来源：http://wi.muxihuayi.cn

================================================================================
来源：http://fo.muxihuayi.cn

[O01] 启动一个线程
来源：http://kw.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sk.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ci.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eh.jianghongdianzi.cn

TS:   // 同 JS
来源：http://wd.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ou.bookmarksfly.cn

Go:   go f()
来源：http://cg.hahajie.cn

Ruby: Thread.new { f }
来源：http://fp.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://oa.panjiajie.cn

[O02] 使用线程池
来源：http://dj.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fp.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yz.colortex.cn

JS:   // worker_threads 线程池
来源：http://qg.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://gz.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://as.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://er.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xy.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iy.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://mm.nicolike.cn

Py:   with lock: shared += 1
来源：http://lm.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lg.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://um.asd995.cn

TS:   // 同 JS
来源：http://gq.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://op.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ac.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nb.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://xv.jctech888.com.cn

[O04] 定义异步函数并等待
来源：http://be.jianghongdianzi.cn

Py:   async def f():⏎    await g()
来源：http://zw.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ud.hahajie.cn

JS:   async function f() { await g(); }
来源：http://py.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zl.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ww.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ji.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oy.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://ke.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://wr.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://uo.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://th.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://fd.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://am.chemitech.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hq.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tp.szsharing.cn

Ruby: threads.map(&:join)
来源：http://vx.szsharing.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tg.nszjky.cn

[O06] 使用进程池
来源：http://lh.shxzskj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hn.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tp.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://xg.chemitech.net.cn

TS:   // child_process / cluster 模块
来源：http://fv.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xi.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ha.asd995.cn

Ruby: // fork 块
来源：http://ow.yuexingan06.cn

C#:   Parallel.For
来源：http://fn.hahajie.cn

================================================================================
来源：http://hw.colortex.cn

P. 常用工具函数
来源：http://fd.szsharing.cn

================================================================================
来源：http://tm.nszjky.cn

[P01] 生成 UUID
来源：http://ij.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://vo.chemitech.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oi.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ze.nicolike.cn

TS:   crypto.randomUUID()
来源：http://ub.wgjwhj.cn

Java: UUID.randomUUID().toString()
来源：http://mm.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://qy.521024.cn

Ruby: SecureRandom.uuid
来源：http://oa.bookmarksfly.cn

C#:   Guid.NewGuid().ToString()
来源：http://rn.chemitech.net.cn

[P02] MD5 / SHA256 摘要
来源：http://db.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cw.yuexingan06.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ad.9csxet.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fr.yuntaijiaju.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tj.chemitech.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hb.521024.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kv.521024.cn


<!-- 参考信息 -->