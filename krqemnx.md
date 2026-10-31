代发 wailian999

[K02] JSON 字符串转对象
来源：http://ss.szsharing.cn

Py:   json.loads(s)
来源：http://sp.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jv.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://fz.shxzskj.cn

TS:   JSON.parse(s)
来源：http://wp.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xm.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://kh.asd995.cn

Ruby: JSON.parse(s)
来源：http://ii.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kp.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://bg.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bi.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://st.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://az.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nt.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qp.yuexingan06.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://om.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qo.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mo.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://hq.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iq.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uu.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zl.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gf.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bc.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bq.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ug.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://na.nszjky.cn

[K05] 深拷贝对象
来源：http://it.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://qd.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://ge.521024.cn

JS:   structuredClone(obj)
来源：http://ur.szsharing.cn

TS:   structuredClone(obj)
来源：http://ho.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gw.nicolike.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dc.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vs.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cl.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://ts.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ba.chemitech.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fb.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rk.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bb.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cg.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qy.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bl.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://is.newstarts.cn

[K07] 进制转换
来源：http://zc.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uv.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qo.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fv.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yc.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ks.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pk.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bd.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dp.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://us.colortex.cn

Py:   pickle.dumps(obj)
来源：http://lf.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fi.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://vv.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://we.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hc.bookmarksfly.cn

Go:   encoding/gob
来源：http://cw.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://cb.szsharing.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qt.szsharing.cn

================================================================================
来源：http://zc.shxzukj.cn

L. 网络请求
来源：http://hu.asd995.cn

================================================================================
来源：http://tm.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://sj.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nn.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fd.hahajie.cn

JS:   await fetch(url)
来源：http://xf.chemitech.net.cn

TS:   await fetch(url)
来源：http://io.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://av.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://hi.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xw.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jp.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://os.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dv.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qk.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xr.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vc.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://th.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://am.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tf.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ta.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://rq.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ep.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qf.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dv.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ca.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hs.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uo.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://om.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wk.bookmarksfly.cn

[L04] 设置超时
来源：http://xr.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://gt.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zm.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dz.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ud.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tc.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://el.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jy.nicolike.cn

[L05] 上传文件（multipart）
来源：http://rl.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tj.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://im.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://el.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yw.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://in.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hg.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pq.huanxung.cn

[L06] 解析响应为 JSON
来源：http://bf.shxzukj.cn

Py:   resp.json()
来源：http://ds.521024.cn

PHP:  json_decode($body, true);
来源：http://yi.muxihuayi.cn

JS:   await resp.json()
来源：http://fv.haigaiapp.cn

TS:   await resp.json()
来源：http://wm.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fo.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://to.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://td.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gv.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://zo.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mj.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://em.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ew.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://ma.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://ws.szsharing.cn

Go:   resp.StatusCode
来源：http://qw.nicolike.cn

Ruby: resp.code.to_i
来源：http://xr.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://wz.colortex.cn

[L08] 并发请求多个地址
来源：http://wq.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ai.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://ct.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ca.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kh.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ou.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qv.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nr.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://en.yuexingan06.cn

================================================================================
来源：http://wz.bookmarksfly.cn

M. 命令行 / 进程 / 环境
来源：http://su.huixiangedu.cn

================================================================================
来源：http://ok.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://jm.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://te.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://gj.521024.cn

JS:   process.argv.slice(2)
来源：http://zq.huanxung.cn

TS:   process.argv.slice(2)
来源：http://li.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://vu.szsharing.cn

Go:   os.Args[1:]
来源：http://ut.521024.cn

Ruby: ARGV
来源：http://iz.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://vy.hnjuh.cn

[M02] 读取环境变量
来源：http://zi.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://mv.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mt.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://kq.yuexingan06.cn

TS:   process.env.HOME
来源：http://ic.szsharing.cn

Java: System.getenv("HOME")
来源：http://nu.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ws.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://ft.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vq.9csxet.cn

[M03] 执行外部命令
来源：http://le.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dp.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rk.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wz.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fb.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sa.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uy.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sv.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://jp.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://oa.colortex.cn

Py:   os.getcwd()
来源：http://na.colortex.cn

PHP:  getcwd();
来源：http://nz.panjiajie.cn

