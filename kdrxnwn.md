代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cq.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ar.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yu.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ah.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://le.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nl.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ax.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bx.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ly.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fd.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ys.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://os.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://om.muxihuayi.cn

[L04] 设置超时
来源：http://gf.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ug.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://id.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ll.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xu.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pr.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sv.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yq.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://em.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://ap.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wb.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ra.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://az.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nl.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sv.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ur.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://is.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nq.9csxet.cn

[L06] 解析响应为 JSON
来源：http://st.asd995.cn

Py:   resp.json()
来源：http://wn.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://xk.muxihuayi.cn

JS:   await resp.json()
来源：http://os.huixinmuqiang.cn

TS:   await resp.json()
来源：http://nh.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jh.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tf.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://xz.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ka.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://lo.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wx.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://to.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://kp.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ap.newstarts.cn

Java: resp.statusCode()
来源：http://wr.colortex.cn

Go:   resp.StatusCode
来源：http://bs.huanxung.cn

Ruby: resp.code.to_i
来源：http://by.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://sj.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://va.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dj.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://yl.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hr.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ov.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pd.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zv.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ye.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://su.asd995.cn

================================================================================
来源：http://af.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://eh.szxytkj.cn

================================================================================
来源：http://fu.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://cu.colortex.cn

Py:   sys.argv[1:]
来源：http://yf.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://kd.newstarts.cn

JS:   process.argv.slice(2)
来源：http://pc.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://qm.521024.cn

Java: args 数组（main 方法参数）
来源：http://ex.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://oj.panjiajie.cn

Ruby: ARGV
来源：http://ez.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://rh.huixiangedu.cn

[M02] 读取环境变量
来源：http://kq.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://mj.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zz.shxzukj.cn

JS:   process.env.HOME
来源：http://vn.wgjwhj.cn

TS:   process.env.HOME
来源：http://dq.huanxung.cn

Java: System.getenv("HOME")
来源：http://va.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vr.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://qp.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kg.haigaiapp.cn

[M03] 执行外部命令
来源：http://xa.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vt.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kr.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lz.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sk.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ek.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ig.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lv.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://lp.panjiajie.cn

[M04] 获取当前工作目录
来源：http://js.haigaiapp.cn

Py:   os.getcwd()
来源：http://md.muxihuayi.cn

PHP:  getcwd();
来源：http://ja.huixiangedu.cn

JS:   process.cwd()
来源：http://sd.szsharing.cn

TS:   process.cwd()
来源：http://pm.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://dz.bjjhwx.cn

Go:   os.Getwd()
来源：http://eh.gzmigu.cn

Ruby: Dir.pwd
来源：http://yz.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wq.lnxyls.cn

[M05] 设置退出码
来源：http://rh.asd995.cn

Py:   sys.exit(1)
来源：http://wa.9csxet.cn

PHP:  exit(1);
来源：http://gg.bjjhwx.cn

JS:   process.exit(1)
来源：http://ze.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://pq.hahajie.cn

Java: System.exit(1)
来源：http://cx.nszjky.cn

Go:   os.Exit(1)
来源：http://na.huanxung.cn

Ruby: exit 1
来源：http://ax.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kz.shtwfgs.cn

[M06] 向标准错误输出
来源：http://kc.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ap.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mh.wgjwhj.cn

JS:   console.error("err")
来源：http://ah.wgjwhj.cn

TS:   console.error("err")
来源：http://xb.shxzskj.cn

Java: System.err.println("err")
来源：http://as.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xv.asd995.cn

Ruby: warn "err"
来源：http://tc.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://df.lnxyls.cn

[M07] 判断是否为主入口
来源：http://oi.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://zq.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ab.nicolike.cn

JS:   require.main === module
来源：http://vl.newstarts.cn

TS:   require.main === module
来源：http://ha.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://eu.chemitech.net.cn

Go:   func main()
来源：http://ez.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kb.newstarts.cn

C#:   static void Main(string[] args)
来源：http://bs.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://jd.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://kh.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://es.hahajie.cn

JS:   process.platform;  process.version
来源：http://lr.nicolike.cn

TS:   process.platform;  process.version
来源：http://lq.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lq.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mn.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yv.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://no.bookmarksfly.cn

================================================================================
来源：http://iu.nicolike.cn

N. 数据结构与算法
来源：http://ov.gzmigu.cn

================================================================================
来源：http://sc.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://fv.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sg.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uc.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ii.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rz.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ou.muxihuayi.cn

Go:   sort.SearchInts(arr, x)
来源：http://hw.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://be.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cw.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://kx.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iy.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zc.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bq.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iy.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://sz.muxihuayi.cn

