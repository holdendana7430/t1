代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oi.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iv.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ja.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sp.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tx.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ha.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://js.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xj.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gj.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ha.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://be.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gg.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fm.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sy.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vr.hahajie.cn

[L06] 解析响应为 JSON
来源：http://ao.wgjwhj.cn

Py:   resp.json()
来源：http://vh.huanxung.cn

PHP:  json_decode($body, true);
来源：http://wg.muxihuayi.cn

JS:   await resp.json()
来源：http://ky.bookmarksfly.cn

TS:   await resp.json()
来源：http://ih.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vq.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dk.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://if.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vf.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://jp.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sq.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fw.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://fr.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://tc.wgjwhj.cn

Java: resp.statusCode()
来源：http://vz.huixiangedu.cn

Go:   resp.StatusCode
来源：http://vn.hahajie.cn

Ruby: resp.code.to_i
来源：http://nw.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://pj.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://jh.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sb.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://xr.nicolike.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sl.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wv.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bu.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ae.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ug.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zi.yuntaijiaju.cn

================================================================================
来源：http://ol.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://rm.9csxet.cn

================================================================================
来源：http://by.asd995.cn

[M01] 读取命令行参数
来源：http://zv.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://as.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://sk.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://wo.szsharing.cn

TS:   process.argv.slice(2)
来源：http://nj.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://wl.wgjwhj.cn

Go:   os.Args[1:]
来源：http://jc.asd995.cn

Ruby: ARGV
来源：http://zd.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://tx.chemitech.net.cn

[M02] 读取环境变量
来源：http://vy.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://tv.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xw.colortex.cn

JS:   process.env.HOME
来源：http://zd.9csxet.cn

TS:   process.env.HOME
来源：http://hl.panjiajie.cn

Java: System.getenv("HOME")
来源：http://rb.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vd.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ut.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bn.521024.cn

[M03] 执行外部命令
来源：http://iz.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vs.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xx.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oa.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wz.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dz.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sy.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xz.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://zq.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://jy.wgjwhj.cn

Py:   os.getcwd()
来源：http://uu.yuexingan06.cn

PHP:  getcwd();
来源：http://om.lnxyls.cn

JS:   process.cwd()
来源：http://nb.huixinmuqiang.cn

TS:   process.cwd()
来源：http://lc.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://cf.bjjhwx.cn

Go:   os.Getwd()
来源：http://no.asd995.cn

Ruby: Dir.pwd
来源：http://zh.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vl.chemitech.net.cn

[M05] 设置退出码
来源：http://bs.szsharing.cn

Py:   sys.exit(1)
来源：http://yw.jianghongdianzi.cn

PHP:  exit(1);
来源：http://wn.shtwfgs.cn

JS:   process.exit(1)
来源：http://ym.bookmarksfly.cn

TS:   process.exit(1)
来源：http://zv.newstarts.cn

Java: System.exit(1)
来源：http://dd.hnjuh.cn

Go:   os.Exit(1)
来源：http://an.huanxung.cn

Ruby: exit 1
来源：http://gp.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fu.521024.cn

[M06] 向标准错误输出
来源：http://ku.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://pj.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qe.huixiangedu.cn

JS:   console.error("err")
来源：http://kz.asd995.cn

TS:   console.error("err")
来源：http://fi.jctech888.com.cn

Java: System.err.println("err")
来源：http://op.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ob.panjiajie.cn

Ruby: warn "err"
来源：http://yz.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://uf.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://bf.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://le.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dt.muxihuayi.cn

JS:   require.main === module
来源：http://ev.shxzskj.cn

TS:   require.main === module
来源：http://er.shxzskj.cn

Java: public static void main(String[] args)
来源：http://gs.jctech888.com.cn

Go:   func main()
来源：http://wj.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vq.colortex.cn

C#:   static void Main(string[] args)
来源：http://to.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://ei.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://br.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://zw.shxzukj.cn

JS:   process.platform;  process.version
来源：http://ca.hahajie.cn

TS:   process.platform;  process.version
来源：http://kj.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ef.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ru.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lg.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jt.hnjuh.cn

================================================================================
来源：http://rq.wgjwhj.cn

N. 数据结构与算法
来源：http://iu.huixinmuqiang.cn

================================================================================
来源：http://tv.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://fj.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ut.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hr.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://id.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jf.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qk.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://qw.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://os.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://co.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://eq.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://lz.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yg.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mt.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qt.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jx.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://rr.szxytkj.cn

Ruby: arr.sort
来源：http://ly.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vc.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://zt.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cc.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://cc.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qb.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vi.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uf.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lm.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tr.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fk.yuexingan06.cn

[N04] 斐波那契数列
来源：http://bk.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nk.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qi.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://so.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ok.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pz.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cy.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xe.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mh.jctech888.com.cn

[N05] 最大公约数
来源：http://lu.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://nt.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wz.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://au.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qt.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fz.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tq.521024.cn

