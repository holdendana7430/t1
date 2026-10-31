代发 wailian999

[J07] 比较两个日期
来源：http://ll.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://da.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ui.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tv.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tn.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ap.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tk.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ob.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://km.gzmigu.cn

[J08] 提取年月日与星期
来源：http://er.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ez.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fa.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qb.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cv.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hp.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uq.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zk.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ko.bookmarksfly.cn

[J09] 时区处理
来源：http://jx.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cg.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vm.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aw.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nv.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ln.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jp.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xb.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ym.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://px.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tw.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nh.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bs.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oi.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vt.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ys.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oy.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bf.huixiangedu.cn

================================================================================
来源：http://kr.521024.cn

K. JSON 与序列化
来源：http://qz.lnxyls.cn

================================================================================
来源：http://ze.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://at.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jg.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nc.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://zv.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://iw.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ev.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://dd.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wl.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zz.colortex.cn

[K02] JSON 字符串转对象
来源：http://if.wgjwhj.cn

Py:   json.loads(s)
来源：http://so.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qw.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://fs.lnxyls.cn

TS:   JSON.parse(s)
来源：http://mt.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vg.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://pa.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://fq.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tj.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://oa.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lp.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sy.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gj.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hg.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lj.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://th.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dd.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://yf.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yy.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yx.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://py.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tk.szxytkj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ci.szxytkj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fa.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ww.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dl.huixiangedu.cn

[K05] 深拷贝对象
来源：http://az.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://nb.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://kf.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://ub.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://sr.huanxung.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ib.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fs.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jh.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vd.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://xa.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yu.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sh.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gb.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ms.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vp.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ud.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wb.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jc.gzmigu.cn

[K07] 进制转换
来源：http://iz.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://er.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sy.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hx.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bw.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mj.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mr.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mu.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kl.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://sx.521024.cn

Py:   pickle.dumps(obj)
来源：http://nv.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://np.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ji.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://li.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xx.521024.cn

Go:   encoding/gob
来源：http://lm.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://uf.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sl.hahajie.cn

================================================================================
来源：http://td.bjjhwx.cn

L. 网络请求
来源：http://nl.shtwfgs.cn

================================================================================
来源：http://wy.nszjky.cn

[L01] 发送 GET 请求
来源：http://bu.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cr.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ga.yuexingan06.cn

JS:   await fetch(url)
来源：http://or.9csxet.cn

TS:   await fetch(url)
来源：http://mv.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ad.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://jr.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hu.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://io.huanxung.cn

[L02] 发送 POST JSON
来源：http://ho.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hs.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ac.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bw.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pe.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hj.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://py.chemitech.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pz.gzmigu.cn

[L03] 设置自定义请求头
来源：http://fx.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ks.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://np.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vi.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uj.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ao.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qn.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ca.huanxung.cn

[L04] 设置超时
来源：http://pf.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://zv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tw.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qo.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ei.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mk.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eb.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kp.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wa.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://fj.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xn.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hn.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cs.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://os.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ge.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mr.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jg.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lp.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://sq.chemitech.net.cn

Py:   resp.json()
来源：http://gb.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://vu.asd995.cn

JS:   await resp.json()
来源：http://ud.521024.cn

TS:   await resp.json()
来源：http://fc.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://je.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vy.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://pn.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://et.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://wa.huixinmuqiang.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eq.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yj.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://sf.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://bv.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://zc.shtwfgs.cn

Go:   resp.StatusCode
来源：http://xk.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://wt.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://pv.521024.cn

[L08] 并发请求多个地址
来源：http://iu.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oo.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ia.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sb.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ew.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vl.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jy.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mc.gzmigu.cn

================================================================================
来源：http://nx.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://qu.nicolike.cn

================================================================================
来源：http://bs.9csxet.cn

[M01] 读取命令行参数
来源：http://kp.newstarts.cn

Py:   sys.argv[1:]
来源：http://wq.hahajie.cn

PHP:  $argv;  $argc;
来源：http://bl.newstarts.cn

JS:   process.argv.slice(2)
来源：http://yy.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://wv.asd995.cn

Java: args 数组（main 方法参数）
来源：http://hr.panjiajie.cn

Go:   os.Args[1:]
来源：http://dy.szxytkj.cn

Ruby: ARGV
来源：http://pd.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://id.yuexingan06.cn

[M02] 读取环境变量
来源：http://uw.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://kf.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lx.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://ph.shxzukj.cn

TS:   process.env.HOME
来源：http://dl.panjiajie.cn

Java: System.getenv("HOME")
来源：http://uo.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ks.asd995.cn

Ruby: ENV["HOME"]
来源：http://xi.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ga.9csxet.cn

[M03] 执行外部命令
来源：http://ss.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oa.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dh.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ur.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ys.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lp.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qq.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://si.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://sl.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://xe.hahajie.cn

Py:   os.getcwd()
来源：http://pb.hnjuh.cn

PHP:  getcwd();
来源：http://ow.panjiajie.cn

JS:   process.cwd()
来源：http://qb.wgjwhj.cn

TS:   process.cwd()
来源：http://hc.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ne.muxihuayi.cn

Go:   os.Getwd()
来源：http://qc.haigaiapp.cn

Ruby: Dir.pwd
来源：http://po.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yw.shxzukj.cn

[M05] 设置退出码
来源：http://yj.szsharing.cn

Py:   sys.exit(1)
来源：http://vr.shxzskj.cn

PHP:  exit(1);
来源：http://se.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://gt.shxzukj.cn

TS:   process.exit(1)
来源：http://lx.lnxyls.cn

Java: System.exit(1)
来源：http://mq.asd995.cn

Go:   os.Exit(1)
来源：http://sk.bjjhwx.cn

Ruby: exit 1
来源：http://ne.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ak.wgjwhj.cn

[M06] 向标准错误输出
来源：http://go.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://di.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ey.shxzskj.cn

JS:   console.error("err")
来源：http://gn.muxihuayi.cn

TS:   console.error("err")
来源：http://we.newstarts.cn

Java: System.err.println("err")
来源：http://qg.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gy.muxihuayi.cn

Ruby: warn "err"
来源：http://pf.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://yp.panjiajie.cn

[M07] 判断是否为主入口
来源：http://jh.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://aq.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uw.bjjhwx.cn

JS:   require.main === module
来源：http://uo.panjiajie.cn

TS:   require.main === module
来源：http://ho.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://zf.bjjhwx.cn

Go:   func main()
来源：http://qt.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ii.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://bs.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://rz.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://at.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://lc.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ra.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://de.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jl.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mg.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bu.shxzukj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fa.shxzskj.cn

================================================================================
来源：http://yl.muxihuayi.cn

N. 数据结构与算法
来源：http://qu.jctech888.com.cn

================================================================================
来源：http://ry.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://gc.nszjky.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gs.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rz.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kp.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hj.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ct.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://xk.bookmarksfly.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sq.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vp.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://rh.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://hi.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jz.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ci.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qw.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sq.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://ao.asd995.cn

Ruby: arr.sort
来源：http://pg.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ff.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://oo.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kh.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://fu.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://de.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gw.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tw.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gp.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ut.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ah.szxytkj.cn

[N04] 斐波那契数列
来源：http://ns.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rj.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://py.asd995.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mc.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://am.yuntaijiaju.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ch.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ys.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ps.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ti.chemitech.net.cn


<!-- 参考信息 -->