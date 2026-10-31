代发 wailian999

[J07] 比较两个日期
来源：http://sm.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://sh.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dp.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ib.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ac.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zw.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lj.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://df.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://al.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://nm.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ci.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gi.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lz.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xa.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hh.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ed.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pc.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sn.newstarts.cn

[J09] 时区处理
来源：http://ge.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ce.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://en.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bs.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zg.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rh.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vi.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tw.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kf.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://vu.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aq.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gu.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ly.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fk.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ec.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://je.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ws.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ng.hahajie.cn

================================================================================
来源：http://nq.521024.cn

K. JSON 与序列化
来源：http://xt.huixiangedu.cn

================================================================================
来源：http://al.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://oi.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zo.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://bh.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://lm.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ho.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://zr.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://od.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qq.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://hv.szsharing.cn

Py:   json.loads(s)
来源：http://eq.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mq.asd995.cn

JS:   JSON.parse(s)
来源：http://zi.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ee.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rt.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://sg.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://up.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jy.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://cu.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://go.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pl.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yr.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xt.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tx.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pn.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ia.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bz.colortex.cn

[K04] 读取 JSON 文件
来源：http://fc.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gv.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oz.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rh.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uh.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gn.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ia.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dt.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gr.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://me.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://vf.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://eu.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://hr.nszjky.cn

TS:   structuredClone(obj)
来源：http://hz.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ez.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vh.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nj.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ql.asd995.cn

[K06] 解析 URL 查询串
来源：http://bs.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://we.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bs.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mt.nicolike.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gn.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oo.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ki.bjjhwx.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xk.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ar.szxytkj.cn

[K07] 进制转换
来源：http://us.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hg.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oh.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ck.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vr.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yi.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fl.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wv.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ih.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://dc.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://xe.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jn.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://sw.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://oa.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.colortex.cn

Go:   encoding/gob
来源：http://cs.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://mt.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wi.shxzskj.cn

================================================================================
来源：http://vc.nszjky.cn

L. 网络请求
来源：http://qa.yuntaijiaju.cn

================================================================================
来源：http://al.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://ed.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tx.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://on.bjjhwx.cn

JS:   await fetch(url)
来源：http://kb.wgjwhj.cn

TS:   await fetch(url)
来源：http://lv.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ak.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://xy.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zs.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bk.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://fb.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zr.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ea.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eo.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mx.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bx.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mq.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yx.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bt.szxytkj.cn

[L03] 设置自定义请求头
来源：http://xw.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sh.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yg.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ix.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jp.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rr.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qc.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ef.bookmarksfly.cn

[L04] 设置超时
来源：http://zo.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://ko.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yp.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jj.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://em.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sy.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://go.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lh.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://li.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://wz.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hw.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vh.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bn.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://up.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rt.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://as.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nb.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ab.shtwfgs.cn

Py:   resp.json()
来源：http://js.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://mw.521024.cn

JS:   await resp.json()
来源：http://jw.panjiajie.cn

TS:   await resp.json()
来源：http://so.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pf.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bx.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://xw.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://va.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://xv.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qs.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bt.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://df.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://yl.hnjuh.cn

Java: resp.statusCode()
来源：http://hu.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://kq.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://ir.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://mx.shxzukj.cn

[L08] 并发请求多个地址
来源：http://cg.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ql.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ks.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yl.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fa.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dg.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qc.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yt.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cq.colortex.cn

================================================================================
来源：http://nm.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://td.szsharing.cn

================================================================================
来源：http://zi.szxytkj.cn

[M01] 读取命令行参数
来源：http://qz.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://li.521024.cn

PHP:  $argv;  $argc;
来源：http://ch.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://ap.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://qx.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://fn.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://vp.jianghongdianzi.cn

Ruby: ARGV
来源：http://tr.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://il.9csxet.cn

[M02] 读取环境变量
来源：http://el.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://tg.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xq.9csxet.cn

JS:   process.env.HOME
来源：http://gb.asd995.cn

TS:   process.env.HOME
来源：http://md.hnjuh.cn

Java: System.getenv("HOME")
来源：http://nu.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tv.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ao.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://av.bookmarksfly.cn

[M03] 执行外部命令
来源：http://yk.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bn.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uv.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wi.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rn.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gh.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xg.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ou.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://yl.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://yb.hahajie.cn

Py:   os.getcwd()
来源：http://ok.wgjwhj.cn

PHP:  getcwd();
来源：http://cq.newstarts.cn

JS:   process.cwd()
来源：http://gb.hnjuh.cn

TS:   process.cwd()
来源：http://pt.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://vc.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://pv.haigaiapp.cn

Ruby: Dir.pwd
来源：http://us.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ne.haigaiapp.cn

[M05] 设置退出码
来源：http://jx.hnjuh.cn

Py:   sys.exit(1)
来源：http://cb.nszjky.cn

PHP:  exit(1);
来源：http://as.hnjuh.cn

JS:   process.exit(1)
来源：http://md.bjjhwx.cn

TS:   process.exit(1)
来源：http://dt.shtwfgs.cn

Java: System.exit(1)
来源：http://ge.chemitech.net.cn

Go:   os.Exit(1)
来源：http://rx.shxzskj.cn

Ruby: exit 1
来源：http://ae.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aq.colortex.cn

[M06] 向标准错误输出
来源：http://zw.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://qo.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cf.yuexingan06.cn

JS:   console.error("err")
来源：http://ar.nicolike.cn

TS:   console.error("err")
来源：http://rz.nicolike.cn

Java: System.err.println("err")
来源：http://eq.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zl.yuntaijiaju.cn

Ruby: warn "err"
来源：http://lv.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://zi.hnjuh.cn

[M07] 判断是否为主入口
来源：http://xv.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://fl.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nd.muxihuayi.cn

JS:   require.main === module
来源：http://dt.jctech888.com.cn

TS:   require.main === module
来源：http://ft.nicolike.cn

Java: public static void main(String[] args)
来源：http://op.lnxyls.cn

Go:   func main()
来源：http://lx.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bt.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://ek.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://cf.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://hu.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://pu.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://wq.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://bg.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wv.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cb.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wi.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xh.huixiangedu.cn

================================================================================
来源：http://hg.9csxet.cn

N. 数据结构与算法
来源：http://hf.wgjwhj.cn

================================================================================
来源：http://fc.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://zf.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kh.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kn.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sa.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hb.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hp.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://sh.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gu.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uw.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://lc.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wk.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qy.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rg.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://no.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jl.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://pw.muxihuayi.cn

Ruby: arr.sort
来源：http://lh.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dc.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://xo.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://si.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ha.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wk.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bb.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lb.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vd.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cc.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ab.9csxet.cn

[N04] 斐波那契数列
来源：http://fq.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://op.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wz.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ya.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tt.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ch.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pz.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pd.shxzskj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dj.gzmigu.cn


<!-- 参考信息 -->