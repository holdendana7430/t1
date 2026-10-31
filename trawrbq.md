代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ib.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sa.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://og.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dg.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://mk.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://fp.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wd.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://va.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xu.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ry.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://br.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xu.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xx.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wk.huixiangedu.cn

[J09] 时区处理
来源：http://lh.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sr.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bj.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ce.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jt.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yn.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lw.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tk.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://nr.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xi.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cp.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lk.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qz.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xx.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bh.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wt.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dp.chemitech.net.cn

================================================================================
来源：http://bn.bookmarksfly.cn

K. JSON 与序列化
来源：http://lx.muxihuayi.cn

================================================================================
来源：http://ec.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://du.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yu.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fg.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://ze.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://sw.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bu.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://dx.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fr.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rv.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://ut.colortex.cn

Py:   json.loads(s)
来源：http://ur.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bn.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://uh.panjiajie.cn

TS:   JSON.parse(s)
来源：http://oj.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rp.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://np.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://do.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wz.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://oz.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hg.szxytkj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://is.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://al.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bk.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kl.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hc.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uw.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tl.nicolike.cn

[K04] 读取 JSON 文件
来源：http://qp.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lr.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ec.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tg.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qp.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ma.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dk.nicolike.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wt.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bh.asd995.cn

[K05] 深拷贝对象
来源：http://qq.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://qe.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://wl.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://bz.colortex.cn

TS:   structuredClone(obj)
来源：http://bc.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jr.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pf.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ij.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dh.huixinmuqiang.cn

[K06] 解析 URL 查询串
来源：http://dl.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cd.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bs.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jp.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cm.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ud.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nd.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://by.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ex.szsharing.cn

[K07] 进制转换
来源：http://ud.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://to.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nq.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xc.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gb.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bt.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qv.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lc.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wh.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://ju.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://xb.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wx.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://ig.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://tv.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gb.521024.cn

Go:   encoding/gob
来源：http://pu.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://vd.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dh.haigaiapp.cn

================================================================================
来源：http://sa.huanxung.cn

L. 网络请求
来源：http://gy.shxzskj.cn

================================================================================
来源：http://iy.lnxyls.cn

[L01] 发送 GET 请求
来源：http://fv.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qq.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vn.szxytkj.cn

JS:   await fetch(url)
来源：http://ic.muxihuayi.cn

TS:   await fetch(url)
来源：http://vz.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://se.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://wb.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oj.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sk.shxzukj.cn

[L02] 发送 POST JSON
来源：http://lr.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tx.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qp.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cn.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uh.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ry.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ib.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cz.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sc.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://qa.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bm.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sj.hnjuh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zl.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bh.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pa.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mb.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bl.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ak.shtwfgs.cn

[L04] 设置超时
来源：http://hd.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://tb.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sy.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://am.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mf.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yh.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rm.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ke.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gp.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://hh.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jx.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uc.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qe.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://by.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cs.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wf.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ap.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jl.colortex.cn

[L06] 解析响应为 JSON
来源：http://aw.hnjuh.cn

Py:   resp.json()
来源：http://ts.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://lm.huixiangedu.cn

JS:   await resp.json()
来源：http://dp.lnxyls.cn

TS:   await resp.json()
来源：http://pm.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dy.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://re.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://ot.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jq.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://bq.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ow.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dq.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ri.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://tu.yuexingan06.cn

Java: resp.statusCode()
来源：http://jn.szxytkj.cn

Go:   resp.StatusCode
来源：http://yf.hnjuh.cn

Ruby: resp.code.to_i
来源：http://lp.panjiajie.cn

C#:   (int)resp.StatusCode
来源：http://uc.nicolike.cn

[L08] 并发请求多个地址
来源：http://je.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sy.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://at.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vw.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eu.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iu.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lk.shxzukj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dr.hahajie.cn

================================================================================
来源：http://zq.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://fk.panjiajie.cn

================================================================================
来源：http://sx.szxytkj.cn

[M01] 读取命令行参数
来源：http://fz.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://xs.hahajie.cn

PHP:  $argv;  $argc;
来源：http://np.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://vj.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://yj.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://oi.szsharing.cn

Go:   os.Args[1:]
来源：http://uh.shtwfgs.cn

Ruby: ARGV
来源：http://ka.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://fr.newstarts.cn

[M02] 读取环境变量
来源：http://wi.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://mx.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ns.nicolike.cn

JS:   process.env.HOME
来源：http://wo.szxytkj.cn

TS:   process.env.HOME
来源：http://xi.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://jq.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tl.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://fg.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xu.panjiajie.cn

[M03] 执行外部命令
来源：http://if.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yz.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jc.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qx.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zg.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jz.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cx.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pu.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://cr.asd995.cn

[M04] 获取当前工作目录
来源：http://oy.szxytkj.cn

Py:   os.getcwd()
来源：http://ts.colortex.cn

PHP:  getcwd();
来源：http://uw.nicolike.cn

JS:   process.cwd()
来源：http://ba.wgjwhj.cn

TS:   process.cwd()
来源：http://nu.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://od.colortex.cn

Go:   os.Getwd()
来源：http://bi.newstarts.cn

Ruby: Dir.pwd
来源：http://cv.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://py.chemitech.net.cn

[M05] 设置退出码
来源：http://ps.haigaiapp.cn

Py:   sys.exit(1)
来源：http://nx.9csxet.cn

PHP:  exit(1);
来源：http://ns.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://vf.9csxet.cn

TS:   process.exit(1)
来源：http://wt.9csxet.cn

Java: System.exit(1)
来源：http://do.newstarts.cn

Go:   os.Exit(1)
来源：http://ny.nicolike.cn

Ruby: exit 1
来源：http://pq.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jh.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ke.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://lc.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yh.shtwfgs.cn

JS:   console.error("err")
来源：http://dx.hahajie.cn

TS:   console.error("err")
来源：http://ex.lnxyls.cn

Java: System.err.println("err")
来源：http://sx.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gy.shxzskj.cn

Ruby: warn "err"
来源：http://jc.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://bf.colortex.cn

[M07] 判断是否为主入口
来源：http://tk.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://wb.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://av.panjiajie.cn

JS:   require.main === module
来源：http://rx.jianghongdianzi.cn

TS:   require.main === module
来源：http://sf.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://az.yuntaijiaju.cn

Go:   func main()
来源：http://sc.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://if.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://rf.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://kr.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://xv.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://oo.9csxet.cn

JS:   process.platform;  process.version
来源：http://fe.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://fe.yuexingan06.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pq.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dc.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pr.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ll.shtwfgs.cn

================================================================================
来源：http://vj.shtwfgs.cn

N. 数据结构与算法
来源：http://ty.shxzskj.cn

================================================================================
来源：http://mz.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://mm.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://at.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zh.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rs.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nk.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dt.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://fj.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ba.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pn.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://or.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ja.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vx.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ei.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://il.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bx.521024.cn

Go:   slices.Sort(arr)
来源：http://rq.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ak.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cm.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://sk.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vx.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://mz.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://up.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hc.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ec.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jq.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://te.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dc.huixiangedu.cn

[N04] 斐波那契数列
来源：http://om.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://em.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bg.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fu.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://an.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cl.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xh.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xn.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zn.hnjuh.cn

[N05] 最大公约数
来源：http://sx.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://xy.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dx.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pw.huanxung.cn


<!-- 参考信息 -->