代发 wailian999

[J07] 比较两个日期
来源：http://ez.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ic.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eb.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vr.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://na.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sj.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xl.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ws.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://xj.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://bz.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://po.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uq.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yd.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://do.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ak.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wc.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wz.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nj.chemitech.net.cn

[J09] 时区处理
来源：http://tm.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cf.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://md.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://va.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://si.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rs.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lj.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vd.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://iz.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kj.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://op.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wd.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lg.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pw.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ku.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://os.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ty.panjiajie.cn

================================================================================
来源：http://pp.newstarts.cn

K. JSON 与序列化
来源：http://ft.szsharing.cn

================================================================================
来源：http://aa.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://xj.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ju.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qd.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://ea.asd995.cn

TS:   JSON.stringify(obj)
来源：http://pr.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mi.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://og.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ti.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wj.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://yg.szxytkj.cn

Py:   json.loads(s)
来源：http://ao.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fk.panjiajie.cn

JS:   JSON.parse(s)
来源：http://py.asd995.cn

TS:   JSON.parse(s)
来源：http://nr.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://af.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://vp.nszjky.cn

Ruby: JSON.parse(s)
来源：http://jh.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lx.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://ia.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://if.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gs.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lb.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jq.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zp.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dl.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uc.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hj.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://wu.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yh.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ah.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cm.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ul.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nu.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rb.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dv.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cj.jctech888.com.cn

[K05] 深拷贝对象
来源：http://sq.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://fq.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://ox.szxytkj.cn

JS:   structuredClone(obj)
来源：http://rk.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://cp.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gw.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ac.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lu.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ii.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://ap.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ni.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sh.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://af.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bz.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ow.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://au.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oa.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vz.szxytkj.cn

[K07] 进制转换
来源：http://lm.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ur.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dv.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kr.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gi.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pt.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://to.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://js.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yj.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://dn.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://js.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mn.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://pm.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://kc.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uy.szsharing.cn

Go:   encoding/gob
来源：http://tx.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://cp.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qf.nszjky.cn

================================================================================
来源：http://ym.hahajie.cn

L. 网络请求
来源：http://ev.nszjky.cn

================================================================================
来源：http://mw.szsharing.cn

[L01] 发送 GET 请求
来源：http://jh.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ad.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zc.szsharing.cn

JS:   await fetch(url)
来源：http://qr.yuexingan06.cn

TS:   await fetch(url)
来源：http://vs.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jd.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://vx.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pl.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wn.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://vb.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xn.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ds.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://va.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iq.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kk.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mo.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sy.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vd.lnxyls.cn

[L03] 设置自定义请求头
来源：http://ol.gzmigu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jl.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vg.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nq.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ak.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yl.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fx.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ar.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xi.hahajie.cn

[L04] 设置超时
来源：http://bl.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://qg.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rm.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rq.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rh.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uk.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gj.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ls.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gb.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://sq.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yx.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hu.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://va.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xm.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yt.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://im.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vu.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lj.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://ez.muxihuayi.cn

Py:   resp.json()
来源：http://rl.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://ca.bookmarksfly.cn

JS:   await resp.json()
来源：http://ru.bookmarksfly.cn

TS:   await resp.json()
来源：http://fo.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mc.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ui.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://np.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wx.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://ge.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ij.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tn.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://ei.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://yo.nszjky.cn

Java: resp.statusCode()
来源：http://fv.bjjhwx.cn

Go:   resp.StatusCode
来源：http://dh.shxzukj.cn

Ruby: resp.code.to_i
来源：http://pp.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://vo.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://uf.9csxet.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iu.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://gy.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zb.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ai.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nw.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uo.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bw.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lf.yuexingan06.cn

================================================================================
来源：http://th.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://ui.gzmigu.cn

================================================================================
来源：http://rs.nicolike.cn

[M01] 读取命令行参数
来源：http://sd.hahajie.cn

Py:   sys.argv[1:]
来源：http://rs.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ql.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://on.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://fr.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://vb.panjiajie.cn

Go:   os.Args[1:]
来源：http://ih.huixiangedu.cn

Ruby: ARGV
来源：http://xm.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://al.huanxung.cn

[M02] 读取环境变量
来源：http://jn.jctech888.com.cn

Py:   os.environ.get("HOME")
来源：http://pz.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xh.panjiajie.cn

JS:   process.env.HOME
来源：http://ky.asd995.cn

TS:   process.env.HOME
来源：http://wq.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://am.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ga.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://aa.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vt.colortex.cn

[M03] 执行外部命令
来源：http://or.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nk.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wd.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gm.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ms.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ez.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sk.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eu.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://sr.hnjuh.cn

[M04] 获取当前工作目录
来源：http://kh.chemitech.net.cn

Py:   os.getcwd()
来源：http://uf.shxzukj.cn

PHP:  getcwd();
来源：http://ku.nicolike.cn

JS:   process.cwd()
来源：http://uo.9csxet.cn

TS:   process.cwd()
来源：http://pu.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://cj.hnjuh.cn

Go:   os.Getwd()
来源：http://fg.asd995.cn

Ruby: Dir.pwd
来源：http://kh.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dp.colortex.cn

[M05] 设置退出码
来源：http://zp.lnxyls.cn

Py:   sys.exit(1)
来源：http://ae.panjiajie.cn

PHP:  exit(1);
来源：http://tz.nszjky.cn

JS:   process.exit(1)
来源：http://lx.panjiajie.cn

TS:   process.exit(1)
来源：http://ti.muxihuayi.cn

Java: System.exit(1)
来源：http://kf.yuexingan06.cn

Go:   os.Exit(1)
来源：http://fh.yuexingan06.cn

Ruby: exit 1
来源：http://nv.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gf.shtwfgs.cn

[M06] 向标准错误输出
来源：http://ne.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://uv.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bx.yuntaijiaju.cn

JS:   console.error("err")
来源：http://pb.chemitech.net.cn

TS:   console.error("err")
来源：http://uv.shxzskj.cn

Java: System.err.println("err")
来源：http://ns.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cr.newstarts.cn

Ruby: warn "err"
来源：http://mr.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://oo.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://sj.521024.cn

Py:   if __name__ == "__main__":
来源：http://bx.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xz.haigaiapp.cn

JS:   require.main === module
来源：http://re.haigaiapp.cn

TS:   require.main === module
来源：http://wg.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://jq.huixinmuqiang.cn

Go:   func main()
来源：http://uk.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rz.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://pv.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://eu.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://dz.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://xq.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://mm.9csxet.cn

TS:   process.platform;  process.version
来源：http://vj.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ew.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nt.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tu.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ac.chemitech.net.cn

================================================================================
来源：http://ss.nicolike.cn

N. 数据结构与算法
来源：http://sc.panjiajie.cn

================================================================================
来源：http://qy.asd995.cn

[N01] 二分查找（有序数组）
来源：http://qz.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://au.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cm.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yw.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://dd.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ss.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oj.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://xs.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pj.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ob.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zu.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lg.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wq.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://az.bjjhwx.cn

Ruby: arr.sort
来源：http://ep.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://au.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://kz.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://al.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ep.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://no.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://of.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kp.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jp.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ps.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://es.hahajie.cn

[N04] 斐波那契数列
来源：http://fz.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://of.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rm.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ro.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cp.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ul.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vw.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vt.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.szsharing.cn


<!-- 参考信息 -->