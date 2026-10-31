代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://od.wgjwhj.cn

[L04] 设置超时
来源：http://sw.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://uf.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ni.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ia.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vw.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hr.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://on.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kj.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://we.szsharing.cn

[L05] 上传文件（multipart）
来源：http://pi.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uf.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nh.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yq.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://be.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://my.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hq.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iw.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://hq.newstarts.cn

Py:   resp.json()
来源：http://mc.szsharing.cn

PHP:  json_decode($body, true);
来源：http://ff.wgjwhj.cn

JS:   await resp.json()
来源：http://cm.muxihuayi.cn

TS:   await resp.json()
来源：http://bn.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kc.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zw.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://dn.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sq.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://rf.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kf.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ya.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://bj.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://zj.chemitech.net.cn

Java: resp.statusCode()
来源：http://ff.shxzskj.cn

Go:   resp.StatusCode
来源：http://iu.gzmigu.cn

Ruby: resp.code.to_i
来源：http://qa.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://qj.asd995.cn

[L08] 并发请求多个地址
来源：http://qk.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ql.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://yh.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://al.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vi.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hw.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cj.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ho.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ag.shtwfgs.cn

================================================================================
来源：http://kx.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://yf.huanxung.cn

================================================================================
来源：http://in.szsharing.cn

[M01] 读取命令行参数
来源：http://hx.asd995.cn

Py:   sys.argv[1:]
来源：http://ey.szsharing.cn

PHP:  $argv;  $argc;
来源：http://tq.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ut.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://wn.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://nc.chemitech.net.cn

Go:   os.Args[1:]
来源：http://bi.muxihuayi.cn

Ruby: ARGV
来源：http://av.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://zm.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://hw.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://br.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sd.shxzukj.cn

JS:   process.env.HOME
来源：http://xo.szxytkj.cn

TS:   process.env.HOME
来源：http://mh.asd995.cn

Java: System.getenv("HOME")
来源：http://lo.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tx.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://ps.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ey.521024.cn

[M03] 执行外部命令
来源：http://vd.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hh.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hn.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ui.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rc.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ra.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lm.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dx.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://dy.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://jl.bjjhwx.cn

Py:   os.getcwd()
来源：http://ff.hnjuh.cn

PHP:  getcwd();
来源：http://ur.huixiangedu.cn

JS:   process.cwd()
来源：http://mx.haigaiapp.cn

TS:   process.cwd()
来源：http://rp.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bj.colortex.cn

Go:   os.Getwd()
来源：http://qz.nicolike.cn

Ruby: Dir.pwd
来源：http://oi.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qq.521024.cn

[M05] 设置退出码
来源：http://tv.wgjwhj.cn

Py:   sys.exit(1)
来源：http://ga.9csxet.cn

PHP:  exit(1);
来源：http://nr.9csxet.cn

JS:   process.exit(1)
来源：http://es.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ob.chemitech.net.cn

Java: System.exit(1)
来源：http://wr.shtwfgs.cn

Go:   os.Exit(1)
来源：http://bg.haigaiapp.cn

Ruby: exit 1
来源：http://aw.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ie.bjjhwx.cn

[M06] 向标准错误输出
来源：http://mo.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://je.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ar.gzmigu.cn

JS:   console.error("err")
来源：http://vr.9csxet.cn

TS:   console.error("err")
来源：http://tz.gzmigu.cn

Java: System.err.println("err")
来源：http://mn.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://re.521024.cn

Ruby: warn "err"
来源：http://nb.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://zg.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://ql.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://jh.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rz.hahajie.cn

JS:   require.main === module
来源：http://sw.huixiangedu.cn

TS:   require.main === module
来源：http://ka.szsharing.cn

Java: public static void main(String[] args)
来源：http://np.521024.cn

Go:   func main()
来源：http://rk.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lc.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://rv.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://mu.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://px.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://dw.lnxyls.cn

JS:   process.platform;  process.version
来源：http://ze.hnjuh.cn

TS:   process.platform;  process.version
来源：http://qy.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://al.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zg.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ct.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hm.szsharing.cn

================================================================================
来源：http://yv.newstarts.cn

N. 数据结构与算法
来源：http://ck.huixinmuqiang.cn

================================================================================
来源：http://wc.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://pp.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fl.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vw.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://na.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ut.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ci.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://oa.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jy.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tp.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://zi.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ef.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fp.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qv.muxihuayi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wr.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wi.newstarts.cn

Go:   slices.Sort(arr)
来源：http://pv.asd995.cn

Ruby: arr.sort
来源：http://ae.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yz.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://we.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vs.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://ay.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://on.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tz.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ke.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yd.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cb.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xn.nszjky.cn

