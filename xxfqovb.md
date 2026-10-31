代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uk.bookmarksfly.cn

[K07] 进制转换
来源：http://xn.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oc.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wv.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pz.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qy.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wn.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ua.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nl.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lb.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://go.521024.cn

Py:   pickle.dumps(obj)
来源：http://az.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vu.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://ga.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://ms.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yf.huixiangedu.cn

Go:   encoding/gob
来源：http://ih.521024.cn

Ruby: Marshal.dump(obj)
来源：http://oh.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pe.huixinmuqiang.cn

================================================================================
来源：http://hc.huanxung.cn

L. 网络请求
来源：http://pj.colortex.cn

================================================================================
来源：http://cf.521024.cn

[L01] 发送 GET 请求
来源：http://xh.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pu.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pb.hahajie.cn

JS:   await fetch(url)
来源：http://dm.asd995.cn

TS:   await fetch(url)
来源：http://nk.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mt.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://tz.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://do.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ip.hnjuh.cn

[L02] 发送 POST JSON
来源：http://th.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yn.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vi.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ez.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sv.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bc.lnxyls.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rp.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bu.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cp.gzmigu.cn

[L03] 设置自定义请求头
来源：http://tk.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mo.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ud.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tr.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ve.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kt.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fw.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jd.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qk.hahajie.cn

[L04] 设置超时
来源：http://dj.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://vf.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://re.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jt.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://so.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ut.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cg.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://de.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pk.wgjwhj.cn

[L05] 上传文件（multipart）
来源：http://yh.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wd.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fd.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kf.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ty.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jw.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ni.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cz.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uq.huanxung.cn

[L06] 解析响应为 JSON
来源：http://gb.szxytkj.cn

Py:   resp.json()
来源：http://pr.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://kv.lnxyls.cn

JS:   await resp.json()
来源：http://dr.asd995.cn

TS:   await resp.json()
来源：http://vk.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ec.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gb.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://fn.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ue.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://yr.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uv.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wt.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://zp.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://zb.nicolike.cn

Java: resp.statusCode()
来源：http://jh.newstarts.cn

Go:   resp.StatusCode
来源：http://nm.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://jh.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://gw.hnjuh.cn

[L08] 并发请求多个地址
来源：http://ng.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mr.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://au.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://br.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kp.jianghongdianzi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xq.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cj.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tb.panjiajie.cn

================================================================================
来源：http://nx.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://gz.huanxung.cn

================================================================================
来源：http://zk.huanxung.cn

[M01] 读取命令行参数
来源：http://xo.panjiajie.cn

Py:   sys.argv[1:]
来源：http://lv.nicolike.cn

PHP:  $argv;  $argc;
来源：http://lm.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://yr.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://nn.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://gp.huanxung.cn

Go:   os.Args[1:]
来源：http://hp.asd995.cn

Ruby: ARGV
来源：http://xc.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://cl.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://wo.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://wv.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vs.hnjuh.cn

JS:   process.env.HOME
来源：http://wz.huanxung.cn

TS:   process.env.HOME
来源：http://zh.521024.cn

Java: System.getenv("HOME")
来源：http://oa.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tv.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://vr.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fx.lnxyls.cn

[M03] 执行外部命令
来源：http://zd.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://en.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qm.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lc.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wg.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aj.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vq.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qv.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://tt.hnjuh.cn

[M04] 获取当前工作目录
来源：http://nt.huanxung.cn

Py:   os.getcwd()
来源：http://py.huixiangedu.cn

PHP:  getcwd();
来源：http://ih.lnxyls.cn

JS:   process.cwd()
来源：http://pr.nszjky.cn

TS:   process.cwd()
来源：http://ey.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://dg.shtwfgs.cn

Go:   os.Getwd()
来源：http://iz.shxzskj.cn

Ruby: Dir.pwd
来源：http://qk.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mh.hahajie.cn

[M05] 设置退出码
来源：http://cw.huanxung.cn

Py:   sys.exit(1)
来源：http://aw.haigaiapp.cn

PHP:  exit(1);
来源：http://md.huanxung.cn

JS:   process.exit(1)
来源：http://xj.9csxet.cn

TS:   process.exit(1)
来源：http://aa.panjiajie.cn

Java: System.exit(1)
来源：http://lw.shtwfgs.cn

Go:   os.Exit(1)
来源：http://iq.panjiajie.cn

Ruby: exit 1
来源：http://fv.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://on.9csxet.cn

