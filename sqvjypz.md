代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zv.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pb.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vf.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://qj.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jh.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://re.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zm.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cu.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zm.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fo.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rj.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://us.hnjuh.cn

================================================================================
来源：http://pe.9csxet.cn

K. JSON 与序列化
来源：http://qy.nszjky.cn

================================================================================
来源：http://ts.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://zz.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xx.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hv.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://qx.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://ft.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jj.huanxung.cn

Go:   json.Marshal(obj)
来源：http://sj.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fg.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fg.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://vy.bookmarksfly.cn

Py:   json.loads(s)
来源：http://wl.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yx.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://kf.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://zl.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fo.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mh.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://em.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zl.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://nw.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tx.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kk.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://az.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kh.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sx.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://af.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uw.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ct.colortex.cn

[K04] 读取 JSON 文件
来源：http://dh.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pr.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bd.521024.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sd.shxzskj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rv.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://os.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mw.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nq.colortex.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tm.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://xe.huanxung.cn

Py:   copy.deepcopy(obj)
来源：http://zd.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://dk.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://qb.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://mz.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://te.bjjhwx.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hk.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jd.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vb.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://ej.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kd.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hx.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ez.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fs.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ps.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yu.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wg.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tw.huanxung.cn

[K07] 进制转换
来源：http://ly.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ry.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eu.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hr.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wj.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fc.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ew.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nd.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uf.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://xw.asd995.cn

Py:   pickle.dumps(obj)
来源：http://nu.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ny.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://bj.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://lx.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wu.lnxyls.cn

Go:   encoding/gob
来源：http://ed.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://zy.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cc.9csxet.cn

================================================================================
来源：http://pt.9csxet.cn

L. 网络请求
来源：http://ar.9csxet.cn

================================================================================
来源：http://gf.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://jw.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://au.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kh.huixiangedu.cn

JS:   await fetch(url)
来源：http://am.shxzskj.cn

TS:   await fetch(url)
来源：http://ey.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zp.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://wr.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fg.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ng.muxihuayi.cn

[L02] 发送 POST JSON
来源：http://gy.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jv.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://db.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cg.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ua.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ej.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nu.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xk.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rq.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://ax.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://br.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jn.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kb.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ov.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qf.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bz.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xm.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cp.9csxet.cn

[L04] 设置超时
来源：http://ao.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://gq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vc.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.wgjwhj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nc.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rb.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mm.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iq.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oa.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://mk.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uq.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tk.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vh.yuexingan06.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jt.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zv.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cs.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ta.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yz.nszjky.cn

[L06] 解析响应为 JSON
来源：http://li.nszjky.cn

Py:   resp.json()
来源：http://qc.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://tj.hnjuh.cn

JS:   await resp.json()
来源：http://yc.gzmigu.cn

TS:   await resp.json()
来源：http://ko.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fz.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zq.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://wl.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zy.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://of.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cg.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://jr.colortex.cn

TS:   resp.ok;  resp.status
来源：http://bm.asd995.cn

Java: resp.statusCode()
来源：http://tv.nicolike.cn

Go:   resp.StatusCode
来源：http://tf.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://wh.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://jd.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://pb.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tw.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://vz.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ws.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lk.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://py.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hq.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gu.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ce.wgjwhj.cn

================================================================================
来源：http://gn.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://sm.newstarts.cn

================================================================================
来源：http://ij.szxytkj.cn

[M01] 读取命令行参数
来源：http://of.nszjky.cn

Py:   sys.argv[1:]
来源：http://oq.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://va.hahajie.cn

JS:   process.argv.slice(2)
来源：http://vo.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://py.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://hd.bjjhwx.cn

Go:   os.Args[1:]
来源：http://sy.panjiajie.cn

Ruby: ARGV
来源：http://ut.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://fk.bjjhwx.cn

[M02] 读取环境变量
来源：http://md.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://we.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ec.newstarts.cn

