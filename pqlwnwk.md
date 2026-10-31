代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ie.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://as.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wg.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ua.lnxyls.cn

[L03] 设置自定义请求头
来源：http://fs.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nf.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nr.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xk.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zl.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oy.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jq.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hy.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wu.colortex.cn

[L04] 设置超时
来源：http://hj.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://yv.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yi.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zn.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hc.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lr.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dm.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ra.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://ww.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yi.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vk.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hr.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ua.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hg.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ao.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://an.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zy.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://ph.yuexingan06.cn

Py:   resp.json()
来源：http://cb.colortex.cn

PHP:  json_decode($body, true);
来源：http://td.bjjhwx.cn

JS:   await resp.json()
来源：http://mc.gzmigu.cn

TS:   await resp.json()
来源：http://on.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hq.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gw.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://fr.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ih.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://nx.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pn.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hs.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://dh.asd995.cn

TS:   resp.ok;  resp.status
来源：http://ie.huixiangedu.cn

Java: resp.statusCode()
来源：http://rv.nszjky.cn

Go:   resp.StatusCode
来源：http://fl.colortex.cn

Ruby: resp.code.to_i
来源：http://lk.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://fh.gzmigu.cn

[L08] 并发请求多个地址
来源：http://cf.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://na.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ne.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kk.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ea.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://si.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vn.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ci.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gg.hnjuh.cn

================================================================================
来源：http://cn.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://dz.huanxung.cn

================================================================================
来源：http://xv.shtwfgs.cn

[M01] 读取命令行参数
来源：http://uc.huanxung.cn

Py:   sys.argv[1:]
来源：http://uc.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://wm.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://zj.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://qe.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://vb.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://mo.huanxung.cn

Ruby: ARGV
来源：http://we.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://lr.huixinmuqiang.cn

[M02] 读取环境变量
来源：http://et.asd995.cn

Py:   os.environ.get("HOME")
来源：http://bb.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pf.szxytkj.cn

JS:   process.env.HOME
来源：http://wp.szsharing.cn

TS:   process.env.HOME
来源：http://ky.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://cv.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kd.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://vo.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sv.huixiangedu.cn

[M03] 执行外部命令
来源：http://ix.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jf.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pp.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pp.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nt.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cf.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oa.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://dm.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://rh.gzmigu.cn

Py:   os.getcwd()
来源：http://rl.newstarts.cn

PHP:  getcwd();
来源：http://kg.hahajie.cn

JS:   process.cwd()
来源：http://lo.panjiajie.cn

TS:   process.cwd()
来源：http://sm.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://eg.huanxung.cn

Go:   os.Getwd()
来源：http://dp.9csxet.cn

Ruby: Dir.pwd
来源：http://wn.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jd.shxzukj.cn

[M05] 设置退出码
来源：http://kw.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ja.huixiangedu.cn

PHP:  exit(1);
来源：http://ie.asd995.cn

JS:   process.exit(1)
来源：http://pi.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://pt.lnxyls.cn

Java: System.exit(1)
来源：http://ab.nszjky.cn

Go:   os.Exit(1)
来源：http://gk.chemitech.net.cn

Ruby: exit 1
来源：http://as.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pj.haigaiapp.cn

[M06] 向标准错误输出
来源：http://mb.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://ye.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gx.haigaiapp.cn

JS:   console.error("err")
来源：http://km.huixinmuqiang.cn

TS:   console.error("err")
来源：http://ze.shxzukj.cn

Java: System.err.println("err")
来源：http://ql.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vm.panjiajie.cn

Ruby: warn "err"
来源：http://mz.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ir.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://di.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://kd.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dj.lnxyls.cn

JS:   require.main === module
来源：http://bs.wgjwhj.cn

TS:   require.main === module
来源：http://pz.newstarts.cn

Java: public static void main(String[] args)
来源：http://fk.hahajie.cn

Go:   func main()
来源：http://am.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nq.newstarts.cn

C#:   static void Main(string[] args)
来源：http://um.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://gc.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://rr.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://ft.gzmigu.cn

JS:   process.platform;  process.version
来源：http://oz.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://np.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yk.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xo.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nc.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gk.huixinmuqiang.cn

================================================================================
来源：http://hb.wgjwhj.cn

N. 数据结构与算法
来源：http://hl.bookmarksfly.cn

================================================================================
来源：http://wn.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://rf.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://io.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ac.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bi.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fy.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://bt.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://be.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ay.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://dw.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://oz.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ya.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ph.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dm.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ud.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://ng.haigaiapp.cn

