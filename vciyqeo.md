代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tz.huixiangedu.cn

[L04] 设置超时
来源：http://ee.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://rh.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://md.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hw.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ud.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://se.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eq.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lw.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qc.asd995.cn

[L05] 上传文件（multipart）
来源：http://ne.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jd.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yl.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rq.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kh.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sh.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tu.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hj.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nf.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://hj.bookmarksfly.cn

Py:   resp.json()
来源：http://tl.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://vz.bjjhwx.cn

JS:   await resp.json()
来源：http://dm.huixiangedu.cn

TS:   await resp.json()
来源：http://fp.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nc.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wt.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://uw.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kk.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://is.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xo.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nh.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://gt.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://bg.lnxyls.cn

Java: resp.statusCode()
来源：http://bf.lnxyls.cn

Go:   resp.StatusCode
来源：http://qz.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://jy.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://rb.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://qe.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://av.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://zc.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ig.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iq.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fn.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lb.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ff.gzmigu.cn

================================================================================
来源：http://gc.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://mo.nicolike.cn

================================================================================
来源：http://tt.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://cc.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://pp.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://vi.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://nh.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://yc.asd995.cn

Java: args 数组（main 方法参数）
来源：http://gc.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://ar.521024.cn

Ruby: ARGV
来源：http://re.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://zl.asd995.cn

[M02] 读取环境变量
来源：http://bl.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://cf.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vj.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://dw.panjiajie.cn

TS:   process.env.HOME
来源：http://gs.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://iq.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vd.nicolike.cn

Ruby: ENV["HOME"]
来源：http://vg.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lt.bjjhwx.cn

[M03] 执行外部命令
来源：http://sn.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ik.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wf.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vo.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qu.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jr.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pp.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hx.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://tl.shxzukj.cn

[M04] 获取当前工作目录
来源：http://im.colortex.cn

Py:   os.getcwd()
来源：http://gr.jianghongdianzi.cn

PHP:  getcwd();
来源：http://hw.nszjky.cn

JS:   process.cwd()
来源：http://qk.gzmigu.cn

TS:   process.cwd()
来源：http://yz.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ny.asd995.cn

Go:   os.Getwd()
来源：http://zy.shxzskj.cn

Ruby: Dir.pwd
来源：http://zm.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iz.nszjky.cn

[M05] 设置退出码
来源：http://hv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://jf.muxihuayi.cn

PHP:  exit(1);
来源：http://bi.wgjwhj.cn

JS:   process.exit(1)
来源：http://sw.wgjwhj.cn

TS:   process.exit(1)
来源：http://ql.wgjwhj.cn

Java: System.exit(1)
来源：http://bk.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://xw.huixiangedu.cn

Ruby: exit 1
来源：http://mc.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://om.nszjky.cn

[M06] 向标准错误输出
来源：http://lo.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ey.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cm.bookmarksfly.cn

JS:   console.error("err")
来源：http://yd.muxihuayi.cn

TS:   console.error("err")
来源：http://qg.nicolike.cn

Java: System.err.println("err")
来源：http://yv.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hb.nicolike.cn

Ruby: warn "err"
来源：http://bb.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ei.szxytkj.cn

[M07] 判断是否为主入口
来源：http://gi.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://oj.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tj.nicolike.cn

JS:   require.main === module
来源：http://oa.bjjhwx.cn

TS:   require.main === module
来源：http://fy.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://bb.newstarts.cn

Go:   func main()
来源：http://hh.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gd.colortex.cn

C#:   static void Main(string[] args)
来源：http://ix.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://xf.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://qr.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://em.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://ds.asd995.cn

TS:   process.platform;  process.version
来源：http://ue.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ww.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wm.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ag.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pk.szsharing.cn

================================================================================
来源：http://zz.asd995.cn

N. 数据结构与算法
来源：http://ev.lnxyls.cn

================================================================================
来源：http://ti.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://yk.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://js.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bd.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://np.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rj.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ok.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://vg.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pv.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aj.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://up.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ou.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dn.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tn.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ps.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cx.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://sr.wgjwhj.cn

Ruby: arr.sort
来源：http://ca.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://il.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://nv.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uu.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://qb.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vp.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tf.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ln.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ob.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ec.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qf.9csxet.cn

[N04] 斐波那契数列
来源：http://nh.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vt.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pt.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mr.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ga.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aw.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ne.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lz.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rl.9csxet.cn

[N05] 最大公约数
来源：http://ll.colortex.cn