JS:   process.env.HOME
来源：http://ap.haigaiapp.cn

TS:   process.env.HOME
来源：http://wr.nicolike.cn

Java: System.getenv("HOME")
来源：http://yq.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://us.nszjky.cn

Ruby: ENV["HOME"]
来源：http://ly.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tu.shxzukj.cn

[M03] 执行外部命令
来源：http://dn.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hu.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fs.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://li.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qn.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wp.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kx.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hv.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://vs.newstarts.cn

[M04] 获取当前工作目录
来源：http://lu.muxihuayi.cn

Py:   os.getcwd()
来源：http://eo.yuexingan06.cn

PHP:  getcwd();
来源：http://te.colortex.cn

JS:   process.cwd()
来源：http://yu.huixiangedu.cn

TS:   process.cwd()
来源：http://dr.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://jy.shtwfgs.cn

Go:   os.Getwd()
来源：http://zq.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ox.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mu.jianghongdianzi.cn

[M05] 设置退出码
来源：http://yh.huanxung.cn

Py:   sys.exit(1)
来源：http://pd.chemitech.net.cn

PHP:  exit(1);
来源：http://yz.colortex.cn

JS:   process.exit(1)
来源：http://qv.szxytkj.cn

TS:   process.exit(1)
来源：http://cf.nszjky.cn

Java: System.exit(1)
来源：http://sr.newstarts.cn

Go:   os.Exit(1)
来源：http://zl.huixinmuqiang.cn

Ruby: exit 1
来源：http://jz.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gu.shxzukj.cn

[M06] 向标准错误输出
来源：http://kc.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://uv.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sz.bjjhwx.cn

JS:   console.error("err")
来源：http://jd.lnxyls.cn

TS:   console.error("err")
来源：http://hr.yuexingan06.cn

Java: System.err.println("err")
来源：http://we.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zu.panjiajie.cn

Ruby: warn "err"
来源：http://be.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://uk.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://cc.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://go.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ve.gzmigu.cn

JS:   require.main === module
来源：http://on.panjiajie.cn

TS:   require.main === module
来源：http://vs.huanxung.cn

Java: public static void main(String[] args)
来源：http://gu.bjjhwx.cn

Go:   func main()
来源：http://ap.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jk.colortex.cn

C#:   static void Main(string[] args)
来源：http://we.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://rb.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://nr.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://zu.nszjky.cn

JS:   process.platform;  process.version
来源：http://jm.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://jb.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ny.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lv.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sl.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.nszjky.cn

================================================================================
来源：http://jw.lnxyls.cn

N. 数据结构与算法
来源：http://jv.huixiangedu.cn

================================================================================
来源：http://af.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://cq.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sd.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mb.jianghongdianzi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fj.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bp.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yb.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://dk.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ux.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yb.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ri.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://gk.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lu.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ug.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ye.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ye.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://zo.521024.cn

Ruby: arr.sort
来源：http://ef.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vj.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://ao.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xi.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://ra.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pn.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tg.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yb.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mi.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zs.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oz.jctech888.com.cn

[N04] 斐波那契数列
来源：http://gh.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pt.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nh.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ik.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yl.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ft.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dv.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tv.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aj.chemitech.net.cn

[N05] 最大公约数
来源：http://at.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://hp.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ma.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mn.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uz.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zy.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lp.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://dh.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pv.shxzskj.cn

[N06] 判断回文字符串
来源：http://un.jctech888.com.cn

Py:   s == s[::-1]
来源：http://ri.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://yw.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://wb.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://vv.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://it.521024.cn

Go:   // 双指针从两端比较
来源：http://wy.szxytkj.cn

Ruby: s == s.reverse
来源：http://tg.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yx.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://ij.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xp.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iw.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ia.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://gb.hahajie.cn

Java: // 手写 HashMap
来源：http://wi.521024.cn


<!-- 参考信息 -->