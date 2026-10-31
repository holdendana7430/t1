代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://qx.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pd.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ki.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://rp.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ss.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qz.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gj.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iw.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dq.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wf.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hw.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sp.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uj.chemitech.net.cn

[J09] 时区处理
来源：http://fa.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vx.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qq.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jl.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lg.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fo.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xy.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://da.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pm.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://vx.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dq.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nf.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ti.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pu.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nb.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wj.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://un.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lg.shtwfgs.cn

================================================================================
来源：http://gu.szxytkj.cn

K. JSON 与序列化
来源：http://ms.bjjhwx.cn

================================================================================
来源：http://cz.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://lq.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ah.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jj.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://xl.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://pq.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://po.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://lh.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://it.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ch.asd995.cn

[K02] JSON 字符串转对象
来源：http://aw.nicolike.cn

Py:   json.loads(s)
来源：http://yq.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ui.panjiajie.cn

JS:   JSON.parse(s)
来源：http://hi.gzmigu.cn

TS:   JSON.parse(s)
来源：http://hp.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xh.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://uo.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://wu.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zm.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://le.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zh.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nx.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cf.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qh.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bm.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://su.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eb.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ke.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://du.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://na.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qr.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fy.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://so.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mp.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aj.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://og.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ua.shtwfgs.cn

[K05] 深拷贝对象
来源：http://lr.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://qa.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ll.asd995.cn

JS:   structuredClone(obj)
来源：http://nb.shxzskj.cn

TS:   structuredClone(obj)
来源：http://zl.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tm.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ag.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nl.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pu.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://gy.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cq.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://np.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hr.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ap.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ua.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kp.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ry.nicolike.cn

[K07] 进制转换
来源：http://zv.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zx.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aw.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ct.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wo.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://df.colortex.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fu.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xg.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ty.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://vi.bjjhwx.cn

Py:   pickle.dumps(obj)
来源：http://hd.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vj.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://ag.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://pl.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://az.szxytkj.cn

Go:   encoding/gob
来源：http://xh.gzmigu.cn

Ruby: Marshal.dump(obj)
来源：http://gy.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ql.yuexingan06.cn

================================================================================
来源：http://hl.hahajie.cn

L. 网络请求
来源：http://yf.newstarts.cn

================================================================================
来源：http://zb.lnxyls.cn

[L01] 发送 GET 请求
来源：http://wr.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jo.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lz.gzmigu.cn

JS:   await fetch(url)
来源：http://wr.nicolike.cn

TS:   await fetch(url)
来源：http://gg.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hb.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://cf.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qp.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sr.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://gg.bjjhwx.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yq.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hc.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fq.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tc.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://st.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bh.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qc.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ok.9csxet.cn

[L03] 设置自定义请求头
来源：http://pe.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ot.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ag.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hy.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vv.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hk.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://al.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mg.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ra.yuexingan06.cn

[L04] 设置超时
来源：http://rs.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://cu.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://te.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zj.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tg.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://th.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bf.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vj.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pn.hahajie.cn

[L05] 上传文件（multipart）
来源：http://ju.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://st.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jr.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mp.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kr.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rm.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jf.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://en.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://di.szsharing.cn

Py:   resp.json()
来源：http://rv.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ok.bjjhwx.cn

JS:   await resp.json()
来源：http://vk.huanxung.cn

TS:   await resp.json()
来源：http://dj.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ju.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nv.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://lt.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ml.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://io.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vn.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lk.asd995.cn

JS:   resp.ok;  resp.status
来源：http://is.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://qt.yuexingan06.cn

Java: resp.statusCode()
来源：http://yq.newstarts.cn

Go:   resp.StatusCode
来源：http://rp.shxzskj.cn

Ruby: resp.code.to_i
来源：http://qw.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://fc.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://ac.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://es.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://bd.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rv.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qe.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fo.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gx.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://it.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mb.jctech888.com.cn

