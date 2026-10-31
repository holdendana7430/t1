代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hv.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vl.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ly.lnxyls.cn

[K05] 深拷贝对象
来源：http://ll.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://nq.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://al.huanxung.cn

JS:   structuredClone(obj)
来源：http://vp.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://uc.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://at.newstarts.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wp.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xi.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gd.colortex.cn

[K06] 解析 URL 查询串
来源：http://rd.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fv.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dm.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sw.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yz.nszjky.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sq.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dm.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ga.bookmarksfly.cn

[K07] 进制转换
来源：http://zs.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ba.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://we.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uh.yuexingan06.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sh.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kx.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ha.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dd.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vo.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://kd.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://xa.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hb.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fv.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://dw.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fk.shxzskj.cn

Go:   encoding/gob
来源：http://nb.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ib.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yd.huixiangedu.cn

================================================================================
来源：http://sn.asd995.cn

L. 网络请求
来源：http://zu.huanxung.cn

================================================================================
来源：http://fi.nszjky.cn

[L01] 发送 GET 请求
来源：http://qm.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sc.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cs.shxzskj.cn

JS:   await fetch(url)
来源：http://dt.shtwfgs.cn

TS:   await fetch(url)
来源：http://tv.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://et.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://cp.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ly.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ya.shxzskj.cn

[L02] 发送 POST JSON
来源：http://ns.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://az.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sz.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ux.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yu.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ju.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mm.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cm.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ue.colortex.cn

[L03] 设置自定义请求头
来源：http://yp.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://om.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mj.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dx.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://os.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ey.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jj.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://by.newstarts.cn

[L04] 设置超时
来源：http://uw.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://sm.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yo.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sp.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fw.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gk.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yt.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pu.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wz.huanxung.cn

[L05] 上传文件（multipart）
来源：http://zp.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mh.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hw.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kt.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dk.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://al.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tn.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oe.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uj.newstarts.cn

[L06] 解析响应为 JSON
来源：http://es.wgjwhj.cn

Py:   resp.json()
来源：http://cv.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ix.haigaiapp.cn

JS:   await resp.json()
来源：http://jq.lnxyls.cn

TS:   await resp.json()
来源：http://zh.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rp.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lq.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ff.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://by.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://dl.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jt.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yp.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://ls.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://en.asd995.cn

Java: resp.statusCode()
来源：http://xe.shxzskj.cn

Go:   resp.StatusCode
来源：http://su.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://gf.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://hu.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://ch.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sj.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://dg.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lb.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://st.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ce.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ql.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fk.huixinmuqiang.cn

================================================================================
来源：http://ui.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://ki.bjjhwx.cn

================================================================================
来源：http://wx.nszjky.cn

[M01] 读取命令行参数
来源：http://iy.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://kw.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://hy.nszjky.cn

JS:   process.argv.slice(2)
来源：http://dk.9csxet.cn

TS:   process.argv.slice(2)
来源：http://ec.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://ar.chemitech.net.cn

Go:   os.Args[1:]
来源：http://od.huixiangedu.cn

Ruby: ARGV
来源：http://ct.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://pz.wgjwhj.cn

[M02] 读取环境变量
来源：http://qw.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://xi.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zn.9csxet.cn

JS:   process.env.HOME
来源：http://qc.wgjwhj.cn

TS:   process.env.HOME
来源：http://kl.asd995.cn

Java: System.getenv("HOME")
来源：http://wi.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sa.nicolike.cn

Ruby: ENV["HOME"]
来源：http://hf.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ew.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://uy.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pp.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qw.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pj.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ms.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qo.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oo.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://xp.huanxung.cn

[M04] 获取当前工作目录
来源：http://mb.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://bv.muxihuayi.cn

PHP:  getcwd();
来源：http://jg.shxzskj.cn

JS:   process.cwd()
来源：http://ap.wgjwhj.cn

TS:   process.cwd()
来源：http://uv.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://rz.shxzukj.cn

Go:   os.Getwd()
来源：http://eh.nszjky.cn

Ruby: Dir.pwd
来源：http://mt.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qe.shxzskj.cn

[M05] 设置退出码
来源：http://hc.panjiajie.cn

Py:   sys.exit(1)
来源：http://pv.huixinmuqiang.cn

PHP:  exit(1);
来源：http://wz.asd995.cn

JS:   process.exit(1)
来源：http://uu.yuexingan06.cn

