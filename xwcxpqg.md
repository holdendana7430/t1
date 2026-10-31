代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zd.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yp.haigaiapp.cn

[J09] 时区处理
来源：http://nu.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nx.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://po.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fz.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vh.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ot.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ys.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oo.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ph.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://ku.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ox.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fc.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vv.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jb.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rf.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ts.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lf.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rc.nszjky.cn

================================================================================
来源：http://yo.9csxet.cn

K. JSON 与序列化
来源：http://zs.hnjuh.cn

================================================================================
来源：http://ze.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://zy.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yq.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yr.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://pl.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://ff.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ja.asd995.cn

Go:   json.Marshal(obj)
来源：http://ys.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ev.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sd.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://gi.newstarts.cn

Py:   json.loads(s)
来源：http://gp.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rp.panjiajie.cn

JS:   JSON.parse(s)
来源：http://hs.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://cr.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fk.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ga.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://fx.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dy.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://qv.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zs.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oy.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eo.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ef.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://si.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nl.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jr.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qp.nicolike.cn

[K04] 读取 JSON 文件
来源：http://xa.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qq.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vg.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pz.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gl.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qo.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ti.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gb.521024.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pm.9csxet.cn

[K05] 深拷贝对象
来源：http://ba.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://mo.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://wd.9csxet.cn

JS:   structuredClone(obj)
来源：http://sh.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://tg.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kb.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qk.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ir.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dh.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://pi.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gl.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rd.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yw.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ln.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://me.yuexingan06.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jo.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gb.chemitech.net.cn

[K07] 进制转换
来源：http://sq.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://db.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ag.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cn.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rs.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hj.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vw.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uh.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ld.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://hk.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://ua.9csxet.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://en.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://vp.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://mv.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ax.bjjhwx.cn

Go:   encoding/gob
来源：http://gx.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://xj.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cy.gzmigu.cn

================================================================================
来源：http://wg.jctech888.com.cn

L. 网络请求
来源：http://tq.huixiangedu.cn

================================================================================
来源：http://cw.9csxet.cn

[L01] 发送 GET 请求
来源：http://gs.wgjwhj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hd.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gb.nszjky.cn

JS:   await fetch(url)
来源：http://ny.bjjhwx.cn

TS:   await fetch(url)
来源：http://en.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hf.521024.cn

Go:   resp, err := http.Get(url)
来源：http://uc.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xl.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mv.szxytkj.cn

[L02] 发送 POST JSON
来源：http://rr.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cm.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lc.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://df.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://go.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jq.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ap.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fa.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dr.huanxung.cn

[L03] 设置自定义请求头
来源：http://mg.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ng.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ly.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yu.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yc.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gm.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gr.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qs.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wt.shxzukj.cn

[L04] 设置超时
来源：http://eb.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://kx.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ju.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nj.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ud.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sn.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xi.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wn.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kx.newstarts.cn

[L05] 上传文件（multipart）
来源：http://pe.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ea.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kt.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dk.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gs.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xc.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wa.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pk.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qu.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://ov.jianghongdianzi.cn

Py:   resp.json()
来源：http://mc.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ln.wgjwhj.cn

JS:   await resp.json()
来源：http://mw.9csxet.cn

TS:   await resp.json()
来源：http://vn.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pg.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fy.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://bj.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bk.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://kv.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cg.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ra.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://it.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://ko.gzmigu.cn

Java: resp.statusCode()
来源：http://ng.muxihuayi.cn

Go:   resp.StatusCode
来源：http://se.nicolike.cn

Ruby: resp.code.to_i
来源：http://vk.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://hd.lnxyls.cn

[L08] 并发请求多个地址
来源：http://yv.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yq.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://al.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vd.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fg.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uc.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fy.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nx.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qj.wgjwhj.cn

================================================================================
来源：http://wk.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://ix.yuntaijiaju.cn

================================================================================
来源：http://ms.bjjhwx.cn

[M01] 读取命令行参数
来源：http://pr.nszjky.cn

Py:   sys.argv[1:]
来源：http://pq.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://fg.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://zb.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ut.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://rg.gzmigu.cn

