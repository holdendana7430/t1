代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rn.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rf.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vb.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hr.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ao.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pb.nszjky.cn

[J09] 时区处理
来源：http://aa.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://is.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yg.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bx.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bm.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bi.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wd.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ir.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://jj.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zj.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yt.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dm.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jl.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xy.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sk.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bh.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oz.huixinmuqiang.cn

================================================================================
来源：http://td.nicolike.cn

K. JSON 与序列化
来源：http://ab.shxzukj.cn

================================================================================
来源：http://uz.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://fm.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sm.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wx.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://xj.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://xv.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pg.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://uv.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://at.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pr.colortex.cn

[K02] JSON 字符串转对象
来源：http://qs.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://bk.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ak.521024.cn

JS:   JSON.parse(s)
来源：http://iw.szxytkj.cn

TS:   JSON.parse(s)
来源：http://wc.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://wd.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://zb.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gk.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hj.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qn.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fi.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cc.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://up.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pm.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mn.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://og.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eb.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fi.muxihuayi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gg.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ga.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ov.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fc.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ts.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ao.colortex.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://te.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dh.jctech888.com.cn

[K05] 深拷贝对象
来源：http://fe.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://zo.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://eu.gzmigu.cn

JS:   structuredClone(obj)
来源：http://wh.nicolike.cn

TS:   structuredClone(obj)
来源：http://ab.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ic.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nq.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://or.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lj.newstarts.cn

[K06] 解析 URL 查询串
来源：http://nr.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ov.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wm.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://of.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zz.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oa.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pt.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wh.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://et.wgjwhj.cn

[K07] 进制转换
来源：http://qe.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uw.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pu.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rc.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://du.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rp.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jh.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nf.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qf.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://aw.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://cg.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rk.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://zq.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://sh.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hh.haigaiapp.cn

Go:   encoding/gob
来源：http://kv.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://fu.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gr.newstarts.cn

================================================================================
来源：http://de.panjiajie.cn

L. 网络请求
来源：http://pt.lnxyls.cn

================================================================================
来源：http://xh.hahajie.cn

[L01] 发送 GET 请求
来源：http://hi.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://si.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zk.huixiangedu.cn

JS:   await fetch(url)
来源：http://et.bjjhwx.cn

TS:   await fetch(url)
来源：http://ob.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://td.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://pr.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kc.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xe.hnjuh.cn

[L02] 发送 POST JSON
来源：http://zo.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hv.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pz.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://im.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nl.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://df.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ei.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nx.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://sr.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vq.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kl.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pc.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ui.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aa.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wg.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iw.jianghongdianzi.cn

[L04] 设置超时
来源：http://gt.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ha.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cf.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vs.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fz.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tw.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ui.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://md.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gv.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://pg.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ie.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zj.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wk.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sa.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://im.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://la.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ph.nszjky.cn

[L06] 解析响应为 JSON
来源：http://am.hnjuh.cn

Py:   resp.json()
来源：http://jl.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://pc.huixiangedu.cn

JS:   await resp.json()
来源：http://hs.yuntaijiaju.cn

TS:   await resp.json()
来源：http://bv.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://br.muxihuayi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hv.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://qs.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ig.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ph.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hj.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qw.colortex.cn

JS:   resp.ok;  resp.status
来源：http://aq.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://jk.9csxet.cn

Java: resp.statusCode()
来源：http://vv.hnjuh.cn

Go:   resp.StatusCode
来源：http://rq.newstarts.cn

Ruby: resp.code.to_i
来源：http://ub.colortex.cn

C#:   (int)resp.StatusCode
来源：http://nd.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://ah.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gg.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ee.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fp.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jb.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aa.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oh.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nv.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dq.panjiajie.cn

================================================================================
来源：http://qi.hnjuh.cn

M. 命令行 / 进程 / 环境
来源：http://lt.szsharing.cn

================================================================================
来源：http://pw.9csxet.cn

[M01] 读取命令行参数
来源：http://kc.asd995.cn