================================================================================
来源：http://qk.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://qb.jctech888.com.cn

================================================================================
来源：http://md.lnxyls.cn

[M01] 读取命令行参数
来源：http://dp.nicolike.cn

Py:   sys.argv[1:]
来源：http://be.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://ty.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://rj.newstarts.cn

TS:   process.argv.slice(2)
来源：http://wr.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://uv.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://sd.huixiangedu.cn

Ruby: ARGV
来源：http://vb.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://ee.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://xv.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://fc.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yu.jianghongdianzi.cn

JS:   process.env.HOME
来源：http://de.nicolike.cn

TS:   process.env.HOME
来源：http://ys.szsharing.cn

Java: System.getenv("HOME")
来源：http://mu.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cv.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://qf.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gc.hnjuh.cn

[M03] 执行外部命令
来源：http://vm.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vp.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rj.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jh.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://or.521024.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wg.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uh.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ls.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://po.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://ll.asd995.cn

Py:   os.getcwd()
来源：http://ro.bjjhwx.cn

PHP:  getcwd();
来源：http://ry.bookmarksfly.cn

JS:   process.cwd()
来源：http://zl.szxytkj.cn

TS:   process.cwd()
来源：http://ao.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ro.yuexingan06.cn

Go:   os.Getwd()
来源：http://bo.shxzukj.cn

Ruby: Dir.pwd
来源：http://oi.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xz.9csxet.cn

[M05] 设置退出码
来源：http://ro.szsharing.cn

Py:   sys.exit(1)
来源：http://lt.huanxung.cn

PHP:  exit(1);
来源：http://ji.bookmarksfly.cn

JS:   process.exit(1)
来源：http://fa.yuexingan06.cn

TS:   process.exit(1)
来源：http://gn.newstarts.cn

Java: System.exit(1)
来源：http://uf.yuexingan06.cn

Go:   os.Exit(1)
来源：http://ef.jianghongdianzi.cn

Ruby: exit 1
来源：http://kk.colortex.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qv.panjiajie.cn

[M06] 向标准错误输出
来源：http://ae.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://fn.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ya.lnxyls.cn

JS:   console.error("err")
来源：http://in.haigaiapp.cn

TS:   console.error("err")
来源：http://lj.521024.cn

Java: System.err.println("err")
来源：http://yn.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rf.shtwfgs.cn

Ruby: warn "err"
来源：http://pi.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://up.hahajie.cn

[M07] 判断是否为主入口
来源：http://bo.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://yy.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hf.bookmarksfly.cn

JS:   require.main === module
来源：http://da.colortex.cn

TS:   require.main === module
来源：http://jv.panjiajie.cn

Java: public static void main(String[] args)
来源：http://en.hnjuh.cn

Go:   func main()
来源：http://jp.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uf.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://wy.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://sz.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://km.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ek.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://go.huanxung.cn

TS:   process.platform;  process.version
来源：http://qn.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xe.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oy.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iu.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://en.shxzukj.cn

================================================================================
来源：http://ql.bookmarksfly.cn

N. 数据结构与算法
来源：http://ds.bjjhwx.cn

================================================================================
来源：http://zs.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://xh.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wb.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bk.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lv.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cv.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wa.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://yq.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tw.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rn.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://mw.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://xg.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cm.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tm.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hd.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vr.colortex.cn

Go:   slices.Sort(arr)
来源：http://mf.shtwfgs.cn

Ruby: arr.sort
来源：http://cr.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gw.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://xl.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hr.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ct.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gr.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xr.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jw.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wi.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ny.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xy.shtwfgs.cn

[N04] 斐波那契数列
来源：http://td.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pj.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mp.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pb.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bu.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nt.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cu.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xi.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xa.szsharing.cn

[N05] 最大公约数
来源：http://cb.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://ja.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jl.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pq.panjiajie.cn


<!-- 参考信息 -->