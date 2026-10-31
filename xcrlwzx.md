代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://eo.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dl.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ff.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bi.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kf.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qj.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gz.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://mm.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tc.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ax.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fd.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://or.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ql.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vy.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tg.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ge.panjiajie.cn

[L04] 设置超时
来源：http://dq.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://ug.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ko.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://is.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pm.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dz.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cr.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qw.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kc.hahajie.cn

[L05] 上传文件（multipart）
来源：http://uv.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gg.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ak.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oy.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sw.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bc.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cr.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://et.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zj.huanxung.cn

[L06] 解析响应为 JSON
来源：http://px.asd995.cn

Py:   resp.json()
来源：http://ei.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://pi.shtwfgs.cn

JS:   await resp.json()
来源：http://ui.nicolike.cn

TS:   await resp.json()
来源：http://od.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ko.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ft.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://wl.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kc.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://tc.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://by.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fc.521024.cn

JS:   resp.ok;  resp.status
来源：http://zp.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://sj.wgjwhj.cn

Java: resp.statusCode()
来源：http://ov.szxytkj.cn

Go:   resp.StatusCode
来源：http://we.shxzskj.cn

Ruby: resp.code.to_i
来源：http://tk.lnxyls.cn

C#:   (int)resp.StatusCode
来源：http://yb.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://cd.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://is.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://zq.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yu.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bt.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lq.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hk.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lk.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rj.hahajie.cn

================================================================================
来源：http://wa.muxihuayi.cn

M. 命令行 / 进程 / 环境
来源：http://mn.nszjky.cn

================================================================================
来源：http://uj.yuexingan06.cn

[M01] 读取命令行参数
来源：http://ka.shxzskj.cn

Py:   sys.argv[1:]
来源：http://mh.9csxet.cn

PHP:  $argv;  $argc;
来源：http://kb.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://nn.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ht.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://sf.9csxet.cn

Go:   os.Args[1:]
来源：http://yq.shxzskj.cn

Ruby: ARGV
来源：http://dh.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://xb.hnjuh.cn

[M02] 读取环境变量
来源：http://ef.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://mp.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wz.chemitech.net.cn

JS:   process.env.HOME
来源：http://rb.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://eq.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://aj.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ef.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://in.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://is.wgjwhj.cn

[M03] 执行外部命令
来源：http://ma.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bq.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bs.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zl.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cr.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dz.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wj.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jh.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://ck.huanxung.cn

[M04] 获取当前工作目录
来源：http://fy.lnxyls.cn

Py:   os.getcwd()
来源：http://gl.shxzukj.cn

PHP:  getcwd();
来源：http://fo.bjjhwx.cn

JS:   process.cwd()
来源：http://nu.gzmigu.cn

TS:   process.cwd()
来源：http://pq.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://dd.muxihuayi.cn

Go:   os.Getwd()
来源：http://gk.muxihuayi.cn

Ruby: Dir.pwd
来源：http://kd.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eb.hahajie.cn

[M05] 设置退出码
来源：http://ot.szxytkj.cn

Py:   sys.exit(1)
来源：http://xv.lnxyls.cn

PHP:  exit(1);
来源：http://xq.huanxung.cn

JS:   process.exit(1)
来源：http://cc.szsharing.cn

TS:   process.exit(1)
来源：http://yj.chemitech.net.cn

Java: System.exit(1)
来源：http://oi.hahajie.cn

Go:   os.Exit(1)
来源：http://no.newstarts.cn

Ruby: exit 1
来源：http://or.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wj.panjiajie.cn

[M06] 向标准错误输出
来源：http://zv.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://ju.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ga.haigaiapp.cn

JS:   console.error("err")
来源：http://qx.bjjhwx.cn

TS:   console.error("err")
来源：http://nx.shxzukj.cn

Java: System.err.println("err")
来源：http://iw.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dy.shxzukj.cn

Ruby: warn "err"
来源：http://pv.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://xx.nszjky.cn

[M07] 判断是否为主入口
来源：http://zi.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://xo.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wo.jctech888.com.cn

JS:   require.main === module
来源：http://sp.newstarts.cn

TS:   require.main === module
来源：http://xd.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://iq.newstarts.cn

Go:   func main()
来源：http://ii.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vn.colortex.cn

C#:   static void Main(string[] args)
来源：http://jc.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://gb.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://iz.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://zf.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://gb.shxzukj.cn

TS:   process.platform;  process.version
来源：http://cl.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vl.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://er.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cn.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fs.szxytkj.cn

