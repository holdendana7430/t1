代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://co.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ge.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://og.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ic.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ju.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zl.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ed.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gu.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rs.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nw.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://it.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://gs.hnjuh.cn

Py:   resp.json()
来源：http://in.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://lr.jctech888.com.cn

JS:   await resp.json()
来源：http://kw.nszjky.cn

TS:   await resp.json()
来源：http://vk.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://um.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mt.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://mc.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zz.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://fi.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nm.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qb.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ug.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://iu.lnxyls.cn

Java: resp.statusCode()
来源：http://aq.shxzukj.cn

Go:   resp.StatusCode
来源：http://bt.hahajie.cn

Ruby: resp.code.to_i
来源：http://jr.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://im.colortex.cn

[L08] 并发请求多个地址
来源：http://zo.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hl.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://kz.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://no.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ul.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lf.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mj.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fd.jianghongdianzi.cn

================================================================================
来源：http://qx.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://dq.9csxet.cn

================================================================================
来源：http://dr.shxzskj.cn

[M01] 读取命令行参数
来源：http://ls.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://by.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://qg.521024.cn

JS:   process.argv.slice(2)
来源：http://hu.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://wy.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://vy.yuexingan06.cn

Go:   os.Args[1:]
来源：http://tc.shxzskj.cn

Ruby: ARGV
来源：http://sz.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://tm.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://jn.asd995.cn

Py:   os.environ.get("HOME")
来源：http://hl.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fd.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://vd.nicolike.cn

TS:   process.env.HOME
来源：http://uj.newstarts.cn

Java: System.getenv("HOME")
来源：http://cd.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wz.asd995.cn

Ruby: ENV["HOME"]
来源：http://fm.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://if.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://ah.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jq.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ma.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ma.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rh.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iq.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://df.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pn.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://ez.gzmigu.cn

[M04] 获取当前工作目录
来源：http://bx.lnxyls.cn

Py:   os.getcwd()
来源：http://kw.asd995.cn

PHP:  getcwd();
来源：http://ut.huixiangedu.cn

JS:   process.cwd()
来源：http://dt.szxytkj.cn

TS:   process.cwd()
来源：http://jf.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://dr.colortex.cn

Go:   os.Getwd()
来源：http://pj.hahajie.cn

Ruby: Dir.pwd
来源：http://ea.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wz.huixinmuqiang.cn

[M05] 设置退出码
来源：http://zb.bjjhwx.cn

Py:   sys.exit(1)
来源：http://ap.hnjuh.cn

PHP:  exit(1);
来源：http://fh.szsharing.cn

JS:   process.exit(1)
来源：http://qa.muxihuayi.cn

TS:   process.exit(1)
来源：http://ml.szsharing.cn

Java: System.exit(1)
来源：http://be.lnxyls.cn

Go:   os.Exit(1)
来源：http://pw.nszjky.cn

Ruby: exit 1
来源：http://js.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sq.huanxung.cn

[M06] 向标准错误输出
来源：http://rp.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://hn.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gj.huanxung.cn

JS:   console.error("err")
来源：http://bm.bookmarksfly.cn

TS:   console.error("err")
来源：http://cc.gzmigu.cn

Java: System.err.println("err")
来源：http://ed.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hf.muxihuayi.cn

Ruby: warn "err"
来源：http://os.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ld.panjiajie.cn

[M07] 判断是否为主入口
来源：http://pp.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://wo.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lh.panjiajie.cn

JS:   require.main === module
来源：http://hd.shxzukj.cn

TS:   require.main === module
来源：http://mj.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://iy.shtwfgs.cn

Go:   func main()
来源：http://jx.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ns.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://jf.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://ys.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://ej.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://dn.lnxyls.cn

JS:   process.platform;  process.version
来源：http://dv.newstarts.cn

TS:   process.platform;  process.version
来源：http://zf.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jl.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pd.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bj.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ik.muxihuayi.cn

================================================================================
来源：http://fo.nicolike.cn

N. 数据结构与算法
来源：http://bx.szsharing.cn

================================================================================
来源：http://oa.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://pa.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sc.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://le.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zt.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hr.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ov.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://ib.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mt.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jv.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://lu.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://sv.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ta.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wv.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bq.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ux.521024.cn

Go:   slices.Sort(arr)
来源：http://ab.asd995.cn

Ruby: arr.sort
来源：http://jj.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tf.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://tk.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vm.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://pf.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wo.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lj.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qh.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lv.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ex.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://sj.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wp.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dc.panjiajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ya.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kr.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nu.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ha.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wt.bjjhwx.cn

[N05] 最大公约数
来源：http://cr.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://rt.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zf.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wh.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hv.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qq.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mn.hahajie.cn

