代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://ga.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://vj.shxzukj.cn

JS:   structuredClone(obj)
来源：http://uh.shxzskj.cn

TS:   structuredClone(obj)
来源：http://qs.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kc.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eh.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uy.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qx.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://rd.bjjhwx.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mr.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://id.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jy.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nd.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nn.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vi.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wv.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jm.9csxet.cn

[K07] 进制转换
来源：http://be.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ti.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wp.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://in.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fq.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://in.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fd.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fu.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lm.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://qn.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://su.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ij.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://oi.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://rd.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rg.jianghongdianzi.cn

Go:   encoding/gob
来源：http://ta.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://pl.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rk.huixiangedu.cn

================================================================================
来源：http://ge.panjiajie.cn

L. 网络请求
来源：http://hj.wgjwhj.cn

================================================================================
来源：http://lb.hnjuh.cn

[L01] 发送 GET 请求
来源：http://sa.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ey.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oq.jctech888.com.cn

JS:   await fetch(url)
来源：http://sb.panjiajie.cn

TS:   await fetch(url)
来源：http://ei.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://so.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://qa.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ud.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ns.hahajie.cn

[L02] 发送 POST JSON
来源：http://jq.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gk.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dx.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://we.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gy.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ru.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yn.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qv.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://du.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://dh.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jv.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yb.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ot.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mb.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ar.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hn.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ba.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ti.nszjky.cn

[L04] 设置超时
来源：http://cj.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://tp.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dv.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ns.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ce.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yk.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ym.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mi.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jl.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://db.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qm.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cj.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fd.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pn.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lx.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rf.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tj.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ie.hahajie.cn

[L06] 解析响应为 JSON
来源：http://gy.haigaiapp.cn

Py:   resp.json()
来源：http://xb.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://zx.huanxung.cn

JS:   await resp.json()
来源：http://oh.shtwfgs.cn

TS:   await resp.json()
来源：http://fw.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nq.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bw.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://om.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cs.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://jq.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mq.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tt.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://hf.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ug.bookmarksfly.cn

Java: resp.statusCode()
来源：http://vj.hahajie.cn

Go:   resp.StatusCode
来源：http://js.huanxung.cn

Ruby: resp.code.to_i
来源：http://yk.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://th.hahajie.cn

[L08] 并发请求多个地址
来源：http://tu.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jw.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://sv.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://id.9csxet.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://se.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rd.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mf.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://av.szxytkj.cn

================================================================================
来源：http://gh.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://rx.521024.cn

================================================================================
来源：http://zu.haigaiapp.cn

[M01] 读取命令行参数
来源：http://zf.shxzskj.cn

Py:   sys.argv[1:]
来源：http://gh.asd995.cn

PHP:  $argv;  $argc;
来源：http://ht.521024.cn

JS:   process.argv.slice(2)
来源：http://mx.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://zx.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://xa.bjjhwx.cn

Go:   os.Args[1:]
来源：http://jz.jctech888.com.cn

Ruby: ARGV
来源：http://tk.muxihuayi.cn

C#:   args 数组（Main 方法参数）
来源：http://yn.shtwfgs.cn

[M02] 读取环境变量
来源：http://ln.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://iu.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dp.bookmarksfly.cn

JS:   process.env.HOME
来源：http://xv.bjjhwx.cn

TS:   process.env.HOME
来源：http://yc.lnxyls.cn

Java: System.getenv("HOME")
来源：http://px.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zt.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://vv.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://th.asd995.cn

[M03] 执行外部命令
来源：http://cz.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oh.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://et.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sd.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sj.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pa.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ea.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://be.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://cm.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://ae.bjjhwx.cn

Py:   os.getcwd()
来源：http://vs.huanxung.cn

PHP:  getcwd();
来源：http://jy.jianghongdianzi.cn

JS:   process.cwd()
来源：http://di.bookmarksfly.cn

TS:   process.cwd()
来源：http://fi.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://zo.chemitech.net.cn

Go:   os.Getwd()
来源：http://bi.haigaiapp.cn

Ruby: Dir.pwd
来源：http://ig.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ja.haigaiapp.cn

[M05] 设置退出码
来源：http://vb.521024.cn

