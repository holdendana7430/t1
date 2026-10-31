代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sr.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nb.hahajie.cn

[L05] 上传文件（multipart）
来源：http://tj.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eg.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ia.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qo.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lm.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fs.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ke.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gy.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sx.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://gk.nicolike.cn

Py:   resp.json()
来源：http://ql.nszjky.cn

PHP:  json_decode($body, true);
来源：http://za.jianghongdianzi.cn

JS:   await resp.json()
来源：http://te.huixinmuqiang.cn

TS:   await resp.json()
来源：http://id.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zq.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qa.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://jt.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jh.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ng.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fu.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://st.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://qy.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://cr.huixiangedu.cn

Java: resp.statusCode()
来源：http://vb.shtwfgs.cn

Go:   resp.StatusCode
来源：http://ki.colortex.cn

Ruby: resp.code.to_i
来源：http://wr.521024.cn

C#:   (int)resp.StatusCode
来源：http://is.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://iq.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rt.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://hl.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bf.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ew.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vc.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dh.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dp.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pw.521024.cn

================================================================================
来源：http://md.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://vy.chemitech.net.cn

================================================================================
来源：http://yr.colortex.cn

[M01] 读取命令行参数
来源：http://xy.hahajie.cn

Py:   sys.argv[1:]
来源：http://pw.szsharing.cn

PHP:  $argv;  $argc;
来源：http://df.9csxet.cn

JS:   process.argv.slice(2)
来源：http://hv.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://qw.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://oo.hnjuh.cn

Go:   os.Args[1:]
来源：http://yl.9csxet.cn

Ruby: ARGV
来源：http://ep.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://dw.huanxung.cn

[M02] 读取环境变量
来源：http://ig.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://he.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hk.huanxung.cn

JS:   process.env.HOME
来源：http://yj.wgjwhj.cn

TS:   process.env.HOME
来源：http://nh.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://cm.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://ng.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oe.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://it.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cq.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dh.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ag.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kr.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vd.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nr.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jh.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://de.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://zr.asd995.cn

Py:   os.getcwd()
来源：http://rc.chemitech.net.cn

PHP:  getcwd();
来源：http://rh.huixinmuqiang.cn

JS:   process.cwd()
来源：http://pm.huanxung.cn

TS:   process.cwd()
来源：http://yh.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://id.yuexingan06.cn

Go:   os.Getwd()
来源：http://ug.huanxung.cn

Ruby: Dir.pwd
来源：http://mv.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qa.bjjhwx.cn

[M05] 设置退出码
来源：http://kt.chemitech.net.cn

Py:   sys.exit(1)
来源：http://tv.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ua.521024.cn

JS:   process.exit(1)
来源：http://wt.colortex.cn

TS:   process.exit(1)
来源：http://ci.521024.cn

Java: System.exit(1)
来源：http://bf.huixiangedu.cn

Go:   os.Exit(1)
来源：http://gr.hnjuh.cn

Ruby: exit 1
来源：http://yb.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gj.szsharing.cn

[M06] 向标准错误输出
来源：http://bp.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://lb.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hr.shxzskj.cn

JS:   console.error("err")
来源：http://mj.shtwfgs.cn

TS:   console.error("err")
来源：http://sp.wgjwhj.cn

Java: System.err.println("err")
来源：http://mm.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hp.newstarts.cn

Ruby: warn "err"
来源：http://hy.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://jw.colortex.cn

[M07] 判断是否为主入口
来源：http://db.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://hu.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dv.chemitech.net.cn

JS:   require.main === module
来源：http://ef.huixinmuqiang.cn

TS:   require.main === module
来源：http://eb.gzmigu.cn

Java: public static void main(String[] args)
来源：http://hc.yuntaijiaju.cn

Go:   func main()
来源：http://bd.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dy.9csxet.cn

C#:   static void Main(string[] args)
来源：http://um.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://kr.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://jl.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://nu.shxzukj.cn

JS:   process.platform;  process.version
来源：http://qx.huanxung.cn

TS:   process.platform;  process.version
来源：http://lh.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ql.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tr.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mo.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lg.hahajie.cn

================================================================================
来源：http://ic.bookmarksfly.cn

N. 数据结构与算法
来源：http://lx.hahajie.cn

================================================================================
来源：http://ms.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://ig.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jz.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hf.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ao.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dt.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://my.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://yr.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eg.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ov.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://nf.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://nr.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yr.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://il.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jy.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nl.nicolike.cn

Go:   slices.Sort(arr)
来源：http://ol.shtwfgs.cn

Ruby: arr.sort
来源：http://gq.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://my.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://tu.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ae.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://xd.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zv.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pd.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vc.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rm.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fb.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ju.colortex.cn

