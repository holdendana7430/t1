代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hy.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://im.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nn.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://zt.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jl.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jr.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://te.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lz.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hw.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ip.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ru.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zn.huanxung.cn

================================================================================
来源：http://pl.hnjuh.cn

K. JSON 与序列化
来源：http://jf.nicolike.cn

================================================================================
来源：http://hs.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://ky.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xt.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iu.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://zx.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://fq.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sk.nicolike.cn

Go:   json.Marshal(obj)
来源：http://qn.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yb.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yb.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ay.shxzskj.cn

Py:   json.loads(s)
来源：http://kt.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jt.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://oq.szxytkj.cn

TS:   JSON.parse(s)
来源：http://fq.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tw.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://uv.nszjky.cn

Ruby: JSON.parse(s)
来源：http://sr.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://io.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://bm.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ka.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hh.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hh.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wm.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fm.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hd.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jy.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ij.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://ph.jctech888.com.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xo.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hg.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rz.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ct.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ng.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jv.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yj.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ma.hahajie.cn

[K05] 深拷贝对象
来源：http://ry.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://yh.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://oq.521024.cn

JS:   structuredClone(obj)
来源：http://qq.gzmigu.cn

TS:   structuredClone(obj)
来源：http://xs.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ll.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yn.wgjwhj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nb.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zi.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://jz.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ki.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qp.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cx.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oh.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ra.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yk.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sq.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ku.bookmarksfly.cn

[K07] 进制转换
来源：http://ed.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://er.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ng.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zv.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://es.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mp.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kh.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hh.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://xn.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://vs.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://al.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://zc.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://nk.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nf.bjjhwx.cn

Go:   encoding/gob
来源：http://bz.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://rg.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yq.jianghongdianzi.cn

================================================================================
来源：http://zp.panjiajie.cn

L. 网络请求
来源：http://re.panjiajie.cn

================================================================================
来源：http://dc.asd995.cn

[L01] 发送 GET 请求
来源：http://ji.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vr.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jq.shxzskj.cn

JS:   await fetch(url)
来源：http://rh.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://tp.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ua.nszjky.cn

Go:   resp, err := http.Get(url)
来源：http://he.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ny.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://he.huanxung.cn

[L02] 发送 POST JSON
来源：http://zh.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ca.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wn.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xp.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pl.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xm.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bn.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yh.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ns.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://kf.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ki.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gc.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ox.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zb.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vx.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hx.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lo.nszjky.cn

[L04] 设置超时
来源：http://cr.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://zm.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ut.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cc.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vv.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xw.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oe.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://si.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ar.nszjky.cn

[L05] 上传文件（multipart）
来源：http://jk.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rs.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wu.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sl.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mw.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nc.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uj.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://af.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://se.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://ot.9csxet.cn

Py:   resp.json()
来源：http://pn.newstarts.cn

PHP:  json_decode($body, true);
来源：http://xc.szsharing.cn

JS:   await resp.json()
来源：http://mp.asd995.cn

TS:   await resp.json()
来源：http://ak.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bm.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jt.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://vw.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ed.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://em.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ee.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jd.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://wc.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://qy.hahajie.cn

Java: resp.statusCode()
来源：http://ri.asd995.cn

Go:   resp.StatusCode
来源：http://ll.panjiajie.cn

Ruby: resp.code.to_i
来源：http://cf.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://yu.nicolike.cn

[L08] 并发请求多个地址
来源：http://tl.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ki.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://sm.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bx.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dz.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ni.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iw.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ir.521024.cn

================================================================================
来源：http://ll.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://xq.shxzukj.cn

================================================================================
来源：http://zq.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://ep.colortex.cn

Py:   sys.argv[1:]
来源：http://go.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://xk.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://jk.huanxung.cn

TS:   process.argv.slice(2)
来源：http://or.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://tz.szxytkj.cn

Go:   os.Args[1:]
来源：http://wa.bjjhwx.cn