================================================================================
来源：http://yq.hahajie.cn

N. 数据结构与算法
来源：http://hg.hahajie.cn

================================================================================
来源：http://jv.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://nz.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://um.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yh.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vq.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://si.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xu.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://pb.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nt.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://fo.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://zo.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kr.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zp.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hl.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yc.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://yr.jctech888.com.cn

Ruby: arr.sort
来源：http://br.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bv.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://qq.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gz.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://mx.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vp.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vk.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iq.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ap.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hn.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fs.muxihuayi.cn

[N04] 斐波那契数列
来源：http://hr.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qq.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zx.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sj.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pc.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iv.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qk.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fl.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nj.lnxyls.cn

[N05] 最大公约数
来源：http://fv.asd995.cn

Py:   math.gcd(a, b)
来源：http://ld.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uj.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fz.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ev.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sk.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://wi.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ao.chemitech.net.cn

[N06] 判断回文字符串
来源：http://xi.panjiajie.cn

Py:   s == s[::-1]
来源：http://bh.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://pu.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://xl.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://cw.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xq.szsharing.cn

Go:   // 双指针从两端比较
来源：http://iw.9csxet.cn

Ruby: s == s.reverse
来源：http://xp.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wb.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://js.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gd.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wr.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hg.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://gh.shtwfgs.cn

Java: // 手写 HashMap
来源：http://yo.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://qw.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://va.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ou.hahajie.cn

[N08] 生成全排列
来源：http://kv.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://os.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://qc.newstarts.cn

JS:   // 手写回溯递归
来源：http://mc.gzmigu.cn

TS:   // 手写回溯递归
来源：http://wu.yuexingan06.cn

Java: // 手写回溯递归
来源：http://zv.shxzukj.cn

Go:   // 手写回溯递归
来源：http://yz.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://st.hahajie.cn

C#:   // 手写回溯递归
来源：http://kd.nicolike.cn

[N09] 栈与队列
来源：http://vy.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ky.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ym.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ut.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tv.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://df.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wc.521024.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kv.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lw.huanxung.cn

[N10] 链表节点定义
来源：http://dy.shtwfgs.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iy.asd995.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rn.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qe.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vf.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://ad.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lm.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ft.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gp.nszjky.cn

[N11] 二叉树中序遍历
来源：http://hs.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yh.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://hl.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dz.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kp.yuntaijiaju.cn

Java: // 手写递归
来源：http://kp.szsharing.cn

Go:   // 手写递归
来源：http://wl.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rj.jianghongdianzi.cn

C#:   // 手写递归
来源：http://nb.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wz.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://am.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zs.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fi.nicolike.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pf.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ii.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mf.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://us.szxytkj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hm.jianghongdianzi.cn

================================================================================
来源：http://sp.szsharing.cn

O. 并发与异步
来源：http://pm.jctech888.com.cn

================================================================================
来源：http://zv.yuexingan06.cn

[O01] 启动一个线程
来源：http://ih.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rb.haigaiapp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wv.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oc.szsharing.cn

TS:   // 同 JS
来源：http://mt.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://fv.nszjky.cn

Go:   go f()
来源：http://hi.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://rj.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://tv.yuexingan06.cn

[O02] 使用线程池
来源：http://of.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hi.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://py.nszjky.cn

JS:   // worker_threads 线程池
来源：http://lm.hahajie.cn

TS:   // worker_threads 线程池
来源：http://hp.chemitech.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kd.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fm.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iu.bookmarksfly.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lv.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://om.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://rb.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ma.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jq.huixiangedu.cn

TS:   // 同 JS
来源：http://zl.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://rt.chemitech.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pn.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://px.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://bw.asd995.cn

[O04] 定义异步函数并等待
来源：http://cw.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://ge.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yn.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://to.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vr.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eb.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wt.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rt.nicolike.cn

C#:   async Task F() { await G(); }
来源：http://mx.colortex.cn

[O05] 并发执行并等待全部完成
来源：http://gg.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://jx.huixiangedu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qu.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://kx.jianghongdianzi.cn

TS:   await Promise.all(tasks)
来源：http://ud.newstarts.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dw.huixiangedu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qx.jctech888.com.cn

Ruby: threads.map(&:join)
来源：http://xw.muxihuayi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sm.hnjuh.cn

[O06] 使用进程池
来源：http://xl.9csxet.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hj.wgjwhj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eg.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://pz.hnjuh.cn


<!-- 参考信息 -->