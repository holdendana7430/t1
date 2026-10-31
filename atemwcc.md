代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sm.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nz.nicolike.cn

[L05] 上传文件（multipart）
来源：http://oe.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://or.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kj.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ib.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sf.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dz.9csxet.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ks.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gz.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tw.521024.cn

[L06] 解析响应为 JSON
来源：http://as.521024.cn

Py:   resp.json()
来源：http://kn.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://ec.colortex.cn

JS:   await resp.json()
来源：http://sd.bjjhwx.cn

TS:   await resp.json()
来源：http://gu.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yc.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gp.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://fz.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://po.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://sj.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dp.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://if.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://qc.521024.cn

TS:   resp.ok;  resp.status
来源：http://ug.wgjwhj.cn

Java: resp.statusCode()
来源：http://nm.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://bt.shxzskj.cn

Ruby: resp.code.to_i
来源：http://sc.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://nt.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://vn.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nk.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://wo.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sa.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bs.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yn.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ki.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sf.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bk.shxzskj.cn

================================================================================
来源：http://jk.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://gt.lnxyls.cn

================================================================================
来源：http://zh.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://io.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://zm.asd995.cn

PHP:  $argv;  $argc;
来源：http://dm.colortex.cn

JS:   process.argv.slice(2)
来源：http://ag.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://oy.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://em.haigaiapp.cn

Go:   os.Args[1:]
来源：http://kp.huixinmuqiang.cn

Ruby: ARGV
来源：http://ga.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://lc.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://bl.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://xe.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jz.521024.cn

JS:   process.env.HOME
来源：http://ux.shxzukj.cn

TS:   process.env.HOME
来源：http://wo.hahajie.cn

Java: System.getenv("HOME")
来源：http://ho.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ef.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://sf.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cg.nicolike.cn

[M03] 执行外部命令
来源：http://ri.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sf.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dx.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kx.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bw.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nd.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oz.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pq.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://fb.lnxyls.cn

[M04] 获取当前工作目录
来源：http://os.nszjky.cn

Py:   os.getcwd()
来源：http://hs.haigaiapp.cn

PHP:  getcwd();
来源：http://ip.521024.cn

JS:   process.cwd()
来源：http://ly.9csxet.cn

TS:   process.cwd()
来源：http://nn.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://kv.szxytkj.cn

Go:   os.Getwd()
来源：http://mn.asd995.cn

Ruby: Dir.pwd
来源：http://ge.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://be.bookmarksfly.cn

[M05] 设置退出码
来源：http://bz.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://cu.hahajie.cn

PHP:  exit(1);
来源：http://ws.colortex.cn

JS:   process.exit(1)
来源：http://kd.bookmarksfly.cn

TS:   process.exit(1)
来源：http://ve.huixinmuqiang.cn

Java: System.exit(1)
来源：http://cw.shxzukj.cn

Go:   os.Exit(1)
来源：http://us.huanxung.cn

Ruby: exit 1
来源：http://kd.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oo.huixiangedu.cn

[M06] 向标准错误输出
来源：http://bn.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://dm.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mr.colortex.cn

JS:   console.error("err")
来源：http://nn.newstarts.cn

TS:   console.error("err")
来源：http://tx.asd995.cn

Java: System.err.println("err")
来源：http://ko.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qk.yuexingan06.cn

Ruby: warn "err"
来源：http://ww.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://vi.panjiajie.cn

[M07] 判断是否为主入口
来源：http://hu.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://zv.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pc.9csxet.cn

JS:   require.main === module
来源：http://mz.haigaiapp.cn

TS:   require.main === module
来源：http://eu.panjiajie.cn

Java: public static void main(String[] args)
来源：http://ka.huixinmuqiang.cn

Go:   func main()
来源：http://dw.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ka.nicolike.cn

C#:   static void Main(string[] args)
来源：http://vb.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://kg.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://hl.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://yh.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://rg.shxzukj.cn

TS:   process.platform;  process.version
来源：http://xr.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sh.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ys.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jc.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dz.521024.cn

================================================================================
来源：http://ef.lnxyls.cn

N. 数据结构与算法
来源：http://mm.panjiajie.cn

================================================================================
来源：http://mo.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://xa.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nd.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hw.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sb.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jw.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jz.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://tm.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yr.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qq.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://uv.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://lo.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jy.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wl.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yy.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ew.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://xl.nicolike.cn

Ruby: arr.sort
来源：http://ed.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mi.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://ur.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rd.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://wb.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eq.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://je.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ua.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lz.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xl.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ix.panjiajie.cn

[N04] 斐波那契数列
来源：http://uq.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cl.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://an.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kh.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yx.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jf.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tp.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gr.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://my.lnxyls.cn

