代发 wailian999

Go:   encoding/gob
来源：http://dk.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://uk.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jk.hnjuh.cn

================================================================================
来源：http://st.haigaiapp.cn

L. 网络请求
来源：http://df.shxzskj.cn

================================================================================
来源：http://ls.szxytkj.cn

[L01] 发送 GET 请求
来源：http://uj.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jk.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yd.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://hm.newstarts.cn

TS:   await fetch(url)
来源：http://ud.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jo.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://lk.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ar.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wb.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ml.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://co.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cp.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fd.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ru.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lj.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ah.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fu.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://by.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://cj.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vz.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ou.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hv.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sa.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tg.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://et.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kv.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cf.colortex.cn

[L04] 设置超时
来源：http://nd.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://qa.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://re.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eh.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vz.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cb.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cp.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gr.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yu.9csxet.cn

[L05] 上传文件（multipart）
来源：http://gy.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uc.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mb.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rw.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ft.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jn.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cx.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://od.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dl.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://ux.bjjhwx.cn

Py:   resp.json()
来源：http://wb.asd995.cn

PHP:  json_decode($body, true);
来源：http://za.yuntaijiaju.cn

JS:   await resp.json()
来源：http://vf.bjjhwx.cn

TS:   await resp.json()
来源：http://zl.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://en.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ju.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://tf.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zq.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://nt.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hn.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ol.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://jo.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://vi.nicolike.cn

Java: resp.statusCode()
来源：http://ds.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://lh.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://ik.521024.cn

C#:   (int)resp.StatusCode
来源：http://cm.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ho.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ir.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ro.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tp.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zk.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bk.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mu.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vg.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yk.521024.cn

================================================================================
来源：http://yo.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://uo.szxytkj.cn

================================================================================
来源：http://hh.szsharing.cn

[M01] 读取命令行参数
来源：http://fl.szsharing.cn

Py:   sys.argv[1:]
来源：http://df.colortex.cn

PHP:  $argv;  $argc;
来源：http://xk.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://kl.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://lx.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://wk.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://bo.yuntaijiaju.cn

Ruby: ARGV
来源：http://gj.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://dm.lnxyls.cn

[M02] 读取环境变量
来源：http://nm.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://sc.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vf.hnjuh.cn

JS:   process.env.HOME
来源：http://wm.bookmarksfly.cn

TS:   process.env.HOME
来源：http://ls.colortex.cn

Java: System.getenv("HOME")
来源：http://vu.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://az.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://vn.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yp.521024.cn

[M03] 执行外部命令
来源：http://mv.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gk.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tn.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ea.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wm.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ir.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zb.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yf.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://pe.shxzskj.cn

[M04] 获取当前工作目录
来源：http://bg.huanxung.cn

Py:   os.getcwd()
来源：http://xg.shxzukj.cn

PHP:  getcwd();
来源：http://ew.asd995.cn

JS:   process.cwd()
来源：http://yd.shxzskj.cn

TS:   process.cwd()
来源：http://wg.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ev.hahajie.cn

Go:   os.Getwd()
来源：http://ta.asd995.cn

Ruby: Dir.pwd
来源：http://fu.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ri.colortex.cn

[M05] 设置退出码
来源：http://lw.521024.cn

Py:   sys.exit(1)
来源：http://yy.lnxyls.cn

PHP:  exit(1);
来源：http://yc.haigaiapp.cn

JS:   process.exit(1)
来源：http://ds.521024.cn

TS:   process.exit(1)
来源：http://pb.9csxet.cn

Java: System.exit(1)
来源：http://jm.shtwfgs.cn

Go:   os.Exit(1)
来源：http://to.shxzukj.cn

Ruby: exit 1
来源：http://bq.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qi.szsharing.cn

[M06] 向标准错误输出
来源：http://oh.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://jh.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://od.bjjhwx.cn

JS:   console.error("err")
来源：http://hy.jctech888.com.cn

TS:   console.error("err")
来源：http://li.muxihuayi.cn

Java: System.err.println("err")
来源：http://yh.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pq.haigaiapp.cn

Ruby: warn "err"
来源：http://ei.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://es.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://yq.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://kj.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wi.wgjwhj.cn

JS:   require.main === module
来源：http://of.szsharing.cn

TS:   require.main === module
来源：http://ew.lnxyls.cn

Java: public static void main(String[] args)
来源：http://tt.521024.cn

