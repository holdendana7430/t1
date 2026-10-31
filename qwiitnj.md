代发 wailian999

[K02] JSON 字符串转对象
来源：http://ly.gzmigu.cn

Py:   json.loads(s)
来源：http://gh.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iv.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://bu.huanxung.cn

TS:   JSON.parse(s)
来源：http://pf.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vt.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://pj.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://vy.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://io.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://xv.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nq.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xu.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vd.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tl.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ir.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pp.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://as.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://bp.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zz.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jl.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uc.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yp.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://px.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ps.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dp.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rw.yuexingan06.cn

[K05] 深拷贝对象
来源：http://xy.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://mx.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://kv.lnxyls.cn

JS:   structuredClone(obj)
来源：http://yn.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://kz.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://su.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dv.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ox.newstarts.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xq.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://yc.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bz.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ra.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yk.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ck.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hp.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cr.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lh.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lw.bookmarksfly.cn

[K07] 进制转换
来源：http://jx.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://el.huixiangedu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jj.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wm.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mt.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hm.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fn.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vs.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lj.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://tk.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ep.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hi.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://hz.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ot.haigaiapp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://is.nszjky.cn

Go:   encoding/gob
来源：http://mr.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://it.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lp.huixinmuqiang.cn

================================================================================
来源：http://it.hnjuh.cn

L. 网络请求
来源：http://av.muxihuayi.cn

================================================================================
来源：http://us.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://wz.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lh.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pb.shtwfgs.cn

JS:   await fetch(url)
来源：http://gt.9csxet.cn

TS:   await fetch(url)
来源：http://cx.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://df.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://ku.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lb.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jq.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://wf.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cf.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uv.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sl.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jj.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://us.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://by.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://si.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iq.wgjwhj.cn

[L03] 设置自定义请求头
来源：http://zu.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fn.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rx.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tx.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kv.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dl.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dw.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xh.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ro.lnxyls.cn

[L04] 设置超时
来源：http://gp.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://fs.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gb.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jy.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hv.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qk.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://no.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://da.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ex.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://dk.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cm.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oh.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sx.bookmarksfly.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gg.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qa.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jp.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jc.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xc.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://nm.huanxung.cn

Py:   resp.json()
来源：http://ea.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://bw.newstarts.cn

JS:   await resp.json()
来源：http://kd.shxzskj.cn

TS:   await resp.json()
来源：http://dw.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ze.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tz.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://rw.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gg.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://er.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ny.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hh.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://nd.colortex.cn

TS:   resp.ok;  resp.status
来源：http://tg.huixiangedu.cn

Java: resp.statusCode()
来源：http://ld.hahajie.cn

Go:   resp.StatusCode
来源：http://cw.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://dl.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://rt.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://wa.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zq.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ga.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sy.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nx.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dm.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uz.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://br.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mm.bjjhwx.cn

================================================================================
来源：http://iz.shtwfgs.cn

M. 命令行 / 进程 / 环境
来源：http://bx.yuexingan06.cn

================================================================================
来源：http://su.chemitech.net.cn

[M01] 读取命令行参数
来源：http://ta.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ku.szsharing.cn

PHP:  $argv;  $argc;
来源：http://bp.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://hu.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://qs.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://ot.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://ci.nszjky.cn

Ruby: ARGV
来源：http://rb.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://rw.panjiajie.cn

[M02] 读取环境变量
来源：http://ru.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://uh.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jm.szsharing.cn

JS:   process.env.HOME
来源：http://ze.521024.cn

TS:   process.env.HOME
来源：http://dt.nicolike.cn

Java: System.getenv("HOME")
来源：http://bb.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dz.hahajie.cn

Ruby: ENV["HOME"]
来源：http://jq.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uq.shxzukj.cn

[M03] 执行外部命令
来源：http://kb.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oi.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rr.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fi.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lt.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ry.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ra.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wo.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://nb.shxzukj.cn

[M04] 获取当前工作目录
来源：http://yf.nszjky.cn

Py:   os.getcwd()
来源：http://mn.yuexingan06.cn