Go:   os.Args[1:]
来源：http://zo.haigaiapp.cn

Ruby: ARGV
来源：http://kf.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://qd.jianghongdianzi.cn

[M02] 读取环境变量
来源：http://sl.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://ee.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aq.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://rc.bjjhwx.cn

TS:   process.env.HOME
来源：http://dc.panjiajie.cn

Java: System.getenv("HOME")
来源：http://to.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://av.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://is.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fh.panjiajie.cn

[M03] 执行外部命令
来源：http://za.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tp.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://re.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rr.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tr.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nl.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zt.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tj.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://ku.9csxet.cn

[M04] 获取当前工作目录
来源：http://sh.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://gq.hnjuh.cn

PHP:  getcwd();
来源：http://qj.newstarts.cn

JS:   process.cwd()
来源：http://wr.shxzukj.cn

TS:   process.cwd()
来源：http://vq.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://ew.szxytkj.cn

Go:   os.Getwd()
来源：http://yu.shxzskj.cn

Ruby: Dir.pwd
来源：http://yh.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://co.9csxet.cn

[M05] 设置退出码
来源：http://jt.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://mc.gzmigu.cn

PHP:  exit(1);
来源：http://hq.wgjwhj.cn

JS:   process.exit(1)
来源：http://ot.shxzskj.cn

TS:   process.exit(1)
来源：http://ef.haigaiapp.cn

Java: System.exit(1)
来源：http://os.hnjuh.cn

Go:   os.Exit(1)
来源：http://fe.bjjhwx.cn

Ruby: exit 1
来源：http://zm.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jj.jctech888.com.cn

[M06] 向标准错误输出
来源：http://oa.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://or.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ka.huixinmuqiang.cn

JS:   console.error("err")
来源：http://jb.bookmarksfly.cn

TS:   console.error("err")
来源：http://hs.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://we.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yp.nszjky.cn

Ruby: warn "err"
来源：http://py.jctech888.com.cn

C#:   Console.Error.WriteLine("err")
来源：http://mn.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://zx.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://zf.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mz.colortex.cn

JS:   require.main === module
来源：http://in.shtwfgs.cn

TS:   require.main === module
来源：http://sy.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://zl.wgjwhj.cn

Go:   func main()
来源：http://je.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ao.nszjky.cn

C#:   static void Main(string[] args)
来源：http://yv.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://zm.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://gl.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://ze.nicolike.cn

JS:   process.platform;  process.version
来源：http://tl.szxytkj.cn

TS:   process.platform;  process.version
来源：http://ll.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gt.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gi.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ns.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vi.jctech888.com.cn

================================================================================
来源：http://pf.chemitech.net.cn

N. 数据结构与算法
来源：http://uz.shxzukj.cn

================================================================================
来源：http://xh.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://mv.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yb.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ez.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hs.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dd.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pb.panjiajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://vi.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eq.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rh.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://hf.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://sj.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vh.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rb.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ei.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mf.hahajie.cn

Go:   slices.Sort(arr)
来源：http://ms.jianghongdianzi.cn

Ruby: arr.sort
来源：http://zl.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tp.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://im.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nc.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://ca.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yx.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cy.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://be.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yp.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mw.shxzskj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ip.yuexingan06.cn

[N04] 斐波那契数列
来源：http://dg.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uq.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ld.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yd.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kv.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tx.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://go.huanxung.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rn.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fc.szsharing.cn

[N05] 最大公约数
来源：http://lo.9csxet.cn

Py:   math.gcd(a, b)
来源：http://yz.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mm.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wu.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qs.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kb.hnjuh.cn

Ruby: a.gcd(b)
来源：http://zq.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yz.szsharing.cn

[N06] 判断回文字符串
来源：http://dg.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://mb.nszjky.cn

PHP:  $s === strrev($s);
来源：http://bk.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://kp.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://kj.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kv.asd995.cn

Go:   // 双指针从两端比较
来源：http://wi.bookmarksfly.cn


<!-- 参考信息 -->