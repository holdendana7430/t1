代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yw.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ga.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://qk.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://rs.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ly.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://cw.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://pm.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ly.nszjky.cn

Go:   encoding/gob
来源：http://ka.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ok.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wl.panjiajie.cn

================================================================================
来源：http://lv.huixinmuqiang.cn

L. 网络请求
来源：http://bd.shxzukj.cn

================================================================================
来源：http://uw.colortex.cn

[L01] 发送 GET 请求
来源：http://um.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xs.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uk.jctech888.com.cn

JS:   await fetch(url)
来源：http://vx.haigaiapp.cn

TS:   await fetch(url)
来源：http://ch.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nl.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://cz.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ef.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qu.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://ey.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vz.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lh.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lb.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sg.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cm.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ct.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sl.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ut.hnjuh.cn

[L03] 设置自定义请求头
来源：http://xu.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bk.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ps.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aq.asd995.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hp.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sa.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yj.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nz.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qy.jctech888.com.cn

[L04] 设置超时
来源：http://oa.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://xc.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ya.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bz.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tz.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cv.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://km.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://np.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ok.newstarts.cn

[L05] 上传文件（multipart）
来源：http://yn.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oi.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qi.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mt.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ri.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aw.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mr.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hd.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ty.521024.cn

[L06] 解析响应为 JSON
来源：http://vq.huanxung.cn

Py:   resp.json()
来源：http://jk.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://jf.gzmigu.cn

JS:   await resp.json()
来源：http://rk.gzmigu.cn

TS:   await resp.json()
来源：http://gd.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qa.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mm.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://ha.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qw.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://lj.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nt.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gg.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://ki.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://ig.521024.cn

Java: resp.statusCode()
来源：http://cs.yuexingan06.cn

Go:   resp.StatusCode
来源：http://so.nicolike.cn

Ruby: resp.code.to_i
来源：http://xb.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://ca.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://oy.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ts.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://zg.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rb.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qa.nicolike.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fo.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bn.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vd.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mo.newstarts.cn

================================================================================
来源：http://ph.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://ug.huixinmuqiang.cn

================================================================================
来源：http://zr.shtwfgs.cn

[M01] 读取命令行参数
来源：http://pp.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://rj.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://um.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://mg.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://mz.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://bh.haigaiapp.cn

Go:   os.Args[1:]
来源：http://qj.colortex.cn

Ruby: ARGV
来源：http://hu.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://xm.asd995.cn

[M02] 读取环境变量
来源：http://ck.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://pj.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ex.szxytkj.cn

JS:   process.env.HOME
来源：http://ok.521024.cn

TS:   process.env.HOME
来源：http://ho.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://kr.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wt.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://kb.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cd.shtwfgs.cn

[M03] 执行外部命令
来源：http://ge.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://st.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gs.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nu.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mp.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zq.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ed.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ie.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://ad.gzmigu.cn

[M04] 获取当前工作目录
来源：http://bj.shxzukj.cn

Py:   os.getcwd()
来源：http://jg.szsharing.cn

PHP:  getcwd();
来源：http://vr.szxytkj.cn

JS:   process.cwd()
来源：http://qw.chemitech.net.cn

TS:   process.cwd()
来源：http://re.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ww.9csxet.cn

Go:   os.Getwd()
来源：http://cw.shxzukj.cn

Ruby: Dir.pwd
来源：http://ri.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hn.panjiajie.cn

[M05] 设置退出码
来源：http://tk.huixiangedu.cn

Py:   sys.exit(1)
来源：http://fh.521024.cn

PHP:  exit(1);
来源：http://hq.colortex.cn

JS:   process.exit(1)
来源：http://sv.huanxung.cn

TS:   process.exit(1)
来源：http://hl.9csxet.cn

Java: System.exit(1)
来源：http://jv.lnxyls.cn

Go:   os.Exit(1)
来源：http://ce.hnjuh.cn

Ruby: exit 1
来源：http://ub.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xi.panjiajie.cn

[M06] 向标准错误输出
来源：http://ms.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://ia.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cx.newstarts.cn

JS:   console.error("err")
来源：http://to.bookmarksfly.cn

TS:   console.error("err")
来源：http://ya.nszjky.cn

Java: System.err.println("err")
来源：http://ra.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wn.asd995.cn

Ruby: warn "err"
来源：http://ws.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://cy.hnjuh.cn

[M07] 判断是否为主入口
来源：http://kn.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://zr.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://og.hnjuh.cn

