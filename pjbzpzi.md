代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sw.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ja.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bl.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rc.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://px.nicolike.cn

[L05] 上传文件（multipart）
来源：http://kz.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://je.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yf.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xt.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wl.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bm.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zl.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ou.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ql.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://xu.szsharing.cn

Py:   resp.json()
来源：http://zk.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://wi.szxytkj.cn

JS:   await resp.json()
来源：http://be.colortex.cn

TS:   await resp.json()
来源：http://vj.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vp.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cr.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://dh.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sc.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://av.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zj.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cm.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://mp.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://qm.bookmarksfly.cn

Java: resp.statusCode()
来源：http://kj.newstarts.cn

Go:   resp.StatusCode
来源：http://nm.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://dk.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://eu.newstarts.cn

[L08] 并发请求多个地址
来源：http://qn.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kx.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://pd.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ep.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ji.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dk.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yg.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ia.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://br.huanxung.cn

================================================================================
来源：http://ow.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ud.shxzskj.cn

================================================================================
来源：http://ll.panjiajie.cn

[M01] 读取命令行参数
来源：http://km.gzmigu.cn

Py:   sys.argv[1:]
来源：http://qq.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://ew.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://ur.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://li.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://lx.colortex.cn

Go:   os.Args[1:]
来源：http://wq.bjjhwx.cn

Ruby: ARGV
来源：http://wt.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://fb.szsharing.cn

[M02] 读取环境变量
来源：http://nj.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://fo.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lk.gzmigu.cn

JS:   process.env.HOME
来源：http://mu.9csxet.cn

TS:   process.env.HOME
来源：http://lp.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://qr.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xi.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://do.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hf.shtwfgs.cn

[M03] 执行外部命令
来源：http://mp.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bp.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eu.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ci.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oh.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://we.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wf.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wz.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://xd.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://kv.9csxet.cn

Py:   os.getcwd()
来源：http://iy.lnxyls.cn

PHP:  getcwd();
来源：http://fy.yuexingan06.cn

JS:   process.cwd()
来源：http://gj.bjjhwx.cn

TS:   process.cwd()
来源：http://ml.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://vz.gzmigu.cn

Go:   os.Getwd()
来源：http://fe.szsharing.cn

Ruby: Dir.pwd
来源：http://oo.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rx.9csxet.cn

[M05] 设置退出码
来源：http://xq.gzmigu.cn

Py:   sys.exit(1)
来源：http://df.asd995.cn

PHP:  exit(1);
来源：http://rl.asd995.cn

JS:   process.exit(1)
来源：http://qz.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://kd.lnxyls.cn

Java: System.exit(1)
来源：http://tb.asd995.cn

Go:   os.Exit(1)
来源：http://ot.shtwfgs.cn

Ruby: exit 1
来源：http://su.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://md.nszjky.cn

[M06] 向标准错误输出
来源：http://an.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://ki.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pw.newstarts.cn

JS:   console.error("err")
来源：http://bm.yuntaijiaju.cn

TS:   console.error("err")
来源：http://jt.jctech888.com.cn

Java: System.err.println("err")
来源：http://zh.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yi.szxytkj.cn

Ruby: warn "err"
来源：http://gq.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://yf.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://nr.521024.cn

Py:   if __name__ == "__main__":
来源：http://yw.shxzukj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rx.bjjhwx.cn

JS:   require.main === module
来源：http://tj.chemitech.net.cn

TS:   require.main === module
来源：http://ll.521024.cn

Java: public static void main(String[] args)
来源：http://hg.bookmarksfly.cn

Go:   func main()
来源：http://qb.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vp.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://xx.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://yb.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://bl.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://kk.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://iy.asd995.cn

TS:   process.platform;  process.version
来源：http://ww.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ih.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fb.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ix.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://on.szsharing.cn

================================================================================
来源：http://ux.wgjwhj.cn

N. 数据结构与算法
来源：http://rh.lnxyls.cn

================================================================================
来源：http://gs.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://qd.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://er.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lh.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gp.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eg.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gk.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://gu.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lm.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fz.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://xh.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://pf.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://te.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mz.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uk.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kw.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://fp.jctech888.com.cn

Ruby: arr.sort
来源：http://oh.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bj.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://of.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fb.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://ai.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eq.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uo.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sd.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yq.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://us.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tv.shtwfgs.cn

