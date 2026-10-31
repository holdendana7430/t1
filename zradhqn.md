代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ia.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bf.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vi.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bh.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://km.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pb.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bl.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://zg.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hh.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://et.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dl.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mb.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ko.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bs.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ok.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vp.jctech888.com.cn

================================================================================
来源：http://xt.hahajie.cn

K. JSON 与序列化
来源：http://jn.9csxet.cn

================================================================================
来源：http://yf.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://rr.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gl.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zo.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://xh.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://gs.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://to.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://xc.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ve.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pd.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://fa.huixiangedu.cn

Py:   json.loads(s)
来源：http://nr.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://er.colortex.cn

JS:   JSON.parse(s)
来源：http://cr.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://rb.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://by.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://kt.colortex.cn

Ruby: JSON.parse(s)
来源：http://ls.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ep.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ed.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cv.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ty.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wf.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qd.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qv.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fh.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kt.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sj.bookmarksfly.cn

[K04] 读取 JSON 文件
来源：http://mg.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vt.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cg.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xu.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jd.shtwfgs.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mw.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jp.wgjwhj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jb.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rt.wgjwhj.cn

[K05] 深拷贝对象
来源：http://mf.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://ze.jianghongdianzi.cn

PHP:  unserialize(serialize($obj));
来源：http://my.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ni.nszjky.cn

TS:   structuredClone(obj)
来源：http://gj.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sn.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jg.shtwfgs.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lm.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wq.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://le.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://la.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nj.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xd.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qq.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xg.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ev.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lq.yuntaijiaju.cn

[K07] 进制转换
来源：http://dc.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://an.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wh.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ny.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cz.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fx.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wl.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ov.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ff.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://cb.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://gg.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kv.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://qq.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://iv.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aa.colortex.cn

Go:   encoding/gob
来源：http://wg.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://cd.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zh.huanxung.cn

================================================================================
来源：http://wl.yuntaijiaju.cn

L. 网络请求
来源：http://bf.9csxet.cn

================================================================================
来源：http://hg.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://cl.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://km.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fq.asd995.cn

JS:   await fetch(url)
来源：http://hi.chemitech.net.cn

TS:   await fetch(url)
来源：http://il.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ur.521024.cn

Go:   resp, err := http.Get(url)
来源：http://hu.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tb.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vg.szsharing.cn

[L02] 发送 POST JSON
来源：http://jn.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://if.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uh.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qd.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ep.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iw.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gu.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tx.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ny.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://tp.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://py.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uv.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yl.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wz.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ql.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ja.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lf.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vy.huixiangedu.cn

[L04] 设置超时
来源：http://yg.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://sr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xa.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uy.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sv.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rd.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rj.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xj.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gc.hahajie.cn

[L05] 上传文件（multipart）
来源：http://rv.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://us.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rs.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://er.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uu.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rd.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://il.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ss.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tj.9csxet.cn

[L06] 解析响应为 JSON
来源：http://zf.haigaiapp.cn

Py:   resp.json()
来源：http://ak.nicolike.cn

PHP:  json_decode($body, true);
来源：http://te.hahajie.cn

JS:   await resp.json()
来源：http://ix.shxzskj.cn

TS:   await resp.json()
来源：http://gm.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xo.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sq.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://nd.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xb.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://kg.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ca.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oc.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://nm.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://cw.newstarts.cn

Java: resp.statusCode()
来源：http://gd.lnxyls.cn

Go:   resp.StatusCode
来源：http://cr.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://dh.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://mu.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://vv.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://od.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://yc.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://im.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yi.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ak.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://za.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tc.gzmigu.cn

================================================================================
来源：http://tw.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ow.yuexingan06.cn

================================================================================
来源：http://uf.bjjhwx.cn

[M01] 读取命令行参数
来源：http://ov.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://kx.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://hj.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://hx.nicolike.cn

TS:   process.argv.slice(2)
来源：http://ge.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://rc.chemitech.net.cn

