代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://on.colortex.cn

[J08] 提取年月日与星期
来源：http://dl.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yt.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zl.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://al.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://te.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xi.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zb.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lu.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dz.shxzukj.cn

[J09] 时区处理
来源：http://yn.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uj.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rz.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hg.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ha.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gj.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://du.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sw.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://mn.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kb.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uw.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ie.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://re.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rs.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ro.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://io.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dz.lnxyls.cn

================================================================================
来源：http://me.yuexingan06.cn

K. JSON 与序列化
来源：http://gm.huanxung.cn

================================================================================
来源：http://kd.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://zv.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ql.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tj.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ke.asd995.cn

TS:   JSON.stringify(obj)
来源：http://xv.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vt.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://aq.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jh.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dl.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://dx.haigaiapp.cn

Py:   json.loads(s)
来源：http://fl.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mi.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://ae.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://bt.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ml.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://hu.hahajie.cn

Ruby: JSON.parse(s)
来源：http://bj.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nl.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tz.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://py.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rn.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oq.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://al.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lc.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zt.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ry.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://im.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fv.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ca.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ra.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bu.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zj.jctech888.com.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rn.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ny.bjjhwx.cn

[K05] 深拷贝对象
来源：http://ob.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://eq.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://rw.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://gr.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://js.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ql.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fc.shxzukj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nf.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mf.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://qk.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yj.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eo.shxzukj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ib.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tq.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iy.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mo.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jt.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mb.shxzukj.cn

[K07] 进制转换
来源：http://dn.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://im.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ey.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tp.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tq.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ri.gzmigu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ct.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://se.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nf.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://vd.colortex.cn

Py:   pickle.dumps(obj)
来源：http://za.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dy.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://mf.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://jb.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zy.jctech888.com.cn

Go:   encoding/gob
来源：http://pd.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://qe.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rz.hahajie.cn

================================================================================
来源：http://tv.gzmigu.cn

L. 网络请求
来源：http://ap.asd995.cn

================================================================================
来源：http://qy.shxzskj.cn

[L01] 发送 GET 请求
来源：http://ju.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hh.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mz.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://zj.yuexingan06.cn

TS:   await fetch(url)
来源：http://ur.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ey.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://ja.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rf.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uh.9csxet.cn

[L02] 发送 POST JSON
来源：http://fn.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xq.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://of.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ub.yuntaijiaju.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bv.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ly.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ha.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ed.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qr.nicolike.cn

[L03] 设置自定义请求头
来源：http://kz.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fl.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mv.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rn.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oo.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kk.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pa.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qi.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ig.wgjwhj.cn

[L04] 设置超时
来源：http://ro.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://nw.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ic.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xe.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ua.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://md.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zs.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pm.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sz.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://ir.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://da.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ej.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lz.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jt.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://am.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ke.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bd.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gn.asd995.cn

[L06] 解析响应为 JSON
来源：http://dt.nszjky.cn

Py:   resp.json()
来源：http://wi.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://lv.huixinmuqiang.cn

JS:   await resp.json()
来源：http://al.szsharing.cn

TS:   await resp.json()
来源：http://yx.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kj.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ub.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://zw.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sq.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://dn.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ws.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kg.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://ek.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://sv.szsharing.cn

Java: resp.statusCode()
来源：http://op.lnxyls.cn

Go:   resp.StatusCode
来源：http://af.panjiajie.cn

Ruby: resp.code.to_i
来源：http://hx.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://tf.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://fm.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xc.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://wg.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zd.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vy.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gk.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://db.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://or.szxytkj.cn

================================================================================
来源：http://up.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ri.szxytkj.cn

================================================================================
来源：http://hd.huixiangedu.cn

[M01] 读取命令行参数
来源：http://kx.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://se.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://ss.521024.cn

JS:   process.argv.slice(2)
来源：http://gj.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ck.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://po.shtwfgs.cn

Go:   os.Args[1:]
来源：http://nt.jctech888.com.cn

Ruby: ARGV
来源：http://ty.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://rw.nszjky.cn

[M02] 读取环境变量
来源：http://qo.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://pw.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://km.panjiajie.cn

JS:   process.env.HOME
来源：http://kf.colortex.cn

TS:   process.env.HOME
来源：http://tf.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://eg.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ti.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://ze.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zh.szxytkj.cn

[M03] 执行外部命令
来源：http://ov.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ee.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ks.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jk.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ej.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ds.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uf.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://co.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://vp.szsharing.cn

[M04] 获取当前工作目录
来源：http://ee.huixiangedu.cn

Py:   os.getcwd()
来源：http://me.bjjhwx.cn

PHP:  getcwd();
来源：http://si.colortex.cn

JS:   process.cwd()
来源：http://pn.wgjwhj.cn

TS:   process.cwd()
来源：http://ui.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://gr.bjjhwx.cn

Go:   os.Getwd()
来源：http://hr.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ew.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ya.huixiangedu.cn

[M05] 设置退出码
来源：http://uj.chemitech.net.cn

Py:   sys.exit(1)
来源：http://xd.newstarts.cn

PHP:  exit(1);
来源：http://dd.nszjky.cn

JS:   process.exit(1)
来源：http://vt.muxihuayi.cn

TS:   process.exit(1)
来源：http://cq.muxihuayi.cn

Java: System.exit(1)
来源：http://wv.chemitech.net.cn

Go:   os.Exit(1)
来源：http://kk.shxzskj.cn

Ruby: exit 1
来源：http://cu.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cc.newstarts.cn

[M06] 向标准错误输出
来源：http://af.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://tn.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ef.9csxet.cn

JS:   console.error("err")
来源：http://fh.chemitech.net.cn

TS:   console.error("err")
来源：http://bj.yuexingan06.cn

Java: System.err.println("err")
来源：http://ra.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jy.muxihuayi.cn

Ruby: warn "err"
来源：http://fz.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ax.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://bb.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://pq.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oi.bookmarksfly.cn

JS:   require.main === module
来源：http://ex.jianghongdianzi.cn

TS:   require.main === module
来源：http://yc.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://kk.lnxyls.cn

Go:   func main()
来源：http://ex.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tv.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://hv.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://ln.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ky.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://qq.shxzskj.cn

JS:   process.platform;  process.version
来源：http://cb.asd995.cn

TS:   process.platform;  process.version
来源：http://ee.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pu.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zy.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eg.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ll.nszjky.cn

================================================================================
来源：http://eb.szxytkj.cn

N. 数据结构与算法
来源：http://ba.shxzukj.cn

================================================================================
来源：http://se.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://ip.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nl.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://em.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pz.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nm.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uz.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://ht.wgjwhj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bi.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pp.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://rn.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jf.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bj.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fg.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fg.newstarts.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fp.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://sx.jctech888.com.cn

Ruby: arr.sort
来源：http://yz.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ym.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://le.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://le.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://er.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sw.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://js.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fk.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ma.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rq.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xk.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://xm.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bl.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yl.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qr.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yr.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://od.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ae.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hb.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lr.newstarts.cn

[N05] 最大公约数
来源：http://kh.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://rb.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iy.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wf.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xd.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ny.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qw.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://eh.colortex.cn


<!-- 参考信息 -->