JS:   process.cwd()
来源：http://hw.bookmarksfly.cn

TS:   process.cwd()
来源：http://pf.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://bv.newstarts.cn

Go:   os.Getwd()
来源：http://hu.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://pv.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jt.gzmigu.cn

[M05] 设置退出码
来源：http://rc.shtwfgs.cn

Py:   sys.exit(1)
来源：http://fe.shxzukj.cn

PHP:  exit(1);
来源：http://ri.szsharing.cn

JS:   process.exit(1)
来源：http://wm.yuexingan06.cn

TS:   process.exit(1)
来源：http://sw.huanxung.cn

Java: System.exit(1)
来源：http://we.shxzskj.cn

Go:   os.Exit(1)
来源：http://bq.hahajie.cn

Ruby: exit 1
来源：http://jl.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ma.shxzskj.cn

[M06] 向标准错误输出
来源：http://qg.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://is.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bx.lnxyls.cn

JS:   console.error("err")
来源：http://zt.nicolike.cn

TS:   console.error("err")
来源：http://sv.chemitech.net.cn

Java: System.err.println("err")
来源：http://ni.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dj.9csxet.cn

Ruby: warn "err"
来源：http://ob.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://pw.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://ja.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://nx.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ar.chemitech.net.cn

JS:   require.main === module
来源：http://no.nszjky.cn

TS:   require.main === module
来源：http://tv.newstarts.cn

Java: public static void main(String[] args)
来源：http://ss.521024.cn

Go:   func main()
来源：http://tg.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ud.huanxung.cn

C#:   static void Main(string[] args)
来源：http://ct.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://zf.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://lt.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://oi.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://vd.9csxet.cn

TS:   process.platform;  process.version
来源：http://vw.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ba.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cb.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rd.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://te.szxytkj.cn

================================================================================
来源：http://gc.colortex.cn

N. 数据结构与算法
来源：http://yt.yuntaijiaju.cn

================================================================================
来源：http://di.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://kt.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kz.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://su.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hm.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zs.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qh.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ar.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uu.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://av.huixinmuqiang.cn

[N02] 排序（工程实践用内置实现）
来源：http://pk.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://ys.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hh.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://un.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yu.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rr.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://sw.hnjuh.cn

Ruby: arr.sort
来源：http://eg.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yk.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://iq.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wh.hnjuh.cn

PHP:  // 递归实现，或用 usort
来源：http://ob.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ud.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://di.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kq.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vf.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kb.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dt.hahajie.cn

[N04] 斐波那契数列
来源：http://tk.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dp.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xy.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fw.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fh.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wu.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qo.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qt.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://af.nicolike.cn

[N05] 最大公约数
来源：http://iy.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://jc.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gj.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rl.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gm.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ax.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sn.nicolike.cn

Ruby: a.gcd(b)
来源：http://ot.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ow.lnxyls.cn

[N06] 判断回文字符串
来源：http://pv.szxytkj.cn

Py:   s == s[::-1]
来源：http://pj.szsharing.cn

PHP:  $s === strrev($s);
来源：http://mv.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://sj.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://af.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ck.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://xw.colortex.cn

Ruby: s == s.reverse
来源：http://pg.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yl.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://jd.wgjwhj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://or.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mp.bookmarksfly.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://be.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://xa.huixiangedu.cn

Java: // 手写 HashMap
来源：http://yl.muxihuayi.cn

Go:   // 手写 map[int]int
来源：http://fq.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://zj.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gv.yuntaijiaju.cn

[N08] 生成全排列
来源：http://vv.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://dg.shxzukj.cn

PHP:  // 手写递归交换
来源：http://xw.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://jh.521024.cn

TS:   // 手写回溯递归
来源：http://hf.yuexingan06.cn

Java: // 手写回溯递归
来源：http://hk.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://zo.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://xe.nicolike.cn

C#:   // 手写回溯递归
来源：http://zg.gzmigu.cn

[N09] 栈与队列
来源：http://qa.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vf.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tq.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ju.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vj.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vl.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wv.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nd.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pl.lnxyls.cn

[N10] 链表节点定义
来源：http://fg.chemitech.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tk.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qj.haigaiapp.cn


<!-- 参考信息 -->