Go:   os.Args[1:]
来源：http://kk.bjjhwx.cn

Ruby: ARGV
来源：http://ts.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://mg.muxihuayi.cn

[M02] 读取环境变量
来源：http://nx.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://sb.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rn.colortex.cn

JS:   process.env.HOME
来源：http://zt.shtwfgs.cn

TS:   process.env.HOME
来源：http://ak.521024.cn

Java: System.getenv("HOME")
来源：http://lt.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zt.huanxung.cn

Ruby: ENV["HOME"]
来源：http://iq.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xf.haigaiapp.cn

[M03] 执行外部命令
来源：http://bw.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hc.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://km.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wq.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yg.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uu.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zv.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ya.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://dl.nszjky.cn

[M04] 获取当前工作目录
来源：http://pj.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://aj.szsharing.cn

PHP:  getcwd();
来源：http://cw.gzmigu.cn

JS:   process.cwd()
来源：http://xh.colortex.cn

TS:   process.cwd()
来源：http://np.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ft.haigaiapp.cn

Go:   os.Getwd()
来源：http://yn.nicolike.cn

Ruby: Dir.pwd
来源：http://ty.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gn.bookmarksfly.cn

[M05] 设置退出码
来源：http://ub.hahajie.cn

Py:   sys.exit(1)
来源：http://vf.9csxet.cn

PHP:  exit(1);
来源：http://st.hnjuh.cn

JS:   process.exit(1)
来源：http://kc.muxihuayi.cn

TS:   process.exit(1)
来源：http://uz.chemitech.net.cn

Java: System.exit(1)
来源：http://jc.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://bi.yuntaijiaju.cn

Ruby: exit 1
来源：http://yp.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qq.newstarts.cn

[M06] 向标准错误输出
来源：http://qg.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://vj.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aj.haigaiapp.cn

JS:   console.error("err")
来源：http://lk.newstarts.cn

TS:   console.error("err")
来源：http://np.9csxet.cn

Java: System.err.println("err")
来源：http://ef.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uv.shxzskj.cn

Ruby: warn "err"
来源：http://db.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://oy.jctech888.com.cn

[M07] 判断是否为主入口
来源：http://jr.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://ok.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eb.9csxet.cn

JS:   require.main === module
来源：http://tp.9csxet.cn

TS:   require.main === module
来源：http://wb.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://lv.newstarts.cn

Go:   func main()
来源：http://vh.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jg.hahajie.cn

C#:   static void Main(string[] args)
来源：http://rj.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://zg.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://wj.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dd.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://cf.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ey.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nz.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ex.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vy.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bn.bookmarksfly.cn

================================================================================
来源：http://tv.nicolike.cn

N. 数据结构与算法
来源：http://hh.colortex.cn

================================================================================
来源：http://ez.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://mn.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sn.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://du.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jy.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bn.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jy.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://oy.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oz.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mn.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://xr.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://gw.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mi.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qb.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ia.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ys.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://vb.9csxet.cn

Ruby: arr.sort
来源：http://vo.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ev.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://rt.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ql.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://vi.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cm.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dg.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vp.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://az.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yx.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vk.huixiangedu.cn

[N04] 斐波那契数列
来源：http://hf.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gv.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bi.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cm.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nc.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fc.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jw.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kl.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ty.colortex.cn

[N05] 最大公约数
来源：http://my.yuntaijiaju.cn

Py:   math.gcd(a, b)
来源：http://uh.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fo.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sy.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://an.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nn.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xn.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ri.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sd.bjjhwx.cn

[N06] 判断回文字符串
来源：http://ty.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://xs.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://jg.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://iu.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://zf.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bl.9csxet.cn

Go:   // 双指针从两端比较
来源：http://op.shtwfgs.cn

Ruby: s == s.reverse
来源：http://ik.muxihuayi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dm.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://db.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xh.szxytkj.cn


<!-- 参考信息 -->