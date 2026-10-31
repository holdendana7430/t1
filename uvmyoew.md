代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fs.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zf.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://jq.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://st.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ry.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xa.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fg.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zg.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qx.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hx.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ah.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://yq.szxytkj.cn

Py:   resp.json()
来源：http://nw.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://oj.jctech888.com.cn

JS:   await resp.json()
来源：http://qq.hahajie.cn

TS:   await resp.json()
来源：http://ob.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ys.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gf.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://uc.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rw.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://js.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mj.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ju.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://jl.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://pz.lnxyls.cn

Java: resp.statusCode()
来源：http://ft.szsharing.cn

Go:   resp.StatusCode
来源：http://bl.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://fj.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://rx.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://xt.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yu.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://pp.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xi.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ah.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bf.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fa.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lv.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fx.nszjky.cn

================================================================================
来源：http://iw.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://fp.newstarts.cn

================================================================================
来源：http://mt.shxzskj.cn

[M01] 读取命令行参数
来源：http://ub.szsharing.cn

Py:   sys.argv[1:]
来源：http://tx.nszjky.cn

PHP:  $argv;  $argc;
来源：http://pn.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://ea.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://us.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://on.newstarts.cn

Go:   os.Args[1:]
来源：http://ho.huanxung.cn

Ruby: ARGV
来源：http://mn.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://sv.nicolike.cn

[M02] 读取环境变量
来源：http://gt.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://kr.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fx.nszjky.cn

JS:   process.env.HOME
来源：http://aq.521024.cn

TS:   process.env.HOME
来源：http://ne.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://gw.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zi.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://so.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bu.gzmigu.cn

[M03] 执行外部命令
来源：http://au.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://am.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bu.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sq.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qq.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hq.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iw.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ax.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://ea.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://up.gzmigu.cn

Py:   os.getcwd()
来源：http://qi.asd995.cn

PHP:  getcwd();
来源：http://jp.shxzukj.cn

JS:   process.cwd()
来源：http://lo.newstarts.cn

TS:   process.cwd()
来源：http://qq.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ao.hnjuh.cn

Go:   os.Getwd()
来源：http://ws.haigaiapp.cn

Ruby: Dir.pwd
来源：http://mi.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wu.gzmigu.cn

[M05] 设置退出码
来源：http://zt.shtwfgs.cn

Py:   sys.exit(1)
来源：http://bt.hnjuh.cn

PHP:  exit(1);
来源：http://be.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://ix.hnjuh.cn

TS:   process.exit(1)
来源：http://xv.521024.cn

Java: System.exit(1)
来源：http://mo.colortex.cn

Go:   os.Exit(1)
来源：http://fh.521024.cn

Ruby: exit 1
来源：http://zm.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zq.huixinmuqiang.cn

[M06] 向标准错误输出
来源：http://ta.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://xk.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://us.yuntaijiaju.cn

JS:   console.error("err")
来源：http://ze.nicolike.cn

TS:   console.error("err")
来源：http://mr.asd995.cn

Java: System.err.println("err")
来源：http://el.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bw.colortex.cn

Ruby: warn "err"
来源：http://dx.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://bb.9csxet.cn

[M07] 判断是否为主入口
来源：http://zw.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://hl.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://no.nicolike.cn

JS:   require.main === module
来源：http://uz.hahajie.cn

TS:   require.main === module
来源：http://om.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://kt.shxzskj.cn

Go:   func main()
来源：http://le.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wl.9csxet.cn

C#:   static void Main(string[] args)
来源：http://mn.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://wp.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://bq.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ws.szxytkj.cn

JS:   process.platform;  process.version
来源：http://is.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://qg.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ot.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pz.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://af.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jd.yuntaijiaju.cn

================================================================================
来源：http://tk.huixiangedu.cn

N. 数据结构与算法
来源：http://li.wgjwhj.cn

================================================================================
来源：http://qh.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://az.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ye.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://en.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eo.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xc.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xt.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://qj.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ud.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qd.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://os.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ex.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ik.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vo.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xm.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sa.colortex.cn

Go:   slices.Sort(arr)
来源：http://rv.lnxyls.cn

Ruby: arr.sort
来源：http://cr.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ph.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://gl.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://px.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://en.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xg.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mi.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kw.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cq.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xd.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://km.shxzskj.cn

[N04] 斐波那契数列
来源：http://xd.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fv.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xm.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zc.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oa.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ao.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rg.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sh.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mz.huanxung.cn

