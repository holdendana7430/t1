代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fd.szxytkj.cn

[L04] 设置超时
来源：http://pw.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://hb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://md.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://il.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lp.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uw.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ra.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fl.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bo.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://lg.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ol.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xg.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bm.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bh.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gl.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bk.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cf.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lo.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://ug.huixiangedu.cn

Py:   resp.json()
来源：http://kv.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://xo.bjjhwx.cn

JS:   await resp.json()
来源：http://nb.wgjwhj.cn

TS:   await resp.json()
来源：http://if.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dg.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vr.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://tb.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iu.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://qb.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xf.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wx.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://zy.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://lo.asd995.cn

Java: resp.statusCode()
来源：http://vh.newstarts.cn

Go:   resp.StatusCode
来源：http://pd.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ru.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://zm.521024.cn

[L08] 并发请求多个地址
来源：http://zd.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vv.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://hk.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jo.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dj.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jb.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mz.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xz.szxytkj.cn

================================================================================
来源：http://gv.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://lj.9csxet.cn

================================================================================
来源：http://rv.jctech888.com.cn

[M01] 读取命令行参数
来源：http://kx.9csxet.cn

Py:   sys.argv[1:]
来源：http://su.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://zo.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://jk.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://zn.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://aj.panjiajie.cn

Go:   os.Args[1:]
来源：http://ql.colortex.cn

Ruby: ARGV
来源：http://py.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://nw.521024.cn

[M02] 读取环境变量
来源：http://ka.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://pk.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bs.yuexingan06.cn

JS:   process.env.HOME
来源：http://so.szsharing.cn

TS:   process.env.HOME
来源：http://sa.huanxung.cn

Java: System.getenv("HOME")
来源：http://nj.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ww.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://nb.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ix.muxihuayi.cn

[M03] 执行外部命令
来源：http://hb.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ck.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://st.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vf.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mo.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tw.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zf.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sk.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://al.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://gg.jctech888.com.cn

Py:   os.getcwd()
来源：http://lg.shxzskj.cn

PHP:  getcwd();
来源：http://mn.newstarts.cn

JS:   process.cwd()
来源：http://ls.huixinmuqiang.cn

TS:   process.cwd()
来源：http://yo.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://oj.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://rb.shtwfgs.cn

Ruby: Dir.pwd
来源：http://se.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tr.hnjuh.cn

[M05] 设置退出码
来源：http://kd.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://vi.shxzukj.cn

PHP:  exit(1);
来源：http://jb.szsharing.cn

JS:   process.exit(1)
来源：http://me.szsharing.cn

TS:   process.exit(1)
来源：http://sx.521024.cn

Java: System.exit(1)
来源：http://uf.haigaiapp.cn

Go:   os.Exit(1)
来源：http://jk.bjjhwx.cn

Ruby: exit 1
来源：http://pa.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pg.huixiangedu.cn

[M06] 向标准错误输出
来源：http://gl.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://kd.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qs.newstarts.cn

JS:   console.error("err")
来源：http://zt.muxihuayi.cn

TS:   console.error("err")
来源：http://ki.huixiangedu.cn

Java: System.err.println("err")
来源：http://an.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wn.asd995.cn

Ruby: warn "err"
来源：http://nc.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://yd.nszjky.cn

[M07] 判断是否为主入口
来源：http://tm.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://zo.newstarts.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cb.wgjwhj.cn

JS:   require.main === module
来源：http://fp.asd995.cn

TS:   require.main === module
来源：http://oi.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://lh.yuexingan06.cn

Go:   func main()
来源：http://br.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qz.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://ni.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://om.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://pj.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://cc.colortex.cn

JS:   process.platform;  process.version
来源：http://vl.gzmigu.cn

TS:   process.platform;  process.version
来源：http://qg.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://is.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oz.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qs.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wo.huanxung.cn

================================================================================
来源：http://si.jianghongdianzi.cn

N. 数据结构与算法
来源：http://at.jianghongdianzi.cn

================================================================================
来源：http://pn.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://uq.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zv.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ei.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://id.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zj.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xp.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://gs.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bw.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qh.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://sz.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://sc.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bw.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vf.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dq.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ib.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://ql.asd995.cn

Ruby: arr.sort
来源：http://fi.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ex.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://dc.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://by.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://jh.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qb.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sw.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ix.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jn.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eb.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mj.szsharing.cn

[N04] 斐波那契数列
来源：http://xt.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kq.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ey.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lg.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ox.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pp.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tg.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://su.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ul.nszjky.cn