PHP:  getcwd();
来源：http://xn.panjiajie.cn

JS:   process.cwd()
来源：http://bt.huixiangedu.cn

TS:   process.cwd()
来源：http://yt.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://pf.wgjwhj.cn

Go:   os.Getwd()
来源：http://ku.521024.cn

Ruby: Dir.pwd
来源：http://ql.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://he.9csxet.cn

[M05] 设置退出码
来源：http://qz.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://nz.gzmigu.cn

PHP:  exit(1);
来源：http://rx.hahajie.cn

JS:   process.exit(1)
来源：http://oo.huanxung.cn

TS:   process.exit(1)
来源：http://ex.huixiangedu.cn

Java: System.exit(1)
来源：http://rf.nszjky.cn

Go:   os.Exit(1)
来源：http://nq.muxihuayi.cn

Ruby: exit 1
来源：http://ae.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gj.wgjwhj.cn

[M06] 向标准错误输出
来源：http://xw.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://rx.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fl.hnjuh.cn

JS:   console.error("err")
来源：http://vj.bjjhwx.cn

TS:   console.error("err")
来源：http://ea.jctech888.com.cn

Java: System.err.println("err")
来源：http://hj.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qy.nicolike.cn

Ruby: warn "err"
来源：http://ax.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://wr.hahajie.cn

[M07] 判断是否为主入口
来源：http://ec.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://jx.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pf.newstarts.cn

JS:   require.main === module
来源：http://bd.bjjhwx.cn

TS:   require.main === module
来源：http://kh.hahajie.cn

Java: public static void main(String[] args)
来源：http://qh.521024.cn

Go:   func main()
来源：http://bn.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iv.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://vc.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://yf.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://wa.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xm.szsharing.cn

JS:   process.platform;  process.version
来源：http://sa.lnxyls.cn

TS:   process.platform;  process.version
来源：http://lf.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nm.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eb.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ny.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ox.shxzskj.cn

================================================================================
来源：http://va.bjjhwx.cn

N. 数据结构与算法
来源：http://xv.gzmigu.cn

================================================================================
来源：http://zl.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://qv.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lh.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bm.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oy.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qp.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ac.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ba.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ep.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vo.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://od.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wb.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ka.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fa.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ad.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mr.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://sk.szsharing.cn

Ruby: arr.sort
来源：http://zl.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yb.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://bm.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ej.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://pb.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ui.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pv.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vd.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yy.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gp.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vq.shtwfgs.cn

[N04] 斐波那契数列
来源：http://py.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ym.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bw.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yw.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fe.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oi.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gd.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hy.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uz.chemitech.net.cn

[N05] 最大公约数
来源：http://cd.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://xu.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ol.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fa.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ao.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yw.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rr.shxzskj.cn

Ruby: a.gcd(b)
来源：http://fq.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lw.9csxet.cn

[N06] 判断回文字符串
来源：http://ti.521024.cn

Py:   s == s[::-1]
来源：http://vm.colortex.cn

PHP:  $s === strrev($s);
来源：http://sp.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://rt.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://zi.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://in.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://pv.muxihuayi.cn

Ruby: s == s.reverse
来源：http://sz.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bf.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://jj.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yy.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://or.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kt.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://pr.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://hg.szsharing.cn

Go:   // 手写 map[int]int
来源：http://yf.shxzskj.cn

Ruby: // 手写 Hash
来源：http://hk.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ov.colortex.cn

[N08] 生成全排列
来源：http://hp.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://mg.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://or.chemitech.net.cn

JS:   // 手写回溯递归
来源：http://kk.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://yc.521024.cn

Java: // 手写回溯递归
来源：http://az.colortex.cn

Go:   // 手写回溯递归
来源：http://sf.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://ij.9csxet.cn

C#:   // 手写回溯递归
来源：http://op.shxzukj.cn

[N09] 栈与队列
来源：http://ch.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://io.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ar.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eh.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nv.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tw.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hw.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://re.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sc.shtwfgs.cn

[N10] 链表节点定义
来源：http://pc.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ht.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cc.shxzukj.cn


<!-- 参考信息 -->