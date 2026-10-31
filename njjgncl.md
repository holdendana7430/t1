代发 wailian999

TS:   JSON.parse(s)
来源：http://ma.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nj.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://fj.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://ad.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fy.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://is.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vs.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wa.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ny.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nb.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bm.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tl.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zk.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hh.nicolike.cn

[K04] 读取 JSON 文件
来源：http://up.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://na.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bb.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ew.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bv.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ae.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xz.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oo.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xe.nicolike.cn

[K05] 深拷贝对象
来源：http://fh.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://yh.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://as.lnxyls.cn

JS:   structuredClone(obj)
来源：http://hr.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://wq.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mb.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mx.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fy.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cq.huanxung.cn

[K06] 解析 URL 查询串
来源：http://ih.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cw.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xl.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jl.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jq.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pn.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ff.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gr.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jy.shxzskj.cn

[K07] 进制转换
来源：http://qa.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kb.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://od.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mp.wgjwhj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zk.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fh.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zn.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yc.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://va.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://iz.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://ic.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nr.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://et.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://tn.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cz.lnxyls.cn

Go:   encoding/gob
来源：http://od.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://ay.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xm.bookmarksfly.cn

================================================================================
来源：http://so.shtwfgs.cn

L. 网络请求
来源：http://cv.muxihuayi.cn

================================================================================
来源：http://mc.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://eu.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lg.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://np.hnjuh.cn

JS:   await fetch(url)
来源：http://to.shtwfgs.cn

TS:   await fetch(url)
来源：http://bw.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tj.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://co.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lg.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zf.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://if.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lb.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://op.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rr.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://et.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vf.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://te.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://do.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hx.colortex.cn

[L03] 设置自定义请求头
来源：http://vn.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vn.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rk.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dj.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wi.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uu.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rg.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cb.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jv.haigaiapp.cn

[L04] 设置超时
来源：http://ev.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://ci.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://we.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wg.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sb.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yx.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xf.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kz.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://cd.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vz.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yj.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ds.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qz.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ff.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qv.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kj.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lz.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://wc.shtwfgs.cn

Py:   resp.json()
来源：http://yp.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://kb.szxytkj.cn

JS:   await resp.json()
来源：http://zu.muxihuayi.cn

TS:   await resp.json()
来源：http://xa.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jp.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ka.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://su.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://it.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://ak.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cv.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bp.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://ft.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://ep.hahajie.cn

Java: resp.statusCode()
来源：http://ny.nszjky.cn

Go:   resp.StatusCode
来源：http://fc.hnjuh.cn

Ruby: resp.code.to_i
来源：http://tr.colortex.cn

C#:   (int)resp.StatusCode
来源：http://no.szsharing.cn

[L08] 并发请求多个地址
来源：http://dy.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zm.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://go.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rd.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pd.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ne.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pp.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nd.szxytkj.cn

================================================================================
来源：http://eu.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://qv.yuntaijiaju.cn

================================================================================
来源：http://be.jctech888.com.cn

[M01] 读取命令行参数
来源：http://zy.shxzskj.cn

Py:   sys.argv[1:]
来源：http://on.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://gf.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://pk.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://xb.szsharing.cn

Java: args 数组（main 方法参数）
来源：http://tl.muxihuayi.cn

Go:   os.Args[1:]
来源：http://yq.jctech888.com.cn

Ruby: ARGV
来源：http://qe.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://vm.gzmigu.cn

[M02] 读取环境变量
来源：http://eq.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://wf.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wg.shxzukj.cn

JS:   process.env.HOME
来源：http://ve.asd995.cn

TS:   process.env.HOME
来源：http://ib.nszjky.cn

Java: System.getenv("HOME")
来源：http://rz.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kf.nicolike.cn

Ruby: ENV["HOME"]
来源：http://ns.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cr.jctech888.com.cn

[M03] 执行外部命令
来源：http://vv.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yg.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://we.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ix.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pl.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://de.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xe.shxzukj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wn.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://qi.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ck.muxihuayi.cn

Py:   os.getcwd()
来源：http://wn.panjiajie.cn

PHP:  getcwd();
来源：http://qf.521024.cn