Py:   sys.argv[1:]
来源：http://ng.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://jz.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://fm.hahajie.cn

TS:   process.argv.slice(2)
来源：http://kd.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://bc.yuexingan06.cn

Go:   os.Args[1:]
来源：http://oo.chemitech.net.cn

Ruby: ARGV
来源：http://jd.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://ts.lnxyls.cn

[M02] 读取环境变量
来源：http://rw.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://cu.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uf.bookmarksfly.cn

JS:   process.env.HOME
来源：http://ku.shtwfgs.cn

TS:   process.env.HOME
来源：http://uy.panjiajie.cn

Java: System.getenv("HOME")
来源：http://gj.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fi.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://nv.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bz.haigaiapp.cn

[M03] 执行外部命令
来源：http://mv.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://be.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yx.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zm.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ay.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ob.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ah.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qh.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://qp.nicolike.cn

[M04] 获取当前工作目录
来源：http://vw.shtwfgs.cn

Py:   os.getcwd()
来源：http://wq.wgjwhj.cn

PHP:  getcwd();
来源：http://sh.panjiajie.cn

JS:   process.cwd()
来源：http://au.chemitech.net.cn

TS:   process.cwd()
来源：http://ds.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wa.bjjhwx.cn

Go:   os.Getwd()
来源：http://ce.521024.cn

Ruby: Dir.pwd
来源：http://ri.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://op.haigaiapp.cn

[M05] 设置退出码
来源：http://fn.huixiangedu.cn

Py:   sys.exit(1)
来源：http://rp.asd995.cn

PHP:  exit(1);
来源：http://ij.hahajie.cn

JS:   process.exit(1)
来源：http://uj.lnxyls.cn

TS:   process.exit(1)
来源：http://di.shxzukj.cn

Java: System.exit(1)
来源：http://tk.yuexingan06.cn

Go:   os.Exit(1)
来源：http://hr.muxihuayi.cn

Ruby: exit 1
来源：http://gx.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ot.hahajie.cn

[M06] 向标准错误输出
来源：http://lc.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://if.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://on.9csxet.cn

JS:   console.error("err")
来源：http://iv.shtwfgs.cn

TS:   console.error("err")
来源：http://ot.gzmigu.cn

Java: System.err.println("err")
来源：http://lp.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ve.gzmigu.cn

Ruby: warn "err"
来源：http://an.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://na.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://ly.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://tm.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aj.yuexingan06.cn

JS:   require.main === module
来源：http://rm.colortex.cn

TS:   require.main === module
来源：http://ir.nszjky.cn

Java: public static void main(String[] args)
来源：http://xh.hnjuh.cn

Go:   func main()
来源：http://gb.asd995.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vj.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ob.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://zi.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://pt.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://ka.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ww.shxzskj.cn

TS:   process.platform;  process.version
来源：http://rf.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ct.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iy.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wv.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wv.yuntaijiaju.cn

================================================================================
来源：http://rj.shxzukj.cn

N. 数据结构与算法
来源：http://xp.newstarts.cn

================================================================================
来源：http://sr.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://st.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yy.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fe.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wc.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rr.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wq.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://si.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rt.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bs.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://yt.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://nv.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xa.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lo.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yb.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zq.521024.cn

Go:   slices.Sort(arr)
来源：http://yn.shxzukj.cn

Ruby: arr.sort
来源：http://xm.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tu.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://bw.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wq.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://pd.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ph.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cd.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fs.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zj.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cl.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vw.yuexingan06.cn

[N04] 斐波那契数列
来源：http://cv.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zv.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ez.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yx.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tf.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tx.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://as.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cu.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ta.bjjhwx.cn

[N05] 最大公约数
来源：http://ff.newstarts.cn

Py:   math.gcd(a, b)
来源：http://ev.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gi.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uh.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ny.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lk.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zr.szsharing.cn

Ruby: a.gcd(b)
来源：http://gl.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qm.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://vr.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://cz.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://ik.huixinmuqiang.cn


<!-- 参考信息 -->