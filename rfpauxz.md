代发 wailian999

[J07] 比较两个日期
来源：http://ku.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://hj.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wj.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://it.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yt.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://on.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jq.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ao.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://rt.shxzukj.cn

[J08] 提取年月日与星期
来源：http://vb.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bm.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://af.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dw.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cs.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://za.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qr.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mo.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ot.panjiajie.cn

[J09] 时区处理
来源：http://fq.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ou.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ny.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qd.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://me.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bq.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hs.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ab.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fl.szxytkj.cn

[J10] 取今天 / 本月第一天
来源：http://hp.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rn.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nx.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://go.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ut.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://te.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nx.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xh.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://np.newstarts.cn

================================================================================
来源：http://pp.panjiajie.cn

K. JSON 与序列化
来源：http://fy.shtwfgs.cn

================================================================================
来源：http://wf.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://dl.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://do.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ra.asd995.cn

JS:   JSON.stringify(obj)
来源：http://ds.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://om.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oi.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://ii.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rc.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ph.colortex.cn

[K02] JSON 字符串转对象
来源：http://ca.wgjwhj.cn

Py:   json.loads(s)
来源：http://rv.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://en.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://zg.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://rt.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ad.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://fq.szsharing.cn

Ruby: JSON.parse(s)
来源：http://sb.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fu.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://yq.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cx.shtwfgs.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://br.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oj.panjiajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eb.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dx.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yp.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ds.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qc.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://lx.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gq.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hi.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dh.wgjwhj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yx.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qa.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://km.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ly.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xu.jctech888.com.cn

[K05] 深拷贝对象
来源：http://uz.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://ex.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://ly.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://qy.shxzskj.cn

TS:   structuredClone(obj)
来源：http://ip.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kt.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dt.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qo.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://no.521024.cn

[K06] 解析 URL 查询串
来源：http://wk.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hy.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ak.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://en.yuntaijiaju.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ow.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dk.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cz.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ws.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cn.yuexingan06.cn

[K07] 进制转换
来源：http://wb.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dq.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hl.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hh.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rg.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://we.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xk.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jz.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cy.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ti.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://mg.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bc.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://zc.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://rr.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://th.muxihuayi.cn

Go:   encoding/gob
来源：http://pt.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://yk.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fq.bookmarksfly.cn

================================================================================
来源：http://rq.wgjwhj.cn

L. 网络请求
来源：http://nl.yuexingan06.cn

================================================================================
来源：http://rj.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ym.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tu.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ks.newstarts.cn

JS:   await fetch(url)
来源：http://mc.huixiangedu.cn

TS:   await fetch(url)
来源：http://xk.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lq.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://na.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kv.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zj.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://qw.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://re.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ar.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qv.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sy.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ru.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wn.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://no.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yi.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://ow.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dm.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eo.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hi.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mh.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wp.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://md.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xf.shxzukj.cn

[L04] 设置超时
来源：http://as.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://yt.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kv.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tx.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ko.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ss.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fc.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sw.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ho.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://gg.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qk.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aq.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kq.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xh.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tg.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pj.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hq.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rq.nicolike.cn

[L06] 解析响应为 JSON
来源：http://qk.szsharing.cn

Py:   resp.json()
来源：http://gb.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://ex.yuexingan06.cn

JS:   await resp.json()
来源：http://vq.szxytkj.cn

TS:   await resp.json()
来源：http://wz.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wf.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lp.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://lw.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rg.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://ht.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xu.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ep.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://au.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://jl.bookmarksfly.cn

Java: resp.statusCode()
来源：http://td.huixiangedu.cn

Go:   resp.StatusCode
来源：http://rm.panjiajie.cn

Ruby: resp.code.to_i
来源：http://fh.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://ji.huanxung.cn

[L08] 并发请求多个地址
来源：http://di.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vw.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://op.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hu.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hy.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qj.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ez.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jc.shxzukj.cn

================================================================================
来源：http://jd.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://qe.nszjky.cn

================================================================================
来源：http://ia.9csxet.cn

[M01] 读取命令行参数
来源：http://jm.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://qe.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://bw.wgjwhj.cn

JS:   process.argv.slice(2)
来源：http://qv.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://lv.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://hg.szsharing.cn

Go:   os.Args[1:]
来源：http://rd.jctech888.com.cn

Ruby: ARGV
来源：http://ms.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://uw.bookmarksfly.cn

[M02] 读取环境变量
来源：http://is.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://cg.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ic.9csxet.cn

JS:   process.env.HOME
来源：http://ul.huixiangedu.cn

TS:   process.env.HOME
来源：http://xd.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://to.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kr.nszjky.cn

Ruby: ENV["HOME"]
来源：http://ra.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://or.gzmigu.cn

[M03] 执行外部命令
来源：http://qm.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vk.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yg.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kv.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wc.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qq.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mh.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jg.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://jq.huanxung.cn

[M04] 获取当前工作目录
来源：http://tt.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://dn.newstarts.cn

PHP:  getcwd();
来源：http://fs.bjjhwx.cn

JS:   process.cwd()
来源：http://sc.bjjhwx.cn

TS:   process.cwd()
来源：http://yh.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://vo.nicolike.cn

Go:   os.Getwd()
来源：http://qh.bookmarksfly.cn

Ruby: Dir.pwd
来源：http://ex.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lv.newstarts.cn

[M05] 设置退出码
来源：http://xz.huixiangedu.cn

Py:   sys.exit(1)
来源：http://ux.shtwfgs.cn

PHP:  exit(1);
来源：http://jg.shtwfgs.cn

JS:   process.exit(1)
来源：http://do.colortex.cn

TS:   process.exit(1)
来源：http://hc.bookmarksfly.cn

Java: System.exit(1)
来源：http://fi.chemitech.net.cn

Go:   os.Exit(1)
来源：http://lt.shtwfgs.cn

Ruby: exit 1
来源：http://qr.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fk.shtwfgs.cn

[M06] 向标准错误输出
来源：http://aw.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://rf.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ja.shtwfgs.cn

JS:   console.error("err")
来源：http://mt.haigaiapp.cn

TS:   console.error("err")
来源：http://fx.hahajie.cn

Java: System.err.println("err")
来源：http://cg.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mh.gzmigu.cn

Ruby: warn "err"
来源：http://xd.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://vz.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://th.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://oz.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uk.bookmarksfly.cn

JS:   require.main === module
来源：http://iw.huanxung.cn

TS:   require.main === module
来源：http://qq.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ne.hnjuh.cn

Go:   func main()
来源：http://bp.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hb.yuntaijiaju.cn

C#:   static void Main(string[] args)
来源：http://js.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://jg.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://ff.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://hr.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://md.shxzskj.cn

TS:   process.platform;  process.version
来源：http://my.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uc.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gz.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gb.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zg.muxihuayi.cn

================================================================================
来源：http://xr.gzmigu.cn

N. 数据结构与算法
来源：http://kv.9csxet.cn

================================================================================
来源：http://qq.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://xz.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lg.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kq.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dx.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vo.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gi.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://ju.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zp.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wc.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://xa.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://xu.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sg.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cz.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sn.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oh.newstarts.cn

Go:   slices.Sort(arr)
来源：http://ig.haigaiapp.cn

Ruby: arr.sort
来源：http://to.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zv.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://zj.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nb.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://pw.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gp.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ya.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cr.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fx.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nj.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xd.panjiajie.cn

[N04] 斐波那契数列
来源：http://du.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pp.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qb.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mf.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gs.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ip.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ms.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wv.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uh.bookmarksfly.cn


<!-- 参考信息 -->