[N04] 斐波那契数列
来源：http://vq.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://et.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gs.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sa.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://od.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xq.shtwfgs.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hn.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cw.bjjhwx.cn

[N05] 最大公约数
来源：http://ne.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://kh.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iv.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vb.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gd.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fx.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://vj.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ka.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://mo.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://hv.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://sq.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://hn.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://nh.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oe.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://uo.gzmigu.cn

Ruby: s == s.reverse
来源：http://ld.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yj.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://ja.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bx.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pu.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ks.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://vi.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://ua.newstarts.cn

Go:   // 手写 map[int]int
来源：http://ih.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://sv.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qs.lnxyls.cn

[N08] 生成全排列
来源：http://lr.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://jw.gzmigu.cn

PHP:  // 手写递归交换
来源：http://ws.shxzskj.cn

JS:   // 手写回溯递归
来源：http://bx.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://bl.newstarts.cn

Java: // 手写回溯递归
来源：http://yb.hnjuh.cn

Go:   // 手写回溯递归
来源：http://qs.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://sl.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://fl.yuntaijiaju.cn

[N09] 栈与队列
来源：http://vn.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ap.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mh.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jr.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bs.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://es.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ay.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iy.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gt.shxzskj.cn

[N10] 链表节点定义
来源：http://pj.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nr.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fp.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gi.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dc.gzmigu.cn

Java: class Node { int v; Node next; }
来源：http://tc.9csxet.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lo.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wc.hnjuh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dt.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://kd.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rl.gzmigu.cn

PHP:  // 手写递归函数
来源：http://rt.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ac.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://se.nicolike.cn

Java: // 手写递归
来源：http://so.haigaiapp.cn

Go:   // 手写递归
来源：http://or.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wm.nszjky.cn

C#:   // 手写递归
来源：http://jq.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tc.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qe.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bu.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ei.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zh.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oh.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bj.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yl.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wa.bookmarksfly.cn

================================================================================
来源：http://kk.asd995.cn

O. 并发与异步
来源：http://so.yuexingan06.cn

================================================================================
来源：http://su.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://jn.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fe.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ds.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rc.hnjuh.cn

TS:   // 同 JS
来源：http://qg.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://pb.colortex.cn

Go:   go f()
来源：http://of.newstarts.cn

Ruby: Thread.new { f }
来源：http://ef.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://xo.shtwfgs.cn

[O02] 使用线程池
来源：http://tb.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bc.muxihuayi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://li.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ev.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://sn.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://an.asd995.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cz.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ni.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fl.muxihuayi.cn

[O03] 加锁保护共享数据
来源：http://ez.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://hg.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://zc.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nx.yuntaijiaju.cn

TS:   // 同 JS
来源：http://tg.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://dg.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fm.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dy.bjjhwx.cn

C#:   lock (gate) { shared++; }
来源：http://in.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://uy.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ay.9csxet.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hh.521024.cn

JS:   async function f() { await g(); }
来源：http://yc.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gz.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cp.newstarts.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ze.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fi.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://og.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://uv.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://jv.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xr.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://ve.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://fb.colortex.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bk.shtwfgs.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vi.hahajie.cn

Ruby: threads.map(&:join)
来源：http://ss.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fs.yuexingan06.cn

[O06] 使用进程池
来源：http://ls.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vd.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gs.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://aq.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://zd.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vu.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://am.haigaiapp.cn

Ruby: // fork 块
来源：http://cn.hnjuh.cn

C#:   Parallel.For
来源：http://zd.haigaiapp.cn

================================================================================
来源：http://wq.hahajie.cn

P. 常用工具函数
来源：http://ll.haigaiapp.cn

================================================================================
来源：http://ih.lnxyls.cn

[P01] 生成 UUID
来源：http://et.asd995.cn

Py:   str(uuid.uuid4())
来源：http://sn.gzmigu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wk.colortex.cn

JS:   crypto.randomUUID()
来源：http://yd.huanxung.cn

TS:   crypto.randomUUID()
来源：http://nk.chemitech.net.cn

Java: UUID.randomUUID().toString()
来源：http://qs.chemitech.net.cn

Go:   // 用 github.com/google/uuid
来源：http://el.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://bs.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://st.muxihuayi.cn

[P02] MD5 / SHA256 摘要
来源：http://gf.haigaiapp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nz.colortex.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sb.huixinmuqiang.cn


<!-- 参考信息 -->