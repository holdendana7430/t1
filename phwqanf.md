代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://el.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bi.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qn.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sm.gzmigu.cn

[L03] 设置自定义请求头
来源：http://vd.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ao.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sc.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kz.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hk.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gb.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eh.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ht.asd995.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uj.chemitech.net.cn

[L04] 设置超时
来源：http://wn.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://ek.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://et.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ud.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oc.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zz.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ir.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qy.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ab.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://fv.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ew.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sp.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zk.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fr.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ci.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ft.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hh.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vc.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://hg.yuntaijiaju.cn

Py:   resp.json()
来源：http://mr.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://nh.asd995.cn

JS:   await resp.json()
来源：http://ks.521024.cn

TS:   await resp.json()
来源：http://sf.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ex.colortex.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gz.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://jk.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lm.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://lb.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pe.huixiangedu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qw.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://xn.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://aa.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://qb.wgjwhj.cn

Go:   resp.StatusCode
来源：http://bz.szxytkj.cn

Ruby: resp.code.to_i
来源：http://ul.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://mj.hahajie.cn

[L08] 并发请求多个地址
来源：http://kc.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ej.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://ga.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zi.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jq.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vy.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nq.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wh.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ve.9csxet.cn

================================================================================
来源：http://df.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://rl.szxytkj.cn

================================================================================
来源：http://uf.colortex.cn

[M01] 读取命令行参数
来源：http://py.asd995.cn

Py:   sys.argv[1:]
来源：http://wy.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://vj.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ci.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://lu.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://xr.huixiangedu.cn

Go:   os.Args[1:]
来源：http://cg.9csxet.cn

Ruby: ARGV
来源：http://ee.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://gu.gzmigu.cn

[M02] 读取环境变量
来源：http://ee.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://os.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lc.gzmigu.cn

JS:   process.env.HOME
来源：http://sg.shtwfgs.cn

TS:   process.env.HOME
来源：http://ro.lnxyls.cn

Java: System.getenv("HOME")
来源：http://tl.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xc.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://sc.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ln.shtwfgs.cn

[M03] 执行外部命令
来源：http://ov.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wc.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kt.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ke.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bk.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ec.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fb.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fq.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://yu.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://fz.huixiangedu.cn

Py:   os.getcwd()
来源：http://og.bjjhwx.cn

PHP:  getcwd();
来源：http://js.jctech888.com.cn

JS:   process.cwd()
来源：http://sa.colortex.cn

TS:   process.cwd()
来源：http://vv.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://kh.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://sf.9csxet.cn

Ruby: Dir.pwd
来源：http://vm.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pm.jianghongdianzi.cn

[M05] 设置退出码
来源：http://dz.colortex.cn

Py:   sys.exit(1)
来源：http://yr.hnjuh.cn

PHP:  exit(1);
来源：http://zk.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://gk.bookmarksfly.cn

TS:   process.exit(1)
来源：http://dw.panjiajie.cn

Java: System.exit(1)
来源：http://kb.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://xj.panjiajie.cn

Ruby: exit 1
来源：http://ru.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dn.shxzskj.cn

[M06] 向标准错误输出
来源：http://bp.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://zc.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dn.colortex.cn

JS:   console.error("err")
来源：http://er.bookmarksfly.cn

TS:   console.error("err")
来源：http://gg.newstarts.cn

Java: System.err.println("err")
来源：http://qu.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dd.yuntaijiaju.cn

Ruby: warn "err"
来源：http://oo.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://cd.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://gr.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://kf.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ya.panjiajie.cn

JS:   require.main === module
来源：http://fk.hnjuh.cn

TS:   require.main === module
来源：http://pz.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://bu.asd995.cn

Go:   func main()
来源：http://va.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eu.colortex.cn

C#:   static void Main(string[] args)
来源：http://mt.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://mx.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://zr.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://af.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://km.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://fg.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nj.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zj.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ah.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jl.szxytkj.cn

================================================================================
来源：http://jv.huixinmuqiang.cn

N. 数据结构与算法
来源：http://xs.yuntaijiaju.cn

================================================================================
来源：http://cf.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://pd.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ne.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wt.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ok.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nz.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://dq.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hk.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cu.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ql.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://kt.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zs.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gy.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iu.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wf.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://yk.szsharing.cn

