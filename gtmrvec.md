代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xn.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vu.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ug.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ya.jianghongdianzi.cn

[L04] 设置超时
来源：http://rp.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://vj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vk.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tr.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lx.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zx.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hb.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hf.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ck.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://bk.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ze.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gk.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sa.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jb.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qz.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wd.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vk.9csxet.cn

[L06] 解析响应为 JSON
来源：http://nv.asd995.cn

Py:   resp.json()
来源：http://ef.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://pc.bjjhwx.cn

JS:   await resp.json()
来源：http://lo.yuntaijiaju.cn

TS:   await resp.json()
来源：http://pk.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wh.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ba.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://wl.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xb.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ru.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dg.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vh.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://qy.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://rn.521024.cn

Java: resp.statusCode()
来源：http://fp.szxytkj.cn

Go:   resp.StatusCode
来源：http://qi.hnjuh.cn

Ruby: resp.code.to_i
来源：http://mp.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://bc.shxzskj.cn

[L08] 并发请求多个地址
来源：http://um.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oa.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://yd.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dn.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jx.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kl.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dv.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wh.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cv.huixiangedu.cn

================================================================================
来源：http://ym.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://he.shxzukj.cn

================================================================================
来源：http://eu.shxzukj.cn

[M01] 读取命令行参数
来源：http://nx.lnxyls.cn

Py:   sys.argv[1:]
来源：http://ml.newstarts.cn

PHP:  $argv;  $argc;
来源：http://yq.newstarts.cn

JS:   process.argv.slice(2)
来源：http://zj.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ns.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://dk.nszjky.cn

Go:   os.Args[1:]
来源：http://ks.huixiangedu.cn

Ruby: ARGV
来源：http://db.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://wy.bookmarksfly.cn

[M02] 读取环境变量
来源：http://im.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://js.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ur.szxytkj.cn

JS:   process.env.HOME
来源：http://bf.huixiangedu.cn

TS:   process.env.HOME
来源：http://ar.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://eh.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nr.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://it.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ip.yuexingan06.cn

[M03] 执行外部命令
来源：http://fh.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://si.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hl.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jq.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://py.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kf.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://go.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pc.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://qm.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://ss.hahajie.cn

Py:   os.getcwd()
来源：http://qs.colortex.cn

PHP:  getcwd();
来源：http://gk.huixiangedu.cn

JS:   process.cwd()
来源：http://hn.nszjky.cn

TS:   process.cwd()
来源：http://jb.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://nf.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://if.9csxet.cn

Ruby: Dir.pwd
来源：http://wd.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cj.nicolike.cn

[M05] 设置退出码
来源：http://ky.wgjwhj.cn

Py:   sys.exit(1)
来源：http://vu.bjjhwx.cn

PHP:  exit(1);
来源：http://qj.yuexingan06.cn

JS:   process.exit(1)
来源：http://ik.shxzukj.cn

TS:   process.exit(1)
来源：http://sl.huanxung.cn

Java: System.exit(1)
来源：http://il.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://om.chemitech.net.cn

Ruby: exit 1
来源：http://mi.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://si.chemitech.net.cn

[M06] 向标准错误输出
来源：http://ny.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://nr.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gb.hahajie.cn

JS:   console.error("err")
来源：http://dq.asd995.cn

TS:   console.error("err")
来源：http://nb.newstarts.cn

Java: System.err.println("err")
来源：http://vj.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yi.jctech888.com.cn

Ruby: warn "err"
来源：http://yd.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://jx.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://gi.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://vf.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wb.haigaiapp.cn

JS:   require.main === module
来源：http://jw.yuexingan06.cn

TS:   require.main === module
来源：http://ym.hahajie.cn

Java: public static void main(String[] args)
来源：http://pa.colortex.cn

Go:   func main()
来源：http://cj.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nq.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://pg.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://jh.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://st.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://je.nszjky.cn

JS:   process.platform;  process.version
来源：http://hq.szxytkj.cn

TS:   process.platform;  process.version
来源：http://ty.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uw.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ja.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://or.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fg.huixinmuqiang.cn

================================================================================
来源：http://yj.hahajie.cn

N. 数据结构与算法
来源：http://jd.9csxet.cn

================================================================================
来源：http://oo.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://dx.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fm.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ct.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zo.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://je.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hs.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://eu.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kp.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ob.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://yy.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ci.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fs.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pl.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wr.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bf.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://nk.yuexingan06.cn

Ruby: arr.sort
来源：http://gx.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lw.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ty.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://us.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://lo.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uq.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ix.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aa.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ax.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eh.szxytkj.cn