Ruby: a.gcd(b)
来源：http://tf.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rd.9csxet.cn

[N06] 判断回文字符串
来源：http://tj.shxzukj.cn

Py:   s == s[::-1]
来源：http://zc.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://jc.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://gw.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://xu.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ka.9csxet.cn

Go:   // 双指针从两端比较
来源：http://cy.bookmarksfly.cn

Ruby: s == s.reverse
来源：http://qa.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sc.521024.cn

[N07] 两数之和（返回下标）
来源：http://xk.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ck.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://um.lnxyls.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mf.521024.cn

TS:   // 手写 Map<string, number>
来源：http://gb.muxihuayi.cn

Java: // 手写 HashMap
来源：http://la.szsharing.cn

Go:   // 手写 map[int]int
来源：http://tr.panjiajie.cn

Ruby: // 手写 Hash
来源：http://jb.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cl.huixiangedu.cn

[N08] 生成全排列
来源：http://mu.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://lo.hahajie.cn

PHP:  // 手写递归交换
来源：http://vr.nszjky.cn

JS:   // 手写回溯递归
来源：http://hu.nszjky.cn

TS:   // 手写回溯递归
来源：http://iv.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://it.521024.cn

Go:   // 手写回溯递归
来源：http://lt.asd995.cn

Ruby: arr.permutation.to_a
来源：http://lt.panjiajie.cn

C#:   // 手写回溯递归
来源：http://xp.hnjuh.cn

[N09] 栈与队列
来源：http://mu.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pg.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://el.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://io.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nw.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wy.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ki.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yl.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://te.szsharing.cn

[N10] 链表节点定义
来源：http://vv.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zu.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pr.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qx.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ay.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://nm.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cg.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ns.wgjwhj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://es.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://wu.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kl.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ds.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nm.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uj.shxzukj.cn

Java: // 手写递归
来源：http://em.bookmarksfly.cn

Go:   // 手写递归
来源：http://rl.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mw.jctech888.com.cn

C#:   // 手写递归
来源：http://oo.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bo.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xm.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wk.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rp.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lx.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jm.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ap.hnjuh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ja.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fk.chemitech.net.cn

================================================================================
来源：http://hx.shxzskj.cn

O. 并发与异步
来源：http://cx.gzmigu.cn

================================================================================
来源：http://nj.szxytkj.cn

[O01] 启动一个线程
来源：http://hm.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rs.shtwfgs.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xz.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uv.gzmigu.cn

TS:   // 同 JS
来源：http://cd.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://da.shxzskj.cn

Go:   go f()
来源：http://pc.colortex.cn

Ruby: Thread.new { f }
来源：http://fx.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://bk.521024.cn

[O02] 使用线程池
来源：http://pu.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rf.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rc.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://ii.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://ji.nicolike.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oz.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rg.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ui.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jo.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://iu.muxihuayi.cn

Py:   with lock: shared += 1
来源：http://uc.haigaiapp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qo.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iz.jctech888.com.cn

TS:   // 同 JS
来源：http://gq.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://ag.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nl.huanxung.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wr.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ro.jianghongdianzi.cn

[O04] 定义异步函数并等待
来源：http://de.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://sy.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dm.bjjhwx.cn

JS:   async function f() { await g(); }
来源：http://vq.shxzukj.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ew.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oy.hnjuh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ba.huixiangedu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wj.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://gz.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://wj.panjiajie.cn

Py:   asyncio.gather(*tasks)
来源：http://kz.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xs.9csxet.cn

JS:   await Promise.all(tasks)
来源：http://rk.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ag.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ds.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dj.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://hj.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xy.9csxet.cn

[O06] 使用进程池
来源：http://uc.huixinmuqiang.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hu.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mi.jctech888.com.cn

JS:   // child_process / cluster 模块
来源：http://gi.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://kp.yuexingan06.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xv.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yx.yuexingan06.cn

Ruby: // fork 块
来源：http://im.jctech888.com.cn

C#:   Parallel.For
来源：http://xw.huixiangedu.cn

================================================================================
来源：http://jy.yuexingan06.cn

P. 常用工具函数
来源：http://bl.panjiajie.cn

================================================================================
来源：http://bd.wgjwhj.cn

[P01] 生成 UUID
来源：http://qw.521024.cn

Py:   str(uuid.uuid4())
来源：http://cf.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vi.jctech888.com.cn

JS:   crypto.randomUUID()
来源：http://vd.yuntaijiaju.cn

TS:   crypto.randomUUID()
来源：http://fg.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://zl.asd995.cn

Go:   // 用 github.com/google/uuid
来源：http://ag.yuntaijiaju.cn

Ruby: SecureRandom.uuid
来源：http://tr.szxytkj.cn

C#:   Guid.NewGuid().ToString()
来源：http://wl.bookmarksfly.cn

[P02] MD5 / SHA256 摘要
来源：http://ps.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://th.jctech888.com.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://us.yuntaijiaju.cn


<!-- 参考信息 -->