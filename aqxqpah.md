代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ww.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yw.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jz.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zw.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sr.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yk.shxzskj.cn

[J09] 时区处理
来源：http://my.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jy.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pg.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bj.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sy.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yz.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ju.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wn.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://lj.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://df.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pb.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gh.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fq.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eb.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mx.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hu.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vu.chemitech.net.cn

================================================================================
来源：http://bj.bjjhwx.cn

K. JSON 与序列化
来源：http://ro.bookmarksfly.cn

================================================================================
来源：http://yu.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://ih.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sn.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gw.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://hs.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://mk.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nt.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://re.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qe.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mr.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://wk.wgjwhj.cn

Py:   json.loads(s)
来源：http://rz.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sx.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://oc.hnjuh.cn

TS:   JSON.parse(s)
来源：http://ga.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vq.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://ws.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://vb.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ec.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://gg.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tn.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mo.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bw.szsharing.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://no.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aq.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ql.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uc.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bw.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://rx.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tz.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dy.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ke.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mg.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kz.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://he.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xz.nszjky.cn

[K05] 深拷贝对象
来源：http://lk.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://tw.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://ub.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ye.9csxet.cn

TS:   structuredClone(obj)
来源：http://ay.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fn.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mn.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qy.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oa.521024.cn

[K06] 解析 URL 查询串
来源：http://pu.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sj.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bh.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tm.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uy.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ib.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gk.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sa.muxihuayi.cn

[K07] 进制转换
来源：http://my.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ug.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wq.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wo.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vb.muxihuayi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fe.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lv.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kg.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eh.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://dr.asd995.cn

Py:   pickle.dumps(obj)
来源：http://wl.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uq.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://rp.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://qk.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kd.hnjuh.cn

Go:   encoding/gob
来源：http://dk.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://vr.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vf.lnxyls.cn

================================================================================
来源：http://oh.yuntaijiaju.cn

L. 网络请求
来源：http://wc.bjjhwx.cn

================================================================================
来源：http://fu.gzmigu.cn

[L01] 发送 GET 请求
来源：http://yk.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ug.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pg.nicolike.cn

JS:   await fetch(url)
来源：http://tg.huixiangedu.cn

TS:   await fetch(url)
来源：http://fk.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sc.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://iv.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pq.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iz.521024.cn

[L02] 发送 POST JSON
来源：http://eq.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eo.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xb.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hv.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://at.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tm.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://up.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fl.szxytkj.cn

[L03] 设置自定义请求头
来源：http://yk.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://od.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kq.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mq.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sn.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://of.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xy.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sb.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zp.asd995.cn

[L04] 设置超时
来源：http://ki.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ke.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zm.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://do.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hj.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ei.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bq.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ma.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://in.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://dm.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rk.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fh.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://md.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zz.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cc.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fx.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wv.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ku.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://my.bjjhwx.cn

Py:   resp.json()
来源：http://xm.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://lf.shxzskj.cn

JS:   await resp.json()
来源：http://tf.wgjwhj.cn

TS:   await resp.json()
来源：http://ma.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wh.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fm.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://sd.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ho.521024.cn

[L07] 处理 HTTP 状态码
来源：http://pa.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yy.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mm.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://ws.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://sh.shtwfgs.cn

Java: resp.statusCode()
来源：http://vn.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://wx.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://yi.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://cj.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://ck.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ub.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ds.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lp.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kp.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cw.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sc.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zp.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kn.9csxet.cn

================================================================================
来源：http://nd.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://is.szsharing.cn

================================================================================
来源：http://cf.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://qy.shxzskj.cn

Py:   sys.argv[1:]
来源：http://yp.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://uw.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://oa.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://lh.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://hm.szsharing.cn

Go:   os.Args[1:]
来源：http://zf.panjiajie.cn

Ruby: ARGV
来源：http://ek.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://td.nicolike.cn

[M02] 读取环境变量
来源：http://eq.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://id.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://el.panjiajie.cn

JS:   process.env.HOME
来源：http://js.yuexingan06.cn

TS:   process.env.HOME
来源：http://pw.hnjuh.cn

Java: System.getenv("HOME")
来源：http://pm.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://th.huanxung.cn

Ruby: ENV["HOME"]
来源：http://sw.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ns.hahajie.cn

[M03] 执行外部命令
来源：http://fn.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zt.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fe.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ut.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cz.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pp.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xf.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ev.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://ng.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://eo.wgjwhj.cn

Py:   os.getcwd()
来源：http://tm.bjjhwx.cn

PHP:  getcwd();
来源：http://il.hahajie.cn

JS:   process.cwd()
来源：http://fs.chemitech.net.cn

TS:   process.cwd()
来源：http://oa.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://gy.shxzukj.cn

Go:   os.Getwd()
来源：http://xo.nszjky.cn

Ruby: Dir.pwd
来源：http://ij.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://my.szsharing.cn

[M05] 设置退出码
来源：http://uv.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://ay.huanxung.cn

PHP:  exit(1);
来源：http://ob.hnjuh.cn

JS:   process.exit(1)
来源：http://ha.shtwfgs.cn

TS:   process.exit(1)
来源：http://vk.haigaiapp.cn

Java: System.exit(1)
来源：http://wr.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://fx.szxytkj.cn

Ruby: exit 1
来源：http://lp.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hx.hnjuh.cn

[M06] 向标准错误输出
来源：http://yw.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://kr.521024.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jf.bookmarksfly.cn

JS:   console.error("err")
来源：http://wx.yuntaijiaju.cn

TS:   console.error("err")
来源：http://mb.szxytkj.cn

Java: System.err.println("err")
来源：http://nt.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ik.hahajie.cn

Ruby: warn "err"
来源：http://vd.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://zj.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://dr.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://jr.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zu.szsharing.cn

JS:   require.main === module
来源：http://vg.shxzukj.cn

TS:   require.main === module
来源：http://xy.newstarts.cn

Java: public static void main(String[] args)
来源：http://lb.yuexingan06.cn

Go:   func main()
来源：http://ht.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://we.colortex.cn

C#:   static void Main(string[] args)
来源：http://tc.asd995.cn

[M08] 获取系统与运行时信息
来源：http://bj.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://kl.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://bl.panjiajie.cn

JS:   process.platform;  process.version
来源：http://yo.nszjky.cn

TS:   process.platform;  process.version
来源：http://dc.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kj.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ih.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fe.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lx.haigaiapp.cn

================================================================================
来源：http://kx.hnjuh.cn

N. 数据结构与算法
来源：http://mz.shxzskj.cn

================================================================================
来源：http://wd.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://fu.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ae.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eq.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://my.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://of.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://kp.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cq.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tv.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://qt.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://zk.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vc.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://da.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ro.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wf.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://xu.gzmigu.cn

Ruby: arr.sort
来源：http://cw.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kx.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://uq.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://km.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://gx.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gi.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wj.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qd.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gf.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lh.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wh.panjiajie.cn

[N04] 斐波那契数列
来源：http://ap.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fc.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mc.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://be.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zh.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bf.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qa.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zv.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://la.9csxet.cn

[N05] 最大公约数
来源：http://df.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://zy.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yz.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yv.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bt.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://os.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ce.szxytkj.cn

Ruby: a.gcd(b)
来源：http://te.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vy.hahajie.cn

[N06] 判断回文字符串
来源：http://rk.szxytkj.cn

Py:   s == s[::-1]
来源：http://xc.szsharing.cn

PHP:  $s === strrev($s);
来源：http://zy.bookmarksfly.cn


<!-- 参考信息 -->