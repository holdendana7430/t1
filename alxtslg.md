代发 wailian999

[L03] 设置自定义请求头
来源：http://jw.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qf.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nl.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ax.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ho.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qd.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qz.nszjky.cn

[L04] 设置超时
来源：http://yk.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://go.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wf.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ss.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://db.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mh.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hr.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cf.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ry.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://pt.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vc.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ll.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dj.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ar.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pl.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xo.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ai.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xw.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://km.yuexingan06.cn

Py:   resp.json()
来源：http://pr.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://rg.haigaiapp.cn

JS:   await resp.json()
来源：http://gd.jianghongdianzi.cn

TS:   await resp.json()
来源：http://we.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gz.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vv.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://lm.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pv.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://xn.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vc.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xu.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://nq.colortex.cn

TS:   resp.ok;  resp.status
来源：http://yn.shtwfgs.cn

Java: resp.statusCode()
来源：http://ox.jctech888.com.cn

Go:   resp.StatusCode
来源：http://jk.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://cz.colortex.cn

C#:   (int)resp.StatusCode
来源：http://mx.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://rv.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nu.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://bo.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rc.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ek.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gj.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ba.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ll.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ju.asd995.cn

================================================================================
来源：http://fi.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://eu.huanxung.cn

================================================================================
来源：http://zt.nicolike.cn

[M01] 读取命令行参数
来源：http://fm.colortex.cn

Py:   sys.argv[1:]
来源：http://vi.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://vz.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://me.szsharing.cn

TS:   process.argv.slice(2)
来源：http://mm.colortex.cn

Java: args 数组（main 方法参数）
来源：http://vl.panjiajie.cn

Go:   os.Args[1:]
来源：http://uy.panjiajie.cn

Ruby: ARGV
来源：http://aa.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://kh.shxzskj.cn

[M02] 读取环境变量
来源：http://bb.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://ar.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ws.shxzskj.cn

JS:   process.env.HOME
来源：http://xd.szxytkj.cn

TS:   process.env.HOME
来源：http://ah.szxytkj.cn

Java: System.getenv("HOME")
来源：http://us.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qc.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://yw.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qf.nszjky.cn

[M03] 执行外部命令
来源：http://px.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dj.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pb.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tg.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ui.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qs.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tx.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mf.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://mp.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://ex.huixiangedu.cn

Py:   os.getcwd()
来源：http://wc.yuntaijiaju.cn

PHP:  getcwd();
来源：http://th.yuexingan06.cn

JS:   process.cwd()
来源：http://ji.9csxet.cn

TS:   process.cwd()
来源：http://ff.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://fz.wgjwhj.cn

Go:   os.Getwd()
来源：http://mb.gzmigu.cn

Ruby: Dir.pwd
来源：http://wa.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oe.haigaiapp.cn

[M05] 设置退出码
来源：http://cy.521024.cn

Py:   sys.exit(1)
来源：http://ul.hnjuh.cn

PHP:  exit(1);
来源：http://ig.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://kq.szxytkj.cn

TS:   process.exit(1)
来源：http://eg.yuexingan06.cn

Java: System.exit(1)
来源：http://bh.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://it.jctech888.com.cn

Ruby: exit 1
来源：http://pu.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://je.shxzskj.cn

[M06] 向标准错误输出
来源：http://ug.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://ge.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vu.9csxet.cn

JS:   console.error("err")
来源：http://jf.nszjky.cn

TS:   console.error("err")
来源：http://fs.panjiajie.cn

Java: System.err.println("err")
来源：http://gt.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kd.szxytkj.cn

Ruby: warn "err"
来源：http://li.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://yf.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://za.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://ka.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pc.szxytkj.cn

JS:   require.main === module
来源：http://mf.haigaiapp.cn

TS:   require.main === module
来源：http://tm.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://wl.9csxet.cn

Go:   func main()
来源：http://jb.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cs.521024.cn

C#:   static void Main(string[] args)
来源：http://sj.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://vx.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://jl.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://qm.huanxung.cn

JS:   process.platform;  process.version
来源：http://px.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://py.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sf.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aq.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cm.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vh.muxihuayi.cn

================================================================================
来源：http://pq.haigaiapp.cn

N. 数据结构与算法
来源：http://ll.bjjhwx.cn

================================================================================
来源：http://wo.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://sp.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nc.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ul.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vy.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ao.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gy.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://bb.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lw.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://og.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://aq.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://zf.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ej.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qd.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zk.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yi.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://uh.haigaiapp.cn

Ruby: arr.sort
来源：http://vn.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hi.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://xi.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://si.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://kf.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://by.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jd.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://no.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ih.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oz.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nl.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://in.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mh.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://no.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ps.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lx.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zs.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cz.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fd.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gg.bookmarksfly.cn