JS:   process.cwd()
来源：http://xs.colortex.cn

TS:   process.cwd()
来源：http://sy.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://qo.bjjhwx.cn

Go:   os.Getwd()
来源：http://dq.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://si.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hn.yuntaijiaju.cn

[M05] 设置退出码
来源：http://rz.panjiajie.cn

Py:   sys.exit(1)
来源：http://qw.nszjky.cn

PHP:  exit(1);
来源：http://lh.colortex.cn

JS:   process.exit(1)
来源：http://wq.haigaiapp.cn

TS:   process.exit(1)
来源：http://qd.gzmigu.cn

Java: System.exit(1)
来源：http://ri.colortex.cn

Go:   os.Exit(1)
来源：http://wg.lnxyls.cn

Ruby: exit 1
来源：http://ez.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fm.shxzskj.cn

[M06] 向标准错误输出
来源：http://ew.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://kh.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sl.jianghongdianzi.cn

JS:   console.error("err")
来源：http://xw.9csxet.cn

TS:   console.error("err")
来源：http://lw.huixiangedu.cn

Java: System.err.println("err")
来源：http://tx.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://to.szxytkj.cn

Ruby: warn "err"
来源：http://sx.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://oe.gzmigu.cn

[M07] 判断是否为主入口
来源：http://qp.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://cb.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ln.huixinmuqiang.cn

JS:   require.main === module
来源：http://qu.huixiangedu.cn

TS:   require.main === module
来源：http://ib.newstarts.cn

Java: public static void main(String[] args)
来源：http://lm.lnxyls.cn

Go:   func main()
来源：http://wr.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bq.521024.cn

C#:   static void Main(string[] args)
来源：http://wr.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://rh.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://un.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://te.lnxyls.cn

JS:   process.platform;  process.version
来源：http://tc.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://yo.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://if.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ua.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dq.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vf.colortex.cn

================================================================================
来源：http://ch.colortex.cn

N. 数据结构与算法
来源：http://es.nszjky.cn

================================================================================
来源：http://lm.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://uh.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pa.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wu.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sh.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fa.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oa.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://xw.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ci.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hr.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://si.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://fw.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jo.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fh.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fd.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ki.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ts.asd995.cn

Ruby: arr.sort
来源：http://rf.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sa.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://ts.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zq.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://um.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uu.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://im.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ta.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xg.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mj.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ay.asd995.cn

[N04] 斐波那契数列
来源：http://uc.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://em.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://na.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jf.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ba.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://el.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ht.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rc.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ds.yuexingan06.cn

[N05] 最大公约数
来源：http://uv.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://kt.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://am.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pl.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jn.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://by.newstarts.cn

Ruby: a.gcd(b)
来源：http://pv.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xx.hnjuh.cn

[N06] 判断回文字符串
来源：http://sp.haigaiapp.cn

Py:   s == s[::-1]
来源：http://fv.nicolike.cn

PHP:  $s === strrev($s);
来源：http://lb.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://gm.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://ko.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ad.9csxet.cn

Go:   // 双指针从两端比较
来源：http://vx.yuexingan06.cn

Ruby: s == s.reverse
来源：http://eq.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qh.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://pt.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://do.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hp.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vp.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://kk.bjjhwx.cn

Java: // 手写 HashMap
来源：http://gr.newstarts.cn

Go:   // 手写 map[int]int
来源：http://tj.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://df.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mo.szxytkj.cn

[N08] 生成全排列
来源：http://fd.9csxet.cn

Py:   itertools.permutations(arr)
来源：http://gv.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ds.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://cr.shxzukj.cn

TS:   // 手写回溯递归
来源：http://ly.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://fx.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://jq.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://ac.huanxung.cn

C#:   // 手写回溯递归
来源：http://mt.shxzskj.cn

[N09] 栈与队列
来源：http://jj.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gm.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jy.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mc.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ht.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gq.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hi.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eo.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sf.nszjky.cn

[N10] 链表节点定义
来源：http://mc.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wu.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pw.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xu.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ns.521024.cn

Java: class Node { int v; Node next; }
来源：http://eo.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://te.lnxyls.cn


<!-- 参考信息 -->