Ruby: arr.sort
来源：http://aj.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gq.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://jw.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aw.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://qj.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kq.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ji.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://um.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yy.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://io.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ka.shxzukj.cn

[N04] 斐波那契数列
来源：http://yf.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qs.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ek.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nk.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bz.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dl.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ns.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ct.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jm.yuexingan06.cn

[N05] 最大公约数
来源：http://yq.nszjky.cn

Py:   math.gcd(a, b)
来源：http://zw.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sk.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ze.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ex.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hh.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://px.nicolike.cn

Ruby: a.gcd(b)
来源：http://jl.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hb.jctech888.com.cn

[N06] 判断回文字符串
来源：http://fm.szsharing.cn

Py:   s == s[::-1]
来源：http://dy.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://mx.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://pb.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://yt.jianghongdianzi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ch.huanxung.cn

Go:   // 双指针从两端比较
来源：http://fw.hahajie.cn

Ruby: s == s.reverse
来源：http://ys.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hk.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://gt.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ir.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oh.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xq.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://me.shxzskj.cn

Java: // 手写 HashMap
来源：http://zf.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://ba.colortex.cn

Ruby: // 手写 Hash
来源：http://tj.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ju.chemitech.net.cn

[N08] 生成全排列
来源：http://ba.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://fq.colortex.cn

PHP:  // 手写递归交换
来源：http://rg.nszjky.cn

JS:   // 手写回溯递归
来源：http://xd.asd995.cn

TS:   // 手写回溯递归
来源：http://li.muxihuayi.cn

Java: // 手写回溯递归
来源：http://fi.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://wb.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ff.9csxet.cn

C#:   // 手写回溯递归
来源：http://vs.huanxung.cn

[N09] 栈与队列
来源：http://uj.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rq.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xl.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eh.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://at.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://js.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uo.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sh.wgjwhj.cn

[N10] 链表节点定义
来源：http://vk.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qp.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xj.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fr.huixiangedu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ww.chemitech.net.cn

Java: class Node { int v; Node next; }
来源：http://lj.521024.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wg.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uv.szxytkj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pp.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://vh.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xb.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://gw.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zm.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sb.gzmigu.cn

Java: // 手写递归
来源：http://kv.shxzskj.cn

Go:   // 手写递归
来源：http://tp.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fk.shxzskj.cn

C#:   // 手写递归
来源：http://hv.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dj.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pj.bjjhwx.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gd.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xo.nszjky.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rv.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hl.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zq.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gv.huixiangedu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pf.bookmarksfly.cn

================================================================================
来源：http://gq.szxytkj.cn

O. 并发与异步
来源：http://jw.yuntaijiaju.cn

================================================================================
来源：http://fx.jctech888.com.cn

[O01] 启动一个线程
来源：http://hn.szsharing.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://su.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tp.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://be.hahajie.cn

TS:   // 同 JS
来源：http://oo.wgjwhj.cn

Java: new Thread(() -> f()).start()
来源：http://tn.bjjhwx.cn

Go:   go f()
来源：http://xf.nicolike.cn

Ruby: Thread.new { f }
来源：http://gg.9csxet.cn

C#:   Task.Run(() => F());
来源：http://ke.521024.cn

[O02] 使用线程池
来源：http://at.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ri.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kd.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://hc.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://is.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ms.lnxyls.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ki.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zb.shxzskj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wc.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://vx.hahajie.cn

Py:   with lock: shared += 1
来源：http://xc.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://ck.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cm.wgjwhj.cn

TS:   // 同 JS
来源：http://le.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://yu.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zq.bjjhwx.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wl.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://it.yuexingan06.cn

[O04] 定义异步函数并等待
来源：http://cu.lnxyls.cn

Py:   async def f():⏎    await g()
来源：http://ds.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xe.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://yu.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ka.shxzukj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jf.hahajie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lp.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bg.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://ik.lnxyls.cn

[O05] 并发执行并等待全部完成
来源：http://kr.521024.cn

Py:   asyncio.gather(*tasks)
来源：http://vp.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ar.lnxyls.cn

JS:   await Promise.all(tasks)
来源：http://zh.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://lm.bjjhwx.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qc.lnxyls.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lq.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://uf.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bj.521024.cn

[O06] 使用进程池
来源：http://ie.lnxyls.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oe.szsharing.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sp.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://yg.yuexingan06.cn

TS:   // child_process / cluster 模块
来源：http://db.wgjwhj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tm.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ha.shxzukj.cn

Ruby: // fork 块
来源：http://ai.lnxyls.cn


<!-- 参考信息 -->