Py:   math.gcd(a, b)
来源：http://ae.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://li.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yl.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lh.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ps.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hu.asd995.cn

Ruby: a.gcd(b)
来源：http://yj.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uq.panjiajie.cn

[N06] 判断回文字符串
来源：http://lv.hahajie.cn

Py:   s == s[::-1]
来源：http://ky.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://dp.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://hm.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://lx.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fm.nszjky.cn

Go:   // 双指针从两端比较
来源：http://tv.szxytkj.cn

Ruby: s == s.reverse
来源：http://cj.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rw.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://yh.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ic.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zs.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ug.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://qg.jctech888.com.cn

Java: // 手写 HashMap
来源：http://id.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://sv.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://no.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cq.szxytkj.cn

[N08] 生成全排列
来源：http://dm.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://gc.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://nh.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://xb.521024.cn

TS:   // 手写回溯递归
来源：http://fx.asd995.cn

Java: // 手写回溯递归
来源：http://vo.gzmigu.cn

Go:   // 手写回溯递归
来源：http://eb.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://pa.shxzskj.cn

C#:   // 手写回溯递归
来源：http://qn.bjjhwx.cn

[N09] 栈与队列
来源：http://ta.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vv.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xg.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://it.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yy.hahajie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mj.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jv.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lv.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lg.521024.cn

[N10] 链表节点定义
来源：http://yf.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mj.shxzskj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wq.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tn.szsharing.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wa.shxzukj.cn

Java: class Node { int v; Node next; }
来源：http://yo.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fj.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ej.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hl.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://aq.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://te.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://sk.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rr.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ft.hahajie.cn

Java: // 手写递归
来源：http://qb.9csxet.cn

Go:   // 手写递归
来源：http://sd.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rv.huixinmuqiang.cn

C#:   // 手写递归
来源：http://uz.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ad.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qm.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cs.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uw.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kw.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cl.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zp.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ga.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ay.nicolike.cn

================================================================================
来源：http://ys.nicolike.cn

O. 并发与异步
来源：http://ow.bjjhwx.cn

================================================================================
来源：http://kn.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://zg.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mz.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lx.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oi.shtwfgs.cn

TS:   // 同 JS
来源：http://ya.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://uj.panjiajie.cn

Go:   go f()
来源：http://za.szxytkj.cn

Ruby: Thread.new { f }
来源：http://xp.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://xj.9csxet.cn

[O02] 使用线程池
来源：http://jf.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rp.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vz.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://wu.nszjky.cn

TS:   // worker_threads 线程池
来源：http://kj.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ht.yuntaijiaju.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rm.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://og.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wu.newstarts.cn

[O03] 加锁保护共享数据
来源：http://my.panjiajie.cn

Py:   with lock: shared += 1
来源：http://bq.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://me.asd995.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sq.asd995.cn

TS:   // 同 JS
来源：http://xo.hahajie.cn

Java: synchronized (this) { shared++; }
来源：http://kf.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qk.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bk.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://dg.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://oe.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://qf.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gw.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://lc.521024.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ce.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qq.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hy.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://at.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://nj.huixinmuqiang.cn

[O05] 并发执行并等待全部完成
来源：http://mk.hahajie.cn

Py:   asyncio.gather(*tasks)
来源：http://ax.haigaiapp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nq.chemitech.net.cn

JS:   await Promise.all(tasks)
来源：http://pq.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://xb.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bz.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bx.huixiangedu.cn

Ruby: threads.map(&:join)
来源：http://ye.shtwfgs.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mi.yuexingan06.cn

[O06] 使用进程池
来源：http://yu.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wv.colortex.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ll.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://oa.lnxyls.cn

TS:   // child_process / cluster 模块
来源：http://hy.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bd.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cn.nszjky.cn

Ruby: // fork 块
来源：http://ip.gzmigu.cn

C#:   Parallel.For
来源：http://et.szxytkj.cn

================================================================================
来源：http://ci.yuexingan06.cn

P. 常用工具函数
来源：http://zn.shxzskj.cn

================================================================================
来源：http://ys.szxytkj.cn

[P01] 生成 UUID
来源：http://of.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://fy.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qj.9csxet.cn

JS:   crypto.randomUUID()
来源：http://zl.9csxet.cn

TS:   crypto.randomUUID()
来源：http://bn.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://dm.hnjuh.cn

Go:   // 用 github.com/google/uuid
来源：http://fj.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://yh.shxzukj.cn


<!-- 参考信息 -->