[N05] 最大公约数
来源：http://kg.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://wd.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://un.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dh.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ii.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ml.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yl.521024.cn

Ruby: a.gcd(b)
来源：http://ss.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pt.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://ry.gzmigu.cn

Py:   s == s[::-1]
来源：http://mo.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://sv.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://lk.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://jg.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rx.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://bu.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://zs.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eq.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://sz.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rw.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ld.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fa.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://up.shxzukj.cn

Java: // 手写 HashMap
来源：http://zu.asd995.cn

Go:   // 手写 map[int]int
来源：http://ak.lnxyls.cn

Ruby: // 手写 Hash
来源：http://rc.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fu.huixiangedu.cn

[N08] 生成全排列
来源：http://ef.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://fo.shxzukj.cn

PHP:  // 手写递归交换
来源：http://sz.panjiajie.cn

JS:   // 手写回溯递归
来源：http://qn.nszjky.cn

TS:   // 手写回溯递归
来源：http://lf.bjjhwx.cn

Java: // 手写回溯递归
来源：http://yi.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://rd.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://ta.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://dp.newstarts.cn

[N09] 栈与队列
来源：http://yn.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ld.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sm.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ij.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xe.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ju.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://al.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ah.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vh.bjjhwx.cn

[N10] 链表节点定义
来源：http://bl.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://va.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wl.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qv.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vz.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://mj.gzmigu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://to.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kt.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fe.nicolike.cn

[N11] 二叉树中序遍历
来源：http://fw.haigaiapp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pv.shxzskj.cn

PHP:  // 手写递归函数
来源：http://qv.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fz.yuexingan06.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ii.yuntaijiaju.cn

Java: // 手写递归
来源：http://bt.asd995.cn

Go:   // 手写递归
来源：http://pw.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dv.lnxyls.cn

C#:   // 手写递归
来源：http://mc.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jp.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ce.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cs.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wq.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ak.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mr.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sb.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hk.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vo.chemitech.net.cn

================================================================================
来源：http://zx.bjjhwx.cn

O. 并发与异步
来源：http://oe.shxzskj.cn

================================================================================
来源：http://ys.newstarts.cn

[O01] 启动一个线程
来源：http://te.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bi.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bf.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hp.nszjky.cn

TS:   // 同 JS
来源：http://vs.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://pj.bookmarksfly.cn

Go:   go f()
来源：http://jw.gzmigu.cn

Ruby: Thread.new { f }
来源：http://kx.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://jg.nicolike.cn

[O02] 使用线程池
来源：http://fn.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qa.9csxet.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hm.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://jy.huixiangedu.cn

TS:   // worker_threads 线程池
来源：http://yn.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://or.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nb.hahajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iw.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://up.521024.cn

[O03] 加锁保护共享数据
来源：http://so.asd995.cn

Py:   with lock: shared += 1
来源：http://nz.hahajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://gy.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bw.521024.cn

TS:   // 同 JS
来源：http://cu.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://ju.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mr.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gi.huanxung.cn

C#:   lock (gate) { shared++; }
来源：http://xe.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://jm.shxzukj.cn

Py:   async def f():⏎    await g()
来源：http://su.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dx.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://zr.newstarts.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lq.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cv.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jh.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dm.yuntaijiaju.cn

C#:   async Task F() { await G(); }
来源：http://ji.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://hz.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://zv.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ke.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://ak.chemitech.net.cn

TS:   await Promise.all(tasks)
来源：http://yt.bookmarksfly.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yo.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dj.521024.cn

Ruby: threads.map(&:join)
来源：http://nd.shxzskj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mf.bjjhwx.cn

[O06] 使用进程池
来源：http://lr.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hg.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ae.huixinmuqiang.cn

JS:   // child_process / cluster 模块
来源：http://je.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://hu.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://as.nszjky.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wb.hnjuh.cn

Ruby: // fork 块
来源：http://sj.shxzskj.cn

C#:   Parallel.For
来源：http://gz.nicolike.cn

================================================================================
来源：http://fj.hnjuh.cn

P. 常用工具函数
来源：http://sv.asd995.cn

================================================================================
来源：http://pb.gzmigu.cn

[P01] 生成 UUID
来源：http://xu.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://se.shxzskj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rj.panjiajie.cn

JS:   crypto.randomUUID()
来源：http://uy.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://aj.newstarts.cn

Java: UUID.randomUUID().toString()
来源：http://he.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://oi.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://ts.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://zt.szsharing.cn

[P02] MD5 / SHA256 摘要
来源：http://au.shtwfgs.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cz.9csxet.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sh.hnjuh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xj.shtwfgs.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rd.521024.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://an.huixinmuqiang.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gk.szsharing.cn


<!-- 参考信息 -->