[N04] 斐波那契数列
来源：http://gi.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ru.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xb.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://se.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nb.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iy.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lu.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fr.gzmigu.cn

[N05] 最大公约数
来源：http://cg.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://nd.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cm.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pv.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ne.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jm.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://df.hahajie.cn

Ruby: a.gcd(b)
来源：http://dx.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wy.shxzskj.cn

[N06] 判断回文字符串
来源：http://np.wgjwhj.cn

Py:   s == s[::-1]
来源：http://na.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://ps.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://rj.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://lt.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sv.nicolike.cn

Go:   // 双指针从两端比较
来源：http://ms.szsharing.cn

Ruby: s == s.reverse
来源：http://oh.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bs.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://ii.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nv.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pm.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tn.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://za.nszjky.cn

Java: // 手写 HashMap
来源：http://iz.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://na.nicolike.cn

Ruby: // 手写 Hash
来源：http://qk.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ii.yuntaijiaju.cn

[N08] 生成全排列
来源：http://rv.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ue.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://gj.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://gd.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://mq.nicolike.cn

Java: // 手写回溯递归
来源：http://pd.panjiajie.cn

Go:   // 手写回溯递归
来源：http://ie.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://rl.hnjuh.cn

C#:   // 手写回溯递归
来源：http://ph.szxytkj.cn

[N09] 栈与队列
来源：http://pe.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kv.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xu.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ut.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wd.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qo.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jw.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://py.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jd.shxzukj.cn

[N10] 链表节点定义
来源：http://dc.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tn.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oe.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xt.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ni.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ou.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pl.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xo.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pg.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://fq.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wq.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://dz.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rn.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gu.huanxung.cn

Java: // 手写递归
来源：http://re.jctech888.com.cn

Go:   // 手写递归
来源：http://cr.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://em.wgjwhj.cn

C#:   // 手写递归
来源：http://ce.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bv.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pq.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oi.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rr.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://de.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bp.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lj.huixinmuqiang.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zu.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lh.huanxung.cn

================================================================================
来源：http://eu.huanxung.cn

O. 并发与异步
来源：http://nq.huixinmuqiang.cn

================================================================================
来源：http://ku.asd995.cn

[O01] 启动一个线程
来源：http://zv.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dy.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://js.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pw.hnjuh.cn

TS:   // 同 JS
来源：http://qa.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://py.nicolike.cn

Go:   go f()
来源：http://aa.huanxung.cn

Ruby: Thread.new { f }
来源：http://ql.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://wh.nszjky.cn

[O02] 使用线程池
来源：http://he.lnxyls.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ai.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pa.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ia.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://ny.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://im.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://da.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gy.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eh.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://sv.szsharing.cn

Py:   with lock: shared += 1
来源：http://ru.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://sd.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://in.newstarts.cn

TS:   // 同 JS
来源：http://xv.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://pi.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pq.huixiangedu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nu.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://tr.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://yd.nicolike.cn

Py:   async def f():⏎    await g()
来源：http://vb.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mu.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://tf.hnjuh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uf.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ir.nicolike.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ph.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bu.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://gd.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://jz.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://bo.yuntaijiaju.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xk.nicolike.cn

JS:   await Promise.all(tasks)
来源：http://js.shxzskj.cn

TS:   await Promise.all(tasks)
来源：http://ib.521024.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uk.hahajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kx.bjjhwx.cn

Ruby: threads.map(&:join)
来源：http://or.asd995.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bz.shtwfgs.cn

[O06] 使用进程池
来源：http://eq.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wd.newstarts.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wo.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://qq.panjiajie.cn

TS:   // child_process / cluster 模块
来源：http://dj.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pb.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wz.nicolike.cn

Ruby: // fork 块
来源：http://iz.asd995.cn

C#:   Parallel.For
来源：http://nu.szxytkj.cn

================================================================================
来源：http://aj.yuexingan06.cn

P. 常用工具函数
来源：http://fj.chemitech.net.cn

================================================================================
来源：http://qp.wgjwhj.cn

[P01] 生成 UUID
来源：http://zg.jctech888.com.cn

Py:   str(uuid.uuid4())
来源：http://xn.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oa.hahajie.cn

JS:   crypto.randomUUID()
来源：http://du.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://mr.gzmigu.cn

Java: UUID.randomUUID().toString()
来源：http://zf.haigaiapp.cn

Go:   // 用 github.com/google/uuid
来源：http://tq.haigaiapp.cn

Ruby: SecureRandom.uuid
来源：http://vw.9csxet.cn


<!-- 参考信息 -->