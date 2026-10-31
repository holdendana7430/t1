代发 wailian999

[J07] 比较两个日期
来源：http://jp.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://ey.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mi.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pk.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sz.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vz.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vm.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://df.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://hb.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://cx.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uh.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://so.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dt.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ry.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ks.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nj.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oi.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rw.bjjhwx.cn

[J09] 时区处理
来源：http://os.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ea.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wg.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qa.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oe.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tq.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sn.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://py.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://kd.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://as.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nx.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oo.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hs.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gk.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ke.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rg.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dr.asd995.cn

================================================================================
来源：http://dv.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ix.hahajie.cn

================================================================================
来源：http://mb.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://rf.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qh.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zo.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://rr.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://xf.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xc.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://nj.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jl.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hq.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://jd.521024.cn

Py:   json.loads(s)
来源：http://vn.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ti.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://jz.colortex.cn

TS:   JSON.parse(s)
来源：http://wl.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oe.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://kl.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://cz.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qg.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://tc.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wn.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gr.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bm.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bv.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pn.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pt.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ts.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gl.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://bm.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pw.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gq.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ip.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://if.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dv.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://go.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hr.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ox.9csxet.cn

[K05] 深拷贝对象
来源：http://gg.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://uc.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://zf.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://ix.asd995.cn

TS:   structuredClone(obj)
来源：http://yy.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xp.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nw.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ea.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mu.521024.cn

[K06] 解析 URL 查询串
来源：http://df.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ac.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vz.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qz.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tw.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ac.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gj.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fz.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oc.szxytkj.cn

[K07] 进制转换
来源：http://cd.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mu.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ro.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wy.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dg.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tn.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ea.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ci.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://nc.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://hd.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://on.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://cd.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://gz.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pe.bookmarksfly.cn

Go:   encoding/gob
来源：http://ya.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://dk.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uz.hahajie.cn

================================================================================
来源：http://hr.newstarts.cn

L. 网络请求
来源：http://uf.gzmigu.cn

================================================================================
来源：http://ou.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://zb.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://do.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lq.wgjwhj.cn

JS:   await fetch(url)
来源：http://ld.muxihuayi.cn

TS:   await fetch(url)
来源：http://ee.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ys.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://zh.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zs.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://en.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://bo.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qq.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://du.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ku.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pg.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nu.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ye.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mj.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wv.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://kl.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kn.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yu.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vd.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://af.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rg.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://op.huixinmuqiang.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vo.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bp.bjjhwx.cn

[L04] 设置超时
来源：http://xp.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://fx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ug.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hx.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uj.chemitech.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lx.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oo.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tr.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://mx.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ov.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rx.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fl.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bc.chemitech.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dn.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vh.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ny.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://si.szsharing.cn

[L06] 解析响应为 JSON
来源：http://sz.colortex.cn

Py:   resp.json()
来源：http://vl.nicolike.cn

PHP:  json_decode($body, true);
来源：http://gr.huanxung.cn

JS:   await resp.json()
来源：http://oo.shxzskj.cn

TS:   await resp.json()
来源：http://pv.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ce.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://od.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://td.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hy.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://mg.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ys.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dh.colortex.cn

JS:   resp.ok;  resp.status
来源：http://lq.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://hr.shtwfgs.cn

Java: resp.statusCode()
来源：http://fx.9csxet.cn

Go:   resp.StatusCode
来源：http://qe.shtwfgs.cn

Ruby: resp.code.to_i
来源：http://gx.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://rv.asd995.cn

[L08] 并发请求多个地址
来源：http://ls.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nv.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://oy.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rq.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pt.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sv.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ql.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ul.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ym.haigaiapp.cn

================================================================================
来源：http://ta.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://td.jianghongdianzi.cn

================================================================================
来源：http://mc.shxzskj.cn

[M01] 读取命令行参数
来源：http://yd.521024.cn

Py:   sys.argv[1:]
来源：http://md.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://gv.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://qk.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://pa.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://nc.newstarts.cn

Go:   os.Args[1:]
来源：http://vv.huanxung.cn

Ruby: ARGV
来源：http://ui.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://zk.colortex.cn

[M02] 读取环境变量
来源：http://fi.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://rq.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://no.newstarts.cn

JS:   process.env.HOME
来源：http://gd.chemitech.net.cn

TS:   process.env.HOME
来源：http://ea.newstarts.cn

Java: System.getenv("HOME")
来源：http://ns.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ba.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://ac.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ao.lnxyls.cn

[M03] 执行外部命令
来源：http://tk.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ms.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ut.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zu.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dd.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rw.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sz.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ub.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://tn.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://qx.shtwfgs.cn

Py:   os.getcwd()
来源：http://uk.colortex.cn

PHP:  getcwd();
来源：http://nu.yuntaijiaju.cn

JS:   process.cwd()
来源：http://pf.hahajie.cn

TS:   process.cwd()
来源：http://cm.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://br.521024.cn

Go:   os.Getwd()
来源：http://xu.521024.cn

Ruby: Dir.pwd
来源：http://ii.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uf.jianghongdianzi.cn

[M05] 设置退出码
来源：http://kz.colortex.cn

Py:   sys.exit(1)
来源：http://bw.hahajie.cn

PHP:  exit(1);
来源：http://iv.yuexingan06.cn

JS:   process.exit(1)
来源：http://sd.shtwfgs.cn

TS:   process.exit(1)
来源：http://nx.colortex.cn

Java: System.exit(1)
来源：http://vn.wgjwhj.cn

Go:   os.Exit(1)
来源：http://dw.hahajie.cn

Ruby: exit 1
来源：http://ok.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hd.wgjwhj.cn

[M06] 向标准错误输出
来源：http://nl.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://rk.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ps.lnxyls.cn

JS:   console.error("err")
来源：http://ih.haigaiapp.cn

TS:   console.error("err")
来源：http://qi.asd995.cn

Java: System.err.println("err")
来源：http://fj.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fk.szxytkj.cn

Ruby: warn "err"
来源：http://ew.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ws.shtwfgs.cn

[M07] 判断是否为主入口
来源：http://hl.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://ot.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pk.szxytkj.cn

JS:   require.main === module
来源：http://sf.szsharing.cn

TS:   require.main === module
来源：http://wy.szsharing.cn

Java: public static void main(String[] args)
来源：http://iq.jctech888.com.cn

Go:   func main()
来源：http://eo.panjiajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jb.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://mk.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://xr.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ci.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://jp.shxzskj.cn

JS:   process.platform;  process.version
来源：http://mh.lnxyls.cn

TS:   process.platform;  process.version
来源：http://yg.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qw.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ck.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://km.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rv.yuexingan06.cn

================================================================================
来源：http://eq.shtwfgs.cn

N. 数据结构与算法
来源：http://ua.shxzukj.cn

================================================================================
来源：http://ox.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://iy.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jm.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vg.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rb.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zm.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bl.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://fv.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rs.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wf.yuexingan06.cn

[N02] 排序（工程实践用内置实现）
来源：http://nv.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://nb.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mg.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dt.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ui.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://do.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://la.huixinmuqiang.cn

Ruby: arr.sort
来源：http://la.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ue.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://zl.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://va.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://xz.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://me.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gm.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iz.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fb.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tt.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sp.huixiangedu.cn

[N04] 斐波那契数列
来源：http://pz.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qr.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sa.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mv.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yc.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dj.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zs.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oa.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mf.szxytkj.cn


<!-- 参考信息 -->