[N04] 斐波那契数列
来源：http://kx.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lo.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hl.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fk.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vn.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bv.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ib.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uj.521024.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vb.huanxung.cn

[N05] 最大公约数
来源：http://mc.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://lb.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nn.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://td.huixiangedu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fw.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vz.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tf.hahajie.cn

Ruby: a.gcd(b)
来源：http://ve.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ex.chemitech.net.cn

[N06] 判断回文字符串
来源：http://ll.shtwfgs.cn

Py:   s == s[::-1]
来源：http://ok.asd995.cn

PHP:  $s === strrev($s);
来源：http://tn.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://ov.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://bq.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vn.szsharing.cn

Go:   // 双指针从两端比较
来源：http://gg.yuexingan06.cn

Ruby: s == s.reverse
来源：http://td.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yw.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://ab.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dv.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fw.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fm.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://ux.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://rf.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://lz.gzmigu.cn

Ruby: // 手写 Hash
来源：http://fw.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ig.9csxet.cn

[N08] 生成全排列
来源：http://yg.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://qd.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://lg.colortex.cn

JS:   // 手写回溯递归
来源：http://zp.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://um.521024.cn

Java: // 手写回溯递归
来源：http://tw.shxzskj.cn

Go:   // 手写回溯递归
来源：http://hz.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://ws.nszjky.cn

C#:   // 手写回溯递归
来源：http://cw.hnjuh.cn

[N09] 栈与队列
来源：http://gb.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ts.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dz.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://er.haigaiapp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cc.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ht.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gq.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fr.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ji.bjjhwx.cn

[N10] 链表节点定义
来源：http://lh.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pg.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zx.shxzskj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bv.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cp.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://xv.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pc.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fd.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fd.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ue.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bd.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://dm.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://om.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ne.muxihuayi.cn

Java: // 手写递归
来源：http://gg.shxzukj.cn

Go:   // 手写递归
来源：http://fu.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vo.jianghongdianzi.cn

C#:   // 手写递归
来源：http://nh.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gj.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lc.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bl.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://it.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tu.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://as.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sv.newstarts.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fa.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ix.bookmarksfly.cn

================================================================================
来源：http://xo.nszjky.cn

O. 并发与异步
来源：http://tl.shxzskj.cn

================================================================================
来源：http://by.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://nv.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vl.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ds.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yy.szsharing.cn

TS:   // 同 JS
来源：http://si.521024.cn

Java: new Thread(() -> f()).start()
来源：http://bx.wgjwhj.cn

Go:   go f()
来源：http://uz.huanxung.cn

Ruby: Thread.new { f }
来源：http://dv.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://cq.szsharing.cn

[O02] 使用线程池
来源：http://lb.haigaiapp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gt.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ds.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://cc.nicolike.cn

TS:   // worker_threads 线程池
来源：http://km.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hz.panjiajie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yo.521024.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dc.shtwfgs.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qu.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://oh.asd995.cn

Py:   with lock: shared += 1
来源：http://zf.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://sg.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bm.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ce.shxzukj.cn

Java: synchronized (this) { shared++; }
来源：http://ol.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jz.lnxyls.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://db.bookmarksfly.cn

C#:   lock (gate) { shared++; }
来源：http://lr.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://zf.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ds.bjjhwx.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zd.huixinmuqiang.cn

JS:   async function f() { await g(); }
来源：http://iv.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zj.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ty.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bd.wgjwhj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ik.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://qb.panjiajie.cn

[O05] 并发执行并等待全部完成
来源：http://sg.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://pj.colortex.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qa.colortex.cn

JS:   await Promise.all(tasks)
来源：http://rc.huixiangedu.cn

TS:   await Promise.all(tasks)
来源：http://ov.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kr.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dp.521024.cn

Ruby: threads.map(&:join)
来源：http://uq.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oo.colortex.cn

[O06] 使用进程池
来源：http://na.hahajie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nw.hahajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vw.hahajie.cn

JS:   // child_process / cluster 模块
来源：http://qv.szxytkj.cn

TS:   // child_process / cluster 模块
来源：http://ta.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sc.huanxung.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bu.jctech888.com.cn

Ruby: // fork 块
来源：http://zz.521024.cn

C#:   Parallel.For
来源：http://tn.nszjky.cn

================================================================================
来源：http://fa.nszjky.cn

P. 常用工具函数
来源：http://cm.muxihuayi.cn

================================================================================
来源：http://sm.haigaiapp.cn

[P01] 生成 UUID
来源：http://ac.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://hh.bjjhwx.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fz.colortex.cn

JS:   crypto.randomUUID()
来源：http://dc.bjjhwx.cn


<!-- 参考信息 -->