Ruby: ARGV
来源：http://ta.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://ws.lnxyls.cn

[M02] 读取环境变量
来源：http://vi.muxihuayi.cn

Py:   os.environ.get("HOME")
来源：http://tg.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aa.hahajie.cn

JS:   process.env.HOME
来源：http://ue.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://sw.asd995.cn

Java: System.getenv("HOME")
来源：http://ti.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ua.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://yb.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fy.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://iu.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rz.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rd.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ee.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gz.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oh.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tw.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xe.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://lj.huanxung.cn

[M04] 获取当前工作目录
来源：http://em.yuexingan06.cn

Py:   os.getcwd()
来源：http://ie.yuntaijiaju.cn

PHP:  getcwd();
来源：http://bn.chemitech.net.cn

JS:   process.cwd()
来源：http://si.lnxyls.cn

TS:   process.cwd()
来源：http://qf.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://hs.nszjky.cn

Go:   os.Getwd()
来源：http://cy.colortex.cn

Ruby: Dir.pwd
来源：http://dv.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ii.yuntaijiaju.cn

[M05] 设置退出码
来源：http://oh.521024.cn

Py:   sys.exit(1)
来源：http://jq.wgjwhj.cn

PHP:  exit(1);
来源：http://pf.asd995.cn

JS:   process.exit(1)
来源：http://cf.muxihuayi.cn

TS:   process.exit(1)
来源：http://hd.szxytkj.cn

Java: System.exit(1)
来源：http://br.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://fk.nicolike.cn

Ruby: exit 1
来源：http://hl.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ci.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ov.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://go.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://az.shtwfgs.cn

JS:   console.error("err")
来源：http://tc.chemitech.net.cn

TS:   console.error("err")
来源：http://gv.szxytkj.cn

Java: System.err.println("err")
来源：http://rx.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xb.huixinmuqiang.cn

Ruby: warn "err"
来源：http://mi.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://he.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://ie.colortex.cn

Py:   if __name__ == "__main__":
来源：http://sh.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ck.nszjky.cn

JS:   require.main === module
来源：http://zn.szxytkj.cn

TS:   require.main === module
来源：http://ox.9csxet.cn

Java: public static void main(String[] args)
来源：http://px.bookmarksfly.cn

Go:   func main()
来源：http://oi.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yu.521024.cn

C#:   static void Main(string[] args)
来源：http://ks.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://nf.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://ot.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://mi.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://cy.lnxyls.cn

TS:   process.platform;  process.version
来源：http://sh.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bx.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yi.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nk.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ws.haigaiapp.cn

================================================================================
来源：http://wp.newstarts.cn

N. 数据结构与算法
来源：http://pw.yuexingan06.cn

================================================================================
来源：http://ak.asd995.cn

[N01] 二分查找（有序数组）
来源：http://yx.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ep.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://th.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jc.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vo.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://in.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pd.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ze.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://im.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ss.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sd.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rq.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://st.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://xk.wgjwhj.cn

Ruby: arr.sort
来源：http://zz.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ge.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://eo.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vn.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://ur.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ib.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fp.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lj.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xq.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gq.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xh.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://aq.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ib.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bh.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hc.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://db.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://je.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ni.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hg.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zq.nszjky.cn

[N05] 最大公约数
来源：http://uj.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://dm.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cr.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://du.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vh.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cj.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://no.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://qo.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://se.shxzukj.cn

[N06] 判断回文字符串
来源：http://yt.9csxet.cn

Py:   s == s[::-1]
来源：http://mr.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://in.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://gl.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://vm.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ni.colortex.cn

Go:   // 双指针从两端比较
来源：http://ql.szsharing.cn

Ruby: s == s.reverse
来源：http://xn.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bj.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://fd.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ir.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pa.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hb.521024.cn

TS:   // 手写 Map<string, number>
来源：http://ah.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://he.jianghongdianzi.cn


<!-- 参考信息 -->