Py:   sys.exit(1)
来源：http://kx.bjjhwx.cn

PHP:  exit(1);
来源：http://lv.asd995.cn

JS:   process.exit(1)
来源：http://bz.muxihuayi.cn

TS:   process.exit(1)
来源：http://il.shtwfgs.cn

Java: System.exit(1)
来源：http://gk.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://lj.bjjhwx.cn

Ruby: exit 1
来源：http://xa.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gc.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://rn.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://sp.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://it.bookmarksfly.cn

JS:   console.error("err")
来源：http://fa.panjiajie.cn

TS:   console.error("err")
来源：http://ug.gzmigu.cn

Java: System.err.println("err")
来源：http://zq.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cc.chemitech.net.cn

Ruby: warn "err"
来源：http://bj.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://yb.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://gb.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://wd.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lt.newstarts.cn

JS:   require.main === module
来源：http://tp.bookmarksfly.cn

TS:   require.main === module
来源：http://tc.szxytkj.cn

Java: public static void main(String[] args)
来源：http://gg.nicolike.cn

Go:   func main()
来源：http://hy.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xg.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://it.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://at.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://hd.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://vo.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://ys.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://gh.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://en.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oq.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wd.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jj.nszjky.cn

================================================================================
来源：http://xs.gzmigu.cn

N. 数据结构与算法
来源：http://um.nszjky.cn

================================================================================
来源：http://fz.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://lp.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gi.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vv.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://al.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fm.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xj.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://tg.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wv.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://th.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://no.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pa.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://px.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ky.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nh.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://nx.panjiajie.cn

Ruby: arr.sort
来源：http://qz.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ai.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://mu.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://di.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://fh.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gk.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wr.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mk.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nq.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rw.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gg.521024.cn

[N04] 斐波那契数列
来源：http://am.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gc.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rk.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://af.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ov.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ki.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nk.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://em.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xe.szxytkj.cn

[N05] 最大公约数
来源：http://vl.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://mv.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://es.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://do.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vj.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nl.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sa.huanxung.cn

Ruby: a.gcd(b)
来源：http://lm.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hl.muxihuayi.cn

[N06] 判断回文字符串
来源：http://mi.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://tz.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://fs.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://no.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ig.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ux.colortex.cn

Go:   // 双指针从两端比较
来源：http://zx.gzmigu.cn

Ruby: s == s.reverse
来源：http://sa.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nm.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://cz.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tq.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nv.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cv.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://az.nicolike.cn

Java: // 手写 HashMap
来源：http://hx.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://vz.panjiajie.cn

Ruby: // 手写 Hash
来源：http://eo.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bn.gzmigu.cn

[N08] 生成全排列
来源：http://af.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://mj.newstarts.cn

PHP:  // 手写递归交换
来源：http://qi.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://em.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://lz.nszjky.cn

Java: // 手写回溯递归
来源：http://sd.shxzskj.cn

Go:   // 手写回溯递归
来源：http://gb.colortex.cn

Ruby: arr.permutation.to_a
来源：http://yj.huanxung.cn

C#:   // 手写回溯递归
来源：http://ej.bookmarksfly.cn

[N09] 栈与队列
来源：http://kp.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vm.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wv.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ha.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://od.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ez.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nq.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qm.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://un.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://so.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qf.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://md.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fj.bjjhwx.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rv.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://oe.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fd.szxytkj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mg.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gn.colortex.cn

[N11] 二叉树中序遍历
来源：http://cp.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qs.nicolike.cn

PHP:  // 手写递归函数
来源：http://tn.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hk.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xq.wgjwhj.cn

Java: // 手写递归
来源：http://qj.yuntaijiaju.cn

Go:   // 手写递归
来源：http://gg.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://id.521024.cn

C#:   // 手写递归
来源：http://hw.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ne.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://or.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yn.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qy.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mz.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zt.newstarts.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ex.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xx.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oq.bjjhwx.cn

================================================================================
来源：http://ty.hahajie.cn

O. 并发与异步
来源：http://xd.yuexingan06.cn

================================================================================
来源：http://as.shxzukj.cn

[O01] 启动一个线程
来源：http://dq.szsharing.cn


<!-- 参考信息 -->