TS:   process.exit(1)
来源：http://vi.lnxyls.cn

Java: System.exit(1)
来源：http://hn.nszjky.cn

Go:   os.Exit(1)
来源：http://ih.huixiangedu.cn

Ruby: exit 1
来源：http://gw.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wm.szsharing.cn

[M06] 向标准错误输出
来源：http://py.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://vn.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zs.bjjhwx.cn

JS:   console.error("err")
来源：http://ed.521024.cn

TS:   console.error("err")
来源：http://xm.shxzskj.cn

Java: System.err.println("err")
来源：http://kc.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zo.yuntaijiaju.cn

Ruby: warn "err"
来源：http://qv.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://wp.panjiajie.cn

[M07] 判断是否为主入口
来源：http://py.colortex.cn

Py:   if __name__ == "__main__":
来源：http://cp.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rf.yuntaijiaju.cn

JS:   require.main === module
来源：http://jh.521024.cn

TS:   require.main === module
来源：http://pz.hahajie.cn

Java: public static void main(String[] args)
来源：http://sz.521024.cn

Go:   func main()
来源：http://xf.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jm.colortex.cn

C#:   static void Main(string[] args)
来源：http://bw.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://bh.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://cd.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://az.szsharing.cn

JS:   process.platform;  process.version
来源：http://yv.colortex.cn

TS:   process.platform;  process.version
来源：http://bt.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zr.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pc.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bg.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hp.yuntaijiaju.cn

================================================================================
来源：http://fc.yuntaijiaju.cn

N. 数据结构与算法
来源：http://bw.huanxung.cn

================================================================================
来源：http://yw.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://co.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://df.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pd.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iv.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ev.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yg.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://pn.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sb.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://km.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://pm.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://mk.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ex.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bb.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pl.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vn.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://gp.wgjwhj.cn

Ruby: arr.sort
来源：http://th.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ty.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://sm.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vs.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://vv.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ub.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sz.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wl.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hr.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sm.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xn.hahajie.cn

[N04] 斐波那契数列
来源：http://ze.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rl.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xt.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nf.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aq.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aj.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ar.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fk.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zo.shtwfgs.cn

[N05] 最大公约数
来源：http://hb.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://lu.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cw.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://by.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bn.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nx.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://td.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mu.asd995.cn

[N06] 判断回文字符串
来源：http://hy.huixiangedu.cn

Py:   s == s[::-1]
来源：http://dk.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ns.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://vq.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://wm.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dp.huanxung.cn

Go:   // 双指针从两端比较
来源：http://rq.521024.cn

Ruby: s == s.reverse
来源：http://ci.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nv.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://cl.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nb.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fh.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ai.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://cf.shtwfgs.cn

Java: // 手写 HashMap
来源：http://ht.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://tl.gzmigu.cn

Ruby: // 手写 Hash
来源：http://uc.newstarts.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gs.9csxet.cn

[N08] 生成全排列
来源：http://co.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://sx.521024.cn

PHP:  // 手写递归交换
来源：http://lo.521024.cn

JS:   // 手写回溯递归
来源：http://dt.colortex.cn

TS:   // 手写回溯递归
来源：http://sq.yuexingan06.cn

Java: // 手写回溯递归
来源：http://lu.hnjuh.cn

Go:   // 手写回溯递归
来源：http://cb.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://zs.nszjky.cn

C#:   // 手写回溯递归
来源：http://hh.colortex.cn

[N09] 栈与队列
来源：http://zf.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xt.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lk.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yg.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gp.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oh.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mm.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xa.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ka.colortex.cn

[N10] 链表节点定义
来源：http://fo.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tx.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ud.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lr.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mz.newstarts.cn

Java: class Node { int v; Node next; }
来源：http://ax.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gf.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://do.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ew.9csxet.cn

[N11] 二叉树中序遍历
来源：http://uk.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zb.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://jz.newstarts.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sw.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zw.yuntaijiaju.cn

Java: // 手写递归
来源：http://om.gzmigu.cn

Go:   // 手写递归
来源：http://jb.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xi.chemitech.net.cn

C#:   // 手写递归
来源：http://lr.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wt.haigaiapp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rg.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lt.bookmarksfly.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nr.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://in.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aq.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vk.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ea.bookmarksfly.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lr.9csxet.cn


<!-- 参考信息 -->