[N05] 最大公约数
来源：http://fq.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://be.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nc.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vj.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ob.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fp.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ta.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://za.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xn.nicolike.cn

[N06] 判断回文字符串
来源：http://tg.lnxyls.cn

Py:   s == s[::-1]
来源：http://po.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://eu.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://zt.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://bl.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bt.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://me.shxzskj.cn

Ruby: s == s.reverse
来源：http://wn.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yg.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://gb.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ot.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jt.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ve.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://hy.szxytkj.cn

Java: // 手写 HashMap
来源：http://uu.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://sp.gzmigu.cn

Ruby: // 手写 Hash
来源：http://vq.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yr.szxytkj.cn

[N08] 生成全排列
来源：http://bh.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://mx.colortex.cn

PHP:  // 手写递归交换
来源：http://zm.asd995.cn

JS:   // 手写回溯递归
来源：http://rp.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://un.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://ou.nicolike.cn

Go:   // 手写回溯递归
来源：http://be.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://rd.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://pt.521024.cn

[N09] 栈与队列
来源：http://iz.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zf.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mh.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sn.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ri.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://es.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nv.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ic.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sl.nicolike.cn

[N10] 链表节点定义
来源：http://gu.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uw.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ws.asd995.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ft.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://na.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://uq.lnxyls.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nt.yuntaijiaju.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uy.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xx.newstarts.cn

[N11] 二叉树中序遍历
来源：http://jy.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eh.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://dn.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kd.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rv.gzmigu.cn

Java: // 手写递归
来源：http://rd.shtwfgs.cn

Go:   // 手写递归
来源：http://cv.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bw.bjjhwx.cn

C#:   // 手写递归
来源：http://ir.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rl.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://og.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cw.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mh.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://is.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lr.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://om.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zb.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nr.bjjhwx.cn

================================================================================
来源：http://ci.muxihuayi.cn

O. 并发与异步
来源：http://uj.yuexingan06.cn

================================================================================
来源：http://sg.shxzskj.cn

[O01] 启动一个线程
来源：http://kh.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uv.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lo.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jk.gzmigu.cn

TS:   // 同 JS
来源：http://gt.521024.cn

Java: new Thread(() -> f()).start()
来源：http://hs.shxzskj.cn

Go:   go f()
来源：http://wt.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://yo.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://uz.huanxung.cn

[O02] 使用线程池
来源：http://vv.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mn.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xq.huixinmuqiang.cn

JS:   // worker_threads 线程池
来源：http://qe.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://gj.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mb.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://al.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nk.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vn.nszjky.cn

[O03] 加锁保护共享数据
来源：http://gf.521024.cn

Py:   with lock: shared += 1
来源：http://hc.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://wi.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ne.nicolike.cn

TS:   // 同 JS
来源：http://fi.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://ct.huixinmuqiang.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sf.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dc.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://ci.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://ph.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://wb.colortex.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pf.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://ee.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mw.shxzskj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uq.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://so.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://us.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://dy.asd995.cn

[O05] 并发执行并等待全部完成
来源：http://nf.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://ge.shxzskj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tp.asd995.cn

JS:   await Promise.all(tasks)
来源：http://tn.shtwfgs.cn

TS:   await Promise.all(tasks)
来源：http://iw.shtwfgs.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://re.chemitech.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ub.newstarts.cn

Ruby: threads.map(&:join)
来源：http://kn.szxytkj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cv.hahajie.cn

[O06] 使用进程池
来源：http://hd.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fd.nicolike.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yd.lnxyls.cn

JS:   // child_process / cluster 模块
来源：http://ox.szsharing.cn

TS:   // child_process / cluster 模块
来源：http://df.9csxet.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ia.shxzskj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hl.jctech888.com.cn

Ruby: // fork 块
来源：http://ro.huanxung.cn

C#:   Parallel.For
来源：http://ja.lnxyls.cn

================================================================================
来源：http://oe.chemitech.net.cn

P. 常用工具函数
来源：http://hi.huanxung.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://io.haigaiapp.cn

Py:   str(uuid.uuid4())
来源：http://fd.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://re.huixiangedu.cn

JS:   crypto.randomUUID()
来源：http://ki.bjjhwx.cn

TS:   crypto.randomUUID()
来源：http://fu.lnxyls.cn

Java: UUID.randomUUID().toString()
来源：http://lk.nicolike.cn

Go:   // 用 github.com/google/uuid
来源：http://pk.shxzukj.cn

Ruby: SecureRandom.uuid
来源：http://ed.huixiangedu.cn


<!-- 参考信息 -->