[M06] 向标准错误输出
来源：http://ua.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://bf.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bl.bjjhwx.cn

JS:   console.error("err")
来源：http://fa.haigaiapp.cn

TS:   console.error("err")
来源：http://qk.hahajie.cn

Java: System.err.println("err")
来源：http://vn.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nb.chemitech.net.cn

Ruby: warn "err"
来源：http://mu.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ln.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://xa.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://hn.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kt.jianghongdianzi.cn

JS:   require.main === module
来源：http://kn.panjiajie.cn

TS:   require.main === module
来源：http://nn.colortex.cn

Java: public static void main(String[] args)
来源：http://ty.haigaiapp.cn

Go:   func main()
来源：http://jm.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qp.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://qg.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://ye.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://zl.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://rr.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://bx.lnxyls.cn

TS:   process.platform;  process.version
来源：http://yz.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qa.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dh.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oh.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ii.szsharing.cn

================================================================================
来源：http://au.shxzukj.cn

N. 数据结构与算法
来源：http://pz.nszjky.cn

================================================================================
来源：http://kj.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://zn.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ix.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://py.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pr.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://du.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://pd.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bz.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oq.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ib.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://jg.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xa.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zk.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wf.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qv.szsharing.cn

Go:   slices.Sort(arr)
来源：http://qr.huixiangedu.cn

Ruby: arr.sort
来源：http://rr.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ks.colortex.cn

[N03] 快速排序（分治示例）
来源：http://lb.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bz.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://wm.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xh.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tk.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://do.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://av.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ea.huanxung.cn

[N04] 斐波那契数列
来源：http://lv.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sx.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ty.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dm.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bo.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cd.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ra.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pt.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ik.jianghongdianzi.cn

[N05] 最大公约数
来源：http://fr.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://nm.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gt.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eg.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gs.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ey.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zz.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://lr.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rk.szsharing.cn

[N06] 判断回文字符串
来源：http://qk.szxytkj.cn

Py:   s == s[::-1]
来源：http://ni.huanxung.cn

PHP:  $s === strrev($s);
来源：http://lp.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://zl.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://bi.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ey.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://gi.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://he.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lx.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://wb.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ng.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xo.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ag.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://sn.bjjhwx.cn

Java: // 手写 HashMap
来源：http://az.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://fj.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://fq.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gm.szsharing.cn

[N08] 生成全排列
来源：http://ga.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://nw.asd995.cn

PHP:  // 手写递归交换
来源：http://nz.521024.cn

JS:   // 手写回溯递归
来源：http://ri.9csxet.cn

TS:   // 手写回溯递归
来源：http://mn.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ou.colortex.cn

Go:   // 手写回溯递归
来源：http://zp.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://vr.shxzskj.cn

C#:   // 手写回溯递归
来源：http://hh.szxytkj.cn

[N09] 栈与队列
来源：http://zh.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kh.asd995.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dy.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://im.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yn.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uu.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qn.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bl.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gn.huanxung.cn

[N10] 链表节点定义
来源：http://tw.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yz.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dd.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zx.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wz.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://gg.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vv.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yk.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cv.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://si.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mb.nszjky.cn

PHP:  // 手写递归函数
来源：http://ud.panjiajie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vo.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oq.asd995.cn

Java: // 手写递归
来源：http://rn.jianghongdianzi.cn

Go:   // 手写递归
来源：http://pc.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jw.gzmigu.cn

C#:   // 手写递归
来源：http://kl.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ls.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dt.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ky.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://it.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rn.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yi.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kv.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ew.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://us.shxzukj.cn

================================================================================
来源：http://bj.jianghongdianzi.cn

O. 并发与异步
来源：http://ee.nszjky.cn

================================================================================
来源：http://jq.bookmarksfly.cn

[O01] 启动一个线程
来源：http://kt.yuexingan06.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://se.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://un.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cd.yuntaijiaju.cn

TS:   // 同 JS
来源：http://jg.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://oj.shxzukj.cn

Go:   go f()
来源：http://mf.wgjwhj.cn

Ruby: Thread.new { f }
来源：http://wh.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://gl.huixiangedu.cn

[O02] 使用线程池
来源：http://zj.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yi.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sn.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://ky.huanxung.cn

TS:   // worker_threads 线程池
来源：http://ov.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cr.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ij.chemitech.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uc.szxytkj.cn


<!-- 参考信息 -->