Ruby: a.gcd(b)
来源：http://yd.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rs.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://hf.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://rp.colortex.cn

PHP:  $s === strrev($s);
来源：http://jv.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://ue.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://wk.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yv.hahajie.cn

Go:   // 双指针从两端比较
来源：http://sy.lnxyls.cn

Ruby: s == s.reverse
来源：http://yd.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vj.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://kk.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qw.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wb.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jc.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://xv.hnjuh.cn

Java: // 手写 HashMap
来源：http://cd.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://jt.lnxyls.cn

Ruby: // 手写 Hash
来源：http://sq.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ef.huixiangedu.cn

[N08] 生成全排列
来源：http://kq.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://ab.gzmigu.cn

PHP:  // 手写递归交换
来源：http://qx.panjiajie.cn

JS:   // 手写回溯递归
来源：http://yg.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://pn.lnxyls.cn

Java: // 手写回溯递归
来源：http://gs.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://hs.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://su.lnxyls.cn

C#:   // 手写回溯递归
来源：http://nv.jianghongdianzi.cn

[N09] 栈与队列
来源：http://fy.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dk.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://js.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mz.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://li.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zq.521024.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oo.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ri.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hp.nicolike.cn

[N10] 链表节点定义
来源：http://gx.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eo.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wt.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vi.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://og.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://es.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xn.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qy.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gn.huanxung.cn

[N11] 二叉树中序遍历
来源：http://da.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sl.gzmigu.cn

PHP:  // 手写递归函数
来源：http://fl.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sh.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rp.hnjuh.cn

Java: // 手写递归
来源：http://sq.gzmigu.cn

Go:   // 手写递归
来源：http://tv.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pa.nicolike.cn

C#:   // 手写递归
来源：http://cj.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hk.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ex.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tu.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cx.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eo.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lt.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mf.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nz.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zh.huanxung.cn

================================================================================
来源：http://fn.huixiangedu.cn

O. 并发与异步
来源：http://gs.newstarts.cn

================================================================================
来源：http://zh.nszjky.cn

[O01] 启动一个线程
来源：http://jz.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ud.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lp.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fn.9csxet.cn

TS:   // 同 JS
来源：http://av.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://vp.lnxyls.cn

Go:   go f()
来源：http://ev.lnxyls.cn

Ruby: Thread.new { f }
来源：http://hc.shxzukj.cn

C#:   Task.Run(() => F());
来源：http://oc.lnxyls.cn

[O02] 使用线程池
来源：http://hk.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zp.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aa.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://to.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://ay.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yv.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ya.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wj.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hw.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://nn.lnxyls.cn

Py:   with lock: shared += 1
来源：http://lg.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ap.huanxung.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vr.jctech888.com.cn

TS:   // 同 JS
来源：http://ry.shtwfgs.cn

Java: synchronized (this) { shared++; }
来源：http://yn.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fq.bookmarksfly.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vh.hnjuh.cn

C#:   lock (gate) { shared++; }
来源：http://nj.szxytkj.cn

[O04] 定义异步函数并等待
来源：http://px.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://bj.szxytkj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ig.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://ts.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kv.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://du.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://if.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lj.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://ob.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://oq.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://hy.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jd.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://iy.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://mq.huixinmuqiang.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ho.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fl.521024.cn

Ruby: threads.map(&:join)
来源：http://me.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vx.huanxung.cn

[O06] 使用进程池
来源：http://xp.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rq.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kn.newstarts.cn

JS:   // child_process / cluster 模块
来源：http://yb.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://sy.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yx.bookmarksfly.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eu.jctech888.com.cn

Ruby: // fork 块
来源：http://hw.jctech888.com.cn

C#:   Parallel.For
来源：http://yx.chemitech.net.cn

================================================================================
来源：http://zp.asd995.cn

P. 常用工具函数
来源：http://ex.gzmigu.cn

================================================================================
来源：http://ef.shtwfgs.cn

[P01] 生成 UUID
来源：http://tm.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://to.huanxung.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kn.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://yb.shxzukj.cn

TS:   crypto.randomUUID()
来源：http://tk.jctech888.com.cn

Java: UUID.randomUUID().toString()
来源：http://wi.huanxung.cn

Go:   // 用 github.com/google/uuid
来源：http://jn.bookmarksfly.cn

Ruby: SecureRandom.uuid
来源：http://vp.hahajie.cn

C#:   Guid.NewGuid().ToString()
来源：http://yw.huixiangedu.cn

[P02] MD5 / SHA256 摘要
来源：http://af.wgjwhj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ck.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rz.huixinmuqiang.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zj.gzmigu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ax.jianghongdianzi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cx.nicolike.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ih.shxzukj.cn


<!-- 参考信息 -->