[N04] 斐波那契数列
来源：http://qi.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dm.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ke.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fp.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fl.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dy.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rl.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://af.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sq.bookmarksfly.cn

[N05] 最大公约数
来源：http://lg.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://vv.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ac.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rp.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xc.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dl.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oa.hahajie.cn

Ruby: a.gcd(b)
来源：http://nf.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nt.asd995.cn

[N06] 判断回文字符串
来源：http://dw.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://xw.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://bo.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://ge.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://ad.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bg.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://xu.newstarts.cn

Ruby: s == s.reverse
来源：http://np.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zg.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://pn.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ku.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qj.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rb.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://vx.gzmigu.cn

Java: // 手写 HashMap
来源：http://jo.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://bk.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://eu.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wb.nszjky.cn

[N08] 生成全排列
来源：http://op.asd995.cn

Py:   itertools.permutations(arr)
来源：http://no.521024.cn

PHP:  // 手写递归交换
来源：http://hp.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://ea.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://lv.newstarts.cn

Java: // 手写回溯递归
来源：http://op.9csxet.cn

Go:   // 手写回溯递归
来源：http://yx.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://un.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://bk.hnjuh.cn

[N09] 栈与队列
来源：http://de.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zg.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sf.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vb.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eo.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mn.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ld.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dx.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gw.jctech888.com.cn

[N10] 链表节点定义
来源：http://wu.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cm.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xy.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://df.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sa.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://zn.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yf.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lb.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iq.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://fw.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://te.nicolike.cn

PHP:  // 手写递归函数
来源：http://nd.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dm.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jl.shxzskj.cn

Java: // 手写递归
来源：http://ly.newstarts.cn

Go:   // 手写递归
来源：http://rk.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tf.huixiangedu.cn

C#:   // 手写递归
来源：http://wc.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tu.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vv.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gp.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://up.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gh.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zm.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kv.panjiajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ro.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ra.muxihuayi.cn

================================================================================
来源：http://fd.asd995.cn

O. 并发与异步
来源：http://zh.lnxyls.cn

================================================================================
来源：http://gl.szsharing.cn

[O01] 启动一个线程
来源：http://ik.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sn.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yp.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gh.gzmigu.cn

TS:   // 同 JS
来源：http://ih.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://xj.hnjuh.cn

Go:   go f()
来源：http://fd.huixiangedu.cn

Ruby: Thread.new { f }
来源：http://ar.9csxet.cn

C#:   Task.Run(() => F());
来源：http://al.lnxyls.cn

[O02] 使用线程池
来源：http://ct.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tw.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://me.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://jd.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://om.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vg.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jk.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wv.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://li.huanxung.cn

[O03] 加锁保护共享数据
来源：http://yo.szsharing.cn

Py:   with lock: shared += 1
来源：http://tm.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://af.chemitech.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hm.chemitech.net.cn

TS:   // 同 JS
来源：http://rp.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://im.9csxet.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gw.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dg.9csxet.cn

C#:   lock (gate) { shared++; }
来源：http://ol.hahajie.cn

[O04] 定义异步函数并等待
来源：http://pg.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://ik.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dq.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://vd.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hn.bookmarksfly.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://an.panjiajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://th.huanxung.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ex.bjjhwx.cn

C#:   async Task F() { await G(); }
来源：http://kw.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://eo.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://kl.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yw.shtwfgs.cn

JS:   await Promise.all(tasks)
来源：http://qk.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://rh.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sl.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ov.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://jf.jctech888.com.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://le.colortex.cn

[O06] 使用进程池
来源：http://mq.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ei.chemitech.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vb.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://wl.521024.cn

TS:   // child_process / cluster 模块
来源：http://gp.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oi.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ln.shxzukj.cn

Ruby: // fork 块
来源：http://zp.shxzukj.cn

C#:   Parallel.For
来源：http://yr.shxzskj.cn

================================================================================
来源：http://qx.panjiajie.cn

P. 常用工具函数
来源：http://vs.wgjwhj.cn

================================================================================
来源：http://ii.newstarts.cn

[P01] 生成 UUID
来源：http://qz.asd995.cn

Py:   str(uuid.uuid4())
来源：http://pl.huixiangedu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gi.9csxet.cn

JS:   crypto.randomUUID()
来源：http://vj.asd995.cn

TS:   crypto.randomUUID()
来源：http://xm.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://hq.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://wm.wgjwhj.cn

Ruby: SecureRandom.uuid
来源：http://fe.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://os.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://ti.hahajie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vn.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bk.colortex.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yw.hnjuh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tm.bookmarksfly.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xg.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ha.panjiajie.cn


<!-- 参考信息 -->