JS:   require.main === module
来源：http://mg.panjiajie.cn

TS:   require.main === module
来源：http://qu.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://ko.szsharing.cn

Go:   func main()
来源：http://oa.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://im.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://up.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://vq.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://hy.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://ms.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ou.nszjky.cn

TS:   process.platform;  process.version
来源：http://ei.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oo.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bz.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lz.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ns.chemitech.net.cn

================================================================================
来源：http://ik.bjjhwx.cn

N. 数据结构与算法
来源：http://wj.jianghongdianzi.cn

================================================================================
来源：http://fu.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://pt.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wt.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ds.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ji.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ko.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jk.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://lf.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dq.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mz.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://sy.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://tl.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ll.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://in.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ba.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gz.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://mj.jctech888.com.cn

Ruby: arr.sort
来源：http://xy.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cd.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://wh.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bl.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://uv.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vg.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ud.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xc.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ij.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bw.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xb.chemitech.net.cn

[N04] 斐波那契数列
来源：http://xy.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hh.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ap.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wy.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qq.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ry.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://py.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iz.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uf.bookmarksfly.cn

[N05] 最大公约数
来源：http://rf.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://sr.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kl.wgjwhj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bj.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ry.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ug.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ux.lnxyls.cn

Ruby: a.gcd(b)
来源：http://pl.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yz.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://in.hnjuh.cn

Py:   s == s[::-1]
来源：http://wz.newstarts.cn

PHP:  $s === strrev($s);
来源：http://jt.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://er.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://nk.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yq.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://sm.yuexingan06.cn

Ruby: s == s.reverse
来源：http://dk.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zz.colortex.cn

[N07] 两数之和（返回下标）
来源：http://of.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zp.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cp.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://as.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://df.szsharing.cn

Java: // 手写 HashMap
来源：http://ka.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://ye.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://ae.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ln.haigaiapp.cn

[N08] 生成全排列
来源：http://re.jctech888.com.cn

Py:   itertools.permutations(arr)
来源：http://aa.nszjky.cn

PHP:  // 手写递归交换
来源：http://ux.panjiajie.cn

JS:   // 手写回溯递归
来源：http://vy.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ff.nicolike.cn

Java: // 手写回溯递归
来源：http://lr.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://es.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://qj.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://xa.jctech888.com.cn

[N09] 栈与队列
来源：http://zw.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dj.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xw.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yp.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wn.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kt.lnxyls.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yc.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://di.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zg.huanxung.cn

[N10] 链表节点定义
来源：http://ou.huixinmuqiang.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rc.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yg.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sk.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cr.colortex.cn

Java: class Node { int v; Node next; }
来源：http://pr.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bl.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gx.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ol.colortex.cn

[N11] 二叉树中序遍历
来源：http://tj.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dm.nicolike.cn

PHP:  // 手写递归函数
来源：http://vs.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jm.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://do.jianghongdianzi.cn

Java: // 手写递归
来源：http://zt.yuntaijiaju.cn

Go:   // 手写递归
来源：http://ng.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bn.colortex.cn

C#:   // 手写递归
来源：http://pn.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gz.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yj.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sa.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mv.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zu.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eh.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nk.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ny.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ax.jianghongdianzi.cn

================================================================================
来源：http://ds.panjiajie.cn

O. 并发与异步
来源：http://mw.chemitech.net.cn

================================================================================
来源：http://iw.jctech888.com.cn

[O01] 启动一个线程
来源：http://xx.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zk.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ml.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lx.gzmigu.cn

TS:   // 同 JS
来源：http://iz.521024.cn

Java: new Thread(() -> f()).start()
来源：http://of.huanxung.cn

Go:   go f()
来源：http://oy.asd995.cn

Ruby: Thread.new { f }
来源：http://vg.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ai.9csxet.cn

[O02] 使用线程池
来源：http://po.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://og.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ut.huanxung.cn

JS:   // worker_threads 线程池
来源：http://im.yuntaijiaju.cn

TS:   // worker_threads 线程池
来源：http://cl.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ww.szsharing.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mm.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ei.muxihuayi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sg.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://ow.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://tq.yuntaijiaju.cn

PHP:  // 用 flock() 做文件锁
来源：http://gu.panjiajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vk.jctech888.com.cn

TS:   // 同 JS
来源：http://yc.jianghongdianzi.cn

Java: synchronized (this) { shared++; }
来源：http://wo.hnjuh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uu.lnxyls.cn


<!-- 参考信息 -->