[N05] 最大公约数
来源：http://tz.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://xh.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pa.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dz.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kc.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tt.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ng.hahajie.cn

Ruby: a.gcd(b)
来源：http://rn.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qg.9csxet.cn

[N06] 判断回文字符串
来源：http://il.nszjky.cn

Py:   s == s[::-1]
来源：http://dm.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://ks.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://lp.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://vd.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ta.hahajie.cn

Go:   // 双指针从两端比较
来源：http://zv.hahajie.cn

Ruby: s == s.reverse
来源：http://tm.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zb.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://hp.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://as.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ys.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vf.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://qo.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://qe.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://nw.521024.cn

Ruby: // 手写 Hash
来源：http://hg.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vk.hnjuh.cn

[N08] 生成全排列
来源：http://ph.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://ws.9csxet.cn

PHP:  // 手写递归交换
来源：http://ks.hnjuh.cn

JS:   // 手写回溯递归
来源：http://tu.nszjky.cn

TS:   // 手写回溯递归
来源：http://np.chemitech.net.cn

Java: // 手写回溯递归
来源：http://wv.asd995.cn

Go:   // 手写回溯递归
来源：http://kc.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://sa.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://kl.shxzukj.cn

[N09] 栈与队列
来源：http://uf.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ro.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lv.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bx.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ek.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ch.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xi.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pe.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ro.521024.cn

[N10] 链表节点定义
来源：http://sw.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zl.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mi.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fj.hahajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sg.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://uf.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rf.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hc.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ub.hahajie.cn

[N11] 二叉树中序遍历
来源：http://uy.wgjwhj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bc.szsharing.cn

PHP:  // 手写递归函数
来源：http://uh.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ip.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dq.gzmigu.cn

Java: // 手写递归
来源：http://nv.nicolike.cn

Go:   // 手写递归
来源：http://hw.szxytkj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rf.9csxet.cn

C#:   // 手写递归
来源：http://ol.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kf.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tl.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ha.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wh.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mp.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dt.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pv.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mo.huixinmuqiang.cn

================================================================================
来源：http://pc.yuntaijiaju.cn

O. 并发与异步
来源：http://pv.muxihuayi.cn

================================================================================
来源：http://vs.szxytkj.cn

[O01] 启动一个线程
来源：http://cb.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nv.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vn.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xd.szsharing.cn

TS:   // 同 JS
来源：http://wi.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://mk.gzmigu.cn

Go:   go f()
来源：http://in.nszjky.cn

Ruby: Thread.new { f }
来源：http://ku.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://nm.521024.cn

[O02] 使用线程池
来源：http://xd.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cx.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://li.bookmarksfly.cn

JS:   // worker_threads 线程池
来源：http://kb.gzmigu.cn

TS:   // worker_threads 线程池
来源：http://cn.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fo.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qd.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qk.colortex.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xc.yuntaijiaju.cn

[O03] 加锁保护共享数据
来源：http://ae.9csxet.cn

Py:   with lock: shared += 1
来源：http://wf.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ew.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ut.lnxyls.cn

TS:   // 同 JS
来源：http://la.yuntaijiaju.cn

Java: synchronized (this) { shared++; }
来源：http://jj.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wm.shxzskj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pg.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://br.9csxet.cn

[O04] 定义异步函数并等待
来源：http://xk.yuexingan06.cn

Py:   async def f():⏎    await g()
来源：http://jy.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vw.jianghongdianzi.cn

JS:   async function f() { await g(); }
来源：http://wv.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tw.newstarts.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://os.bookmarksfly.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lf.asd995.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jp.chemitech.net.cn

C#:   async Task F() { await G(); }
来源：http://ju.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://pu.szsharing.cn

Py:   asyncio.gather(*tasks)
来源：http://ek.panjiajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ck.haigaiapp.cn

JS:   await Promise.all(tasks)
来源：http://gg.lnxyls.cn

TS:   await Promise.all(tasks)
来源：http://qq.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://io.nszjky.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://no.szsharing.cn

Ruby: threads.map(&:join)
来源：http://la.bookmarksfly.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zs.bjjhwx.cn

[O06] 使用进程池
来源：http://dw.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vk.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wa.yuntaijiaju.cn

JS:   // child_process / cluster 模块
来源：http://pg.shxzukj.cn

TS:   // child_process / cluster 模块
来源：http://ve.shxzukj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://di.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eu.521024.cn

Ruby: // fork 块
来源：http://cz.shxzukj.cn

C#:   Parallel.For
来源：http://um.bookmarksfly.cn

================================================================================
来源：http://xp.hahajie.cn

P. 常用工具函数
来源：http://ro.yuexingan06.cn

================================================================================
来源：http://yh.chemitech.net.cn


<!-- 参考信息 -->