Go:   func main()
来源：http://xs.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gq.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://zb.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://jw.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://tg.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://yq.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://gj.521024.cn

TS:   process.platform;  process.version
来源：http://md.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://my.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ot.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bz.huixinmuqiang.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cp.yuexingan06.cn

================================================================================
来源：http://lb.newstarts.cn

N. 数据结构与算法
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://ve.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://el.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://um.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://se.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cn.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://do.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://in.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ri.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ht.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qa.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://nc.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://zp.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ar.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sj.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qa.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lc.9csxet.cn

Go:   slices.Sort(arr)
来源：http://hk.muxihuayi.cn

Ruby: arr.sort
来源：http://hf.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qj.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://uh.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bu.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://zv.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tv.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aj.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jk.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cu.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cs.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sh.bjjhwx.cn

[N04] 斐波那契数列
来源：http://tt.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qa.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ub.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ve.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wx.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jo.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tm.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wd.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ab.hnjuh.cn

[N05] 最大公约数
来源：http://sr.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://vv.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qi.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uy.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iu.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fq.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mi.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://lb.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sv.hnjuh.cn

[N06] 判断回文字符串
来源：http://mm.shxzskj.cn

Py:   s == s[::-1]
来源：http://qo.hnjuh.cn

PHP:  $s === strrev($s);
来源：http://mc.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://sd.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://wt.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qg.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://pl.haigaiapp.cn

Ruby: s == s.reverse
来源：http://fg.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://af.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://es.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ok.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ts.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://si.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://me.huixiangedu.cn

Java: // 手写 HashMap
来源：http://ld.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://jq.szxytkj.cn

Ruby: // 手写 Hash
来源：http://vb.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fk.nicolike.cn

[N08] 生成全排列
来源：http://lh.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://ot.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://zh.huanxung.cn

JS:   // 手写回溯递归
来源：http://zi.panjiajie.cn

TS:   // 手写回溯递归
来源：http://yh.bjjhwx.cn

Java: // 手写回溯递归
来源：http://nh.lnxyls.cn

Go:   // 手写回溯递归
来源：http://ss.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ih.shxzukj.cn

C#:   // 手写回溯递归
来源：http://pa.newstarts.cn

[N09] 栈与队列
来源：http://mp.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vj.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wi.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xy.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qn.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qz.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wm.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://it.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lz.huanxung.cn

[N10] 链表节点定义
来源：http://hi.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sp.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qg.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lu.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lv.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://gv.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://an.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mx.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mc.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://xr.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ev.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://gm.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ya.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bq.shxzskj.cn

Java: // 手写递归
来源：http://hd.newstarts.cn

Go:   // 手写递归
来源：http://hd.huanxung.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uy.gzmigu.cn

C#:   // 手写递归
来源：http://rm.huanxung.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://my.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yw.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jg.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mb.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fh.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ct.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uq.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mq.asd995.cn

================================================================================
来源：http://qc.gzmigu.cn

O. 并发与异步
来源：http://wb.colortex.cn

================================================================================
来源：http://ie.bookmarksfly.cn

[O01] 启动一个线程
来源：http://xs.huixinmuqiang.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ds.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://us.hahajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://te.asd995.cn

TS:   // 同 JS
来源：http://yc.newstarts.cn

Java: new Thread(() -> f()).start()
来源：http://lo.jianghongdianzi.cn

Go:   go f()
来源：http://tt.nicolike.cn

Ruby: Thread.new { f }
来源：http://ls.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://ql.panjiajie.cn

[O02] 使用线程池
来源：http://ah.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kk.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ji.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://tn.nszjky.cn

TS:   // worker_threads 线程池
来源：http://cz.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pg.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ik.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jb.hnjuh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eb.wgjwhj.cn

[O03] 加锁保护共享数据
来源：http://qb.szsharing.cn

Py:   with lock: shared += 1
来源：http://cb.panjiajie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ng.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://af.colortex.cn

TS:   // 同 JS
来源：http://lj.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://kq.asd995.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iz.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ua.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://dj.nicolike.cn

[O04] 定义异步函数并等待
来源：http://oq.bookmarksfly.cn

Py:   async def f():⏎    await g()
来源：http://bs.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://io.huixiangedu.cn

JS:   async function f() { await g(); }
来源：http://eu.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mu.szsharing.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gb.chemitech.net.cn


<!-- 参考信息 -->