[N05] 最大公约数
来源：http://gj.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://fd.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lo.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pj.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ni.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ij.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sh.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://ia.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cd.gzmigu.cn

[N06] 判断回文字符串
来源：http://yo.huanxung.cn

Py:   s == s[::-1]
来源：http://op.newstarts.cn

PHP:  $s === strrev($s);
来源：http://rq.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://ag.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ga.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://li.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://dz.huanxung.cn

Ruby: s == s.reverse
来源：http://df.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://js.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://dk.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mp.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pz.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rk.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://yw.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://wl.asd995.cn

Go:   // 手写 map[int]int
来源：http://jh.gzmigu.cn

Ruby: // 手写 Hash
来源：http://ia.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gf.gzmigu.cn

[N08] 生成全排列
来源：http://zr.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://gy.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://xu.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://vk.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://tl.huanxung.cn

Java: // 手写回溯递归
来源：http://ns.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://ko.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://nn.asd995.cn

C#:   // 手写回溯递归
来源：http://ra.521024.cn

[N09] 栈与队列
来源：http://fq.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hg.gzmigu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fm.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ws.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ob.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ag.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eo.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xl.asd995.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pq.9csxet.cn

[N10] 链表节点定义
来源：http://xt.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ws.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jp.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ss.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lt.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://lx.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vn.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jc.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dp.szsharing.cn

[N11] 二叉树中序遍历
来源：http://dy.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rb.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://qo.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wz.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://io.shxzskj.cn

Java: // 手写递归
来源：http://hv.yuexingan06.cn

Go:   // 手写递归
来源：http://ob.shxzskj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jf.asd995.cn

C#:   // 手写递归
来源：http://bg.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ba.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hh.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fh.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://id.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nc.wgjwhj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uq.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wh.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mu.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rr.asd995.cn

================================================================================
来源：http://qi.panjiajie.cn

O. 并发与异步
来源：http://sz.szsharing.cn

================================================================================
来源：http://dk.muxihuayi.cn

[O01] 启动一个线程
来源：http://yh.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://my.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qm.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iz.haigaiapp.cn

TS:   // 同 JS
来源：http://fk.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://av.yuntaijiaju.cn

Go:   go f()
来源：http://ya.gzmigu.cn

Ruby: Thread.new { f }
来源：http://dx.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://pt.yuexingan06.cn

[O02] 使用线程池
来源：http://te.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://md.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dn.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://ww.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://sn.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ql.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ub.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vl.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yq.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://sn.chemitech.net.cn

Py:   with lock: shared += 1
来源：http://sj.szsharing.cn

PHP:  // 用 flock() 做文件锁
来源：http://mb.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zw.colortex.cn

TS:   // 同 JS
来源：http://yi.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://ds.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sl.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fx.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://al.shtwfgs.cn

[O04] 定义异步函数并等待
来源：http://yq.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://oi.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://np.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://jt.lnxyls.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ak.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bl.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yn.521024.cn

Ruby: # 用 Fiber 或 async gem
来源：http://av.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://wi.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://vy.shxzskj.cn

Py:   asyncio.gather(*tasks)
来源：http://fw.shtwfgs.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vt.szsharing.cn

JS:   await Promise.all(tasks)
来源：http://jr.szsharing.cn

TS:   await Promise.all(tasks)
来源：http://za.yuexingan06.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iy.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jf.bookmarksfly.cn

Ruby: threads.map(&:join)
来源：http://ek.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nr.muxihuayi.cn

[O06] 使用进程池
来源：http://ke.bookmarksfly.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hs.9csxet.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hn.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://td.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://ck.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zg.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bo.bookmarksfly.cn

Ruby: // fork 块
来源：http://rq.wgjwhj.cn

C#:   Parallel.For
来源：http://id.lnxyls.cn

================================================================================
来源：http://mn.haigaiapp.cn

P. 常用工具函数
来源：http://wn.jctech888.com.cn

================================================================================
来源：http://nw.yuexingan06.cn

[P01] 生成 UUID
来源：http://rd.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://kd.colortex.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zu.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ll.521024.cn

TS:   crypto.randomUUID()
来源：http://xg.szxytkj.cn

Java: UUID.randomUUID().toString()
来源：http://qk.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://lq.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://nb.colortex.cn

C#:   Guid.NewGuid().ToString()
来源：http://yt.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://vd.yuntaijiaju.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bl.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://io.asd995.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://za.jctech888.com.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xw.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qn.panjiajie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://un.yuexingan06.cn


<!-- 参考信息 -->