Ruby: arr.sort
来源：http://fb.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ee.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://wv.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oa.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://or.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jw.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rd.shtwfgs.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qe.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wo.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rb.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kt.colortex.cn

[N04] 斐波那契数列
来源：http://yo.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eg.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://di.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bb.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xn.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zm.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kx.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wc.panjiajie.cn

[N05] 最大公约数
来源：http://su.asd995.cn

Py:   math.gcd(a, b)
来源：http://ar.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rn.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://me.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://am.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bh.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pq.huanxung.cn

Ruby: a.gcd(b)
来源：http://su.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pm.yuexingan06.cn

[N06] 判断回文字符串
来源：http://gh.yuexingan06.cn

Py:   s == s[::-1]
来源：http://je.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://qv.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://ff.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://bf.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jf.nicolike.cn

Go:   // 双指针从两端比较
来源：http://zq.huanxung.cn

Ruby: s == s.reverse
来源：http://jz.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dn.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://nt.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ax.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sz.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uu.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://os.wgjwhj.cn

Java: // 手写 HashMap
来源：http://rx.szsharing.cn

Go:   // 手写 map[int]int
来源：http://as.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://fz.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ql.szsharing.cn

[N08] 生成全排列
来源：http://xb.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://pi.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://rw.9csxet.cn

JS:   // 手写回溯递归
来源：http://kk.szxytkj.cn

TS:   // 手写回溯递归
来源：http://pc.szsharing.cn

Java: // 手写回溯递归
来源：http://uy.nicolike.cn

Go:   // 手写回溯递归
来源：http://cx.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://bv.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://iw.shxzukj.cn

[N09] 栈与队列
来源：http://qx.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gi.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lz.asd995.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mg.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uf.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nq.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sm.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ik.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fo.szsharing.cn

[N10] 链表节点定义
来源：http://ky.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ec.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dj.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://st.nszjky.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fi.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://ip.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gs.huanxung.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ea.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xt.hahajie.cn

[N11] 二叉树中序遍历
来源：http://vl.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ue.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://iw.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gp.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tx.szsharing.cn

Java: // 手写递归
来源：http://rj.gzmigu.cn

Go:   // 手写递归
来源：http://jg.shtwfgs.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jm.newstarts.cn

C#:   // 手写递归
来源：http://kk.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://po.huixinmuqiang.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cd.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ky.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pq.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yj.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vz.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pa.yuntaijiaju.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pp.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://od.muxihuayi.cn

================================================================================
来源：http://ky.jctech888.com.cn

O. 并发与异步
来源：http://nn.muxihuayi.cn

================================================================================
来源：http://nf.muxihuayi.cn

[O01] 启动一个线程
来源：http://df.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kz.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ct.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ll.gzmigu.cn

TS:   // 同 JS
来源：http://vr.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://cl.chemitech.net.cn

Go:   go f()
来源：http://kz.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://kb.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://yp.colortex.cn

[O02] 使用线程池
来源：http://sf.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qp.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sd.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://mq.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://cu.jianghongdianzi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lv.bookmarksfly.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rs.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rw.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kz.jianghongdianzi.cn

[O03] 加锁保护共享数据
来源：http://ot.nicolike.cn

Py:   with lock: shared += 1
来源：http://eo.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://jf.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://if.szxytkj.cn

TS:   // 同 JS
来源：http://nz.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://cc.bjjhwx.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hv.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uq.jianghongdianzi.cn

C#:   lock (gate) { shared++; }
来源：http://ku.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://cu.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://tx.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iu.huanxung.cn

JS:   async function f() { await g(); }
来源：http://qc.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qz.9csxet.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ck.huixinmuqiang.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fo.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hz.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://qa.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://ry.muxihuayi.cn

Py:   asyncio.gather(*tasks)
来源：http://ay.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cz.asd995.cn

JS:   await Promise.all(tasks)
来源：http://hr.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://vt.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vr.yuexingan06.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pw.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://rl.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ct.hahajie.cn

[O06] 使用进程池
来源：http://ci.wgjwhj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ix.gzmigu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tz.yuexingan06.cn

JS:   // child_process / cluster 模块
来源：http://um.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://oa.jianghongdianzi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jg.lnxyls.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bx.haigaiapp.cn

Ruby: // fork 块
来源：http://eh.panjiajie.cn


<!-- 参考信息 -->