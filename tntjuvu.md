代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://bh.panjiajie.cn

[J08] 提取年月日与星期
来源：http://mv.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vd.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ne.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rx.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bk.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cw.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tu.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uf.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lg.shtwfgs.cn

[J09] 时区处理
来源：http://vn.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xh.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ru.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xq.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ie.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bi.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://en.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://al.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ch.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://qt.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://za.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ye.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xv.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uc.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rf.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tf.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fe.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gx.szxytkj.cn

================================================================================
来源：http://iz.521024.cn

K. JSON 与序列化
来源：http://bz.chemitech.net.cn

================================================================================
来源：http://fl.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://tj.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vo.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kc.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ky.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://qr.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tt.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://vn.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zc.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jt.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://wp.colortex.cn

Py:   json.loads(s)
来源：http://mh.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://al.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://de.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://tr.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ge.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://hu.colortex.cn

Ruby: JSON.parse(s)
来源：http://yc.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gq.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://nj.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sq.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gv.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ps.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ao.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yh.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rh.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sz.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rp.panjiajie.cn

[K04] 读取 JSON 文件
来源：http://xc.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ln.shtwfgs.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ef.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mo.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cd.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bx.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ci.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://of.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jz.chemitech.net.cn

[K05] 深拷贝对象
来源：http://gs.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://js.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://em.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://pl.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://bv.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sf.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xi.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sp.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pq.szsharing.cn

[K06] 解析 URL 查询串
来源：http://pz.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nr.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qj.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yh.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oe.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ci.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sn.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://id.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cx.bookmarksfly.cn

[K07] 进制转换
来源：http://ik.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hp.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://db.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tw.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cd.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ca.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zc.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://to.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uh.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://qv.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://rt.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xn.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://td.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ti.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ff.hnjuh.cn

Go:   encoding/gob
来源：http://kl.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://bl.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ij.szsharing.cn

================================================================================
来源：http://rw.hahajie.cn

L. 网络请求
来源：http://rg.muxihuayi.cn

================================================================================
来源：http://cx.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://gf.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gv.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://im.panjiajie.cn

JS:   await fetch(url)
来源：http://bz.jctech888.com.cn

TS:   await fetch(url)
来源：http://zg.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jr.lnxyls.cn

Go:   resp, err := http.Get(url)
来源：http://os.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wf.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://af.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://nu.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wh.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rf.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nx.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wa.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aa.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sz.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ic.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yg.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://qj.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ui.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oa.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cv.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gb.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xx.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hf.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://my.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hl.hahajie.cn

[L04] 设置超时
来源：http://ke.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://dq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yh.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://in.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xn.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zz.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mn.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ja.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ic.nszjky.cn

[L05] 上传文件（multipart）
来源：http://oz.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hd.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xn.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gw.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xa.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://or.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lk.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sl.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dt.hahajie.cn

[L06] 解析响应为 JSON
来源：http://ag.nszjky.cn

Py:   resp.json()
来源：http://qr.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://af.shtwfgs.cn

JS:   await resp.json()
来源：http://ec.jctech888.com.cn

TS:   await resp.json()
来源：http://vd.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jn.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bv.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://qo.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fa.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://pb.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nn.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sl.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://fy.jctech888.com.cn

TS:   resp.ok;  resp.status
来源：http://od.szsharing.cn

Java: resp.statusCode()
来源：http://hq.bjjhwx.cn

Go:   resp.StatusCode
来源：http://bj.gzmigu.cn

Ruby: resp.code.to_i
来源：http://gz.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://eg.9csxet.cn

[L08] 并发请求多个地址
来源：http://zr.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ny.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://sy.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://up.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gx.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ia.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oe.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ai.521024.cn

================================================================================
来源：http://bw.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://tl.chemitech.net.cn

================================================================================
来源：http://bl.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://kb.hnjuh.cn

Py:   sys.argv[1:]
来源：http://yr.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://op.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://hv.521024.cn

TS:   process.argv.slice(2)
来源：http://um.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://om.asd995.cn

Go:   os.Args[1:]
来源：http://le.nicolike.cn

Ruby: ARGV
来源：http://rd.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://up.panjiajie.cn

[M02] 读取环境变量
来源：http://lb.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://oc.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ex.nszjky.cn

JS:   process.env.HOME
来源：http://dh.muxihuayi.cn

TS:   process.env.HOME
来源：http://bk.huanxung.cn

Java: System.getenv("HOME")
来源：http://uh.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jz.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://su.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tu.muxihuayi.cn

[M03] 执行外部命令
来源：http://kb.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ej.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ex.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ly.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jk.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oe.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xy.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xw.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://ds.panjiajie.cn

[M04] 获取当前工作目录
来源：http://zn.bookmarksfly.cn

Py:   os.getcwd()
来源：http://nq.haigaiapp.cn

PHP:  getcwd();
来源：http://wa.hahajie.cn

JS:   process.cwd()
来源：http://dh.nszjky.cn

TS:   process.cwd()
来源：http://tg.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ym.shxzskj.cn

Go:   os.Getwd()
来源：http://vc.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ca.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ou.huanxung.cn

[M05] 设置退出码
来源：http://rp.szsharing.cn

Py:   sys.exit(1)
来源：http://kz.wgjwhj.cn

PHP:  exit(1);
来源：http://la.hnjuh.cn

JS:   process.exit(1)
来源：http://pi.9csxet.cn

TS:   process.exit(1)
来源：http://sw.jianghongdianzi.cn

Java: System.exit(1)
来源：http://ux.szxytkj.cn

Go:   os.Exit(1)
来源：http://mh.yuntaijiaju.cn

Ruby: exit 1
来源：http://kv.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qh.nszjky.cn

[M06] 向标准错误输出
来源：http://ke.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://gv.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bq.521024.cn

JS:   console.error("err")
来源：http://mr.shtwfgs.cn

TS:   console.error("err")
来源：http://id.huanxung.cn

Java: System.err.println("err")
来源：http://um.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fh.newstarts.cn

Ruby: warn "err"
来源：http://jr.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://ns.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ge.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://pk.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://el.lnxyls.cn

JS:   require.main === module
来源：http://mi.szsharing.cn

TS:   require.main === module
来源：http://ty.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://fj.hnjuh.cn

Go:   func main()
来源：http://sh.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yd.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://bq.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://nt.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://ov.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ud.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://ow.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://gw.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aw.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kl.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kq.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ap.asd995.cn

================================================================================
来源：http://ot.muxihuayi.cn

N. 数据结构与算法
来源：http://no.chemitech.net.cn

================================================================================
来源：http://oe.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://fx.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cg.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vs.szxytkj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://id.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://do.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jd.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://aw.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vd.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ss.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://pl.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vh.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sz.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xu.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://do.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rp.nszjky.cn

Go:   slices.Sort(arr)
来源：http://fw.bjjhwx.cn

Ruby: arr.sort
来源：http://au.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kc.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://iw.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dl.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://li.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qz.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ka.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pk.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hb.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fh.nszjky.cn

[N04] 斐波那契数列
来源：http://zo.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://al.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dv.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eo.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ep.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ar.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zw.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ka.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lt.nszjky.cn

[N05] 最大公约数
来源：http://jr.nszjky.cn

Py:   math.gcd(a, b)
来源：http://fo.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pj.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://za.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lm.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lg.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zh.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://uw.hnjuh.cn


<!-- 参考信息 -->