Ruby: arr.sort
来源：http://yo.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gj.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://qy.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qo.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://ao.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qd.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ba.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xa.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dq.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pr.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jo.shtwfgs.cn

[N04] 斐波那契数列
来源：http://hk.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ln.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oh.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ic.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jq.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ef.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gg.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wq.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://px.chemitech.net.cn

[N05] 最大公约数
来源：http://el.newstarts.cn

Py:   math.gcd(a, b)
来源：http://ct.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xx.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aj.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pg.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qi.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ly.szsharing.cn

Ruby: a.gcd(b)
来源：http://wd.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iw.bjjhwx.cn

[N06] 判断回文字符串
来源：http://aa.muxihuayi.cn

Py:   s == s[::-1]
来源：http://ow.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://wb.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://qn.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://qw.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zr.szsharing.cn

Go:   // 双指针从两端比较
来源：http://gq.chemitech.net.cn

Ruby: s == s.reverse
来源：http://vs.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://li.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://zb.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tv.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fn.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://av.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://bc.muxihuayi.cn

Java: // 手写 HashMap
来源：http://hu.colortex.cn

Go:   // 手写 map[int]int
来源：http://bx.huanxung.cn

Ruby: // 手写 Hash
来源：http://qz.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://oz.nicolike.cn

[N08] 生成全排列
来源：http://fv.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://dh.shxzskj.cn

PHP:  // 手写递归交换
来源：http://wb.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://ez.panjiajie.cn

TS:   // 手写回溯递归
来源：http://kc.lnxyls.cn

Java: // 手写回溯递归
来源：http://iw.szxytkj.cn

Go:   // 手写回溯递归
来源：http://jt.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://ub.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ep.bookmarksfly.cn

[N09] 栈与队列
来源：http://me.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xr.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vs.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wi.asd995.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hh.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zk.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ba.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ca.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fs.chemitech.net.cn

[N10] 链表节点定义
来源：http://of.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pa.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cy.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ns.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cy.colortex.cn

Java: class Node { int v; Node next; }
来源：http://vd.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uf.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ue.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hv.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://fp.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rp.jctech888.com.cn

PHP:  // 手写递归函数
来源：http://jw.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://la.9csxet.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qh.newstarts.cn

Java: // 手写递归
来源：http://xk.hahajie.cn

Go:   // 手写递归
来源：http://wo.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uk.shtwfgs.cn

C#:   // 手写递归
来源：http://kf.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bx.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nh.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://th.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zj.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tt.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tx.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kq.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ro.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ie.hnjuh.cn

================================================================================
来源：http://xk.yuntaijiaju.cn

O. 并发与异步
来源：http://ng.shxzskj.cn

================================================================================
来源：http://el.521024.cn

[O01] 启动一个线程
来源：http://bi.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xn.nicolike.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ai.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jl.9csxet.cn

TS:   // 同 JS
来源：http://qb.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://pr.huixiangedu.cn

Go:   go f()
来源：http://ve.newstarts.cn

Ruby: Thread.new { f }
来源：http://nw.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ic.bjjhwx.cn

[O02] 使用线程池
来源：http://el.huanxung.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vb.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dt.yuexingan06.cn

JS:   // worker_threads 线程池
来源：http://ti.bookmarksfly.cn

TS:   // worker_threads 线程池
来源：http://nn.lnxyls.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yw.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ub.bjjhwx.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qc.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eq.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://iv.shxzukj.cn

Py:   with lock: shared += 1
来源：http://ze.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://vo.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hs.huixinmuqiang.cn

TS:   // 同 JS
来源：http://hc.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://sj.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kx.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://db.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://lk.muxihuayi.cn

[O04] 定义异步函数并等待
来源：http://ke.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://wc.panjiajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zd.panjiajie.cn

JS:   async function f() { await g(); }
来源：http://ft.asd995.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ln.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ol.haigaiapp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://en.asd995.cn

C#:   async Task F() { await G(); }
来源：http://da.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://th.bjjhwx.cn

Py:   asyncio.gather(*tasks)
来源：http://sf.szsharing.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ok.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://rl.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://rz.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ng.gzmigu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kq.521024.cn

Ruby: threads.map(&:join)
来源：http://py.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ng.521024.cn

[O06] 使用进程池
来源：http://ik.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ax.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rs.szxytkj.cn

JS:   // child_process / cluster 模块
来源：http://xe.wgjwhj.cn

TS:   // child_process / cluster 模块
来源：http://sc.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ay.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://um.hahajie.cn

Ruby: // fork 块
来源：http://wd.wgjwhj.cn


<!-- 参考信息 -->