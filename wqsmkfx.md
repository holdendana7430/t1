代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fl.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fu.haigaiapp.cn

[J09] 时区处理
来源：http://cm.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://in.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wi.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jb.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://co.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://an.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ln.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://si.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://nc.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wn.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jf.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vf.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jt.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gy.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tx.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ox.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cr.chemitech.net.cn

================================================================================
来源：http://gi.shxzukj.cn

K. JSON 与序列化
来源：http://ej.nicolike.cn

================================================================================
来源：http://qs.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://gi.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lo.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rl.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ll.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://sp.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ui.colortex.cn

Go:   json.Marshal(obj)
来源：http://vh.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iv.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://od.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://hf.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://re.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bz.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://ea.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://jl.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uw.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://hr.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://rn.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qm.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://eo.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dd.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qj.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kk.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lw.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ii.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sj.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wv.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://it.newstarts.cn

[K04] 读取 JSON 文件
来源：http://aj.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://th.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://le.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sn.gzmigu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://te.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ue.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wz.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xf.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gv.chemitech.net.cn

[K05] 深拷贝对象
来源：http://fc.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://kz.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://br.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://as.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://wb.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ft.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://of.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://te.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tz.chemitech.net.cn

[K06] 解析 URL 查询串
来源：http://jy.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hy.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zk.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ss.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xi.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hg.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ub.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gu.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fu.nszjky.cn

[K07] 进制转换
来源：http://gp.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ae.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vs.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://px.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hw.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://go.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vz.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ji.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://op.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://nu.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://le.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pd.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://li.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://sj.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wp.asd995.cn

Go:   encoding/gob
来源：http://xt.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://rc.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qh.huixiangedu.cn

================================================================================
来源：http://cy.huanxung.cn

L. 网络请求
来源：http://na.huixiangedu.cn

================================================================================
来源：http://xk.521024.cn

[L01] 发送 GET 请求
来源：http://nj.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vr.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ye.hnjuh.cn

JS:   await fetch(url)
来源：http://am.szxytkj.cn

TS:   await fetch(url)
来源：http://pk.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fb.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://sa.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lm.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ex.asd995.cn

[L02] 发送 POST JSON
来源：http://pv.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eo.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bf.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://je.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nb.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dc.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iq.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ra.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ab.newstarts.cn

[L03] 设置自定义请求头
来源：http://mi.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://by.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ps.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pz.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gr.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wa.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qb.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ro.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ks.huixinmuqiang.cn

[L04] 设置超时
来源：http://if.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://nz.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cp.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wi.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ph.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nm.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xn.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gy.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qx.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://na.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zs.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qm.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ma.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vm.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yx.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rw.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hq.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lb.9csxet.cn

[L06] 解析响应为 JSON
来源：http://xp.chemitech.net.cn

Py:   resp.json()
来源：http://lu.wgjwhj.cn

PHP:  json_decode($body, true);
来源：http://xz.chemitech.net.cn

JS:   await resp.json()
来源：http://ba.panjiajie.cn

TS:   await resp.json()
来源：http://um.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qu.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zo.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://sw.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nj.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://un.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ht.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lb.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://wk.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://zz.colortex.cn

Java: resp.statusCode()
来源：http://nk.jctech888.com.cn

Go:   resp.StatusCode
来源：http://kc.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://ca.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://zv.shxzskj.cn

[L08] 并发请求多个地址
来源：http://pz.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bj.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://bg.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eh.lnxyls.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sx.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pq.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lx.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://om.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wz.jianghongdianzi.cn

================================================================================
来源：http://bo.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://sz.521024.cn

================================================================================
来源：http://rx.jctech888.com.cn

[M01] 读取命令行参数
来源：http://jt.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://wi.nszjky.cn

PHP:  $argv;  $argc;
来源：http://dn.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://dd.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://lf.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://ua.bjjhwx.cn

Go:   os.Args[1:]
来源：http://uq.shxzukj.cn

Ruby: ARGV
来源：http://jk.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://dr.9csxet.cn

[M02] 读取环境变量
来源：http://za.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://yp.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ny.hnjuh.cn

JS:   process.env.HOME
来源：http://dn.shtwfgs.cn

TS:   process.env.HOME
来源：http://xb.9csxet.cn

Java: System.getenv("HOME")
来源：http://wg.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://az.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ra.shtwfgs.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hx.yuexingan06.cn

[M03] 执行外部命令
来源：http://tp.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cu.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ub.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yj.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jk.muxihuayi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xw.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ek.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uh.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://mh.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://hp.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://fw.lnxyls.cn

PHP:  getcwd();
来源：http://hh.9csxet.cn

JS:   process.cwd()
来源：http://wt.huixinmuqiang.cn

TS:   process.cwd()
来源：http://ev.huixinmuqiang.cn

Java: Path.of("").toAbsolutePath()
来源：http://pu.bjjhwx.cn

Go:   os.Getwd()
来源：http://xc.chemitech.net.cn

Ruby: Dir.pwd
来源：http://ko.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mc.bjjhwx.cn

[M05] 设置退出码
来源：http://gt.lnxyls.cn

Py:   sys.exit(1)
来源：http://cr.bookmarksfly.cn

PHP:  exit(1);
来源：http://bq.wgjwhj.cn

JS:   process.exit(1)
来源：http://ve.yuexingan06.cn

TS:   process.exit(1)
来源：http://lo.shxzskj.cn

Java: System.exit(1)
来源：http://nz.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://hj.hahajie.cn

Ruby: exit 1
来源：http://hz.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bp.huanxung.cn

[M06] 向标准错误输出
来源：http://dv.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://sh.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://px.bookmarksfly.cn

JS:   console.error("err")
来源：http://mi.bookmarksfly.cn

TS:   console.error("err")
来源：http://uu.shxzukj.cn

Java: System.err.println("err")
来源：http://hw.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vx.9csxet.cn

Ruby: warn "err"
来源：http://rq.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://us.nszjky.cn

[M07] 判断是否为主入口
来源：http://mf.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://qw.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gx.haigaiapp.cn

JS:   require.main === module
来源：http://ip.nszjky.cn

TS:   require.main === module
来源：http://za.newstarts.cn

Java: public static void main(String[] args)
来源：http://dq.shxzukj.cn

Go:   func main()
来源：http://vr.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ly.huanxung.cn

C#:   static void Main(string[] args)
来源：http://te.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://fp.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://nh.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://lw.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://ea.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://xy.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vv.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ak.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lj.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tx.gzmigu.cn

================================================================================
来源：http://em.bjjhwx.cn

N. 数据结构与算法
来源：http://px.huanxung.cn

================================================================================
来源：http://hf.colortex.cn

[N01] 二分查找（有序数组）
来源：http://ra.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sa.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mo.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lh.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ir.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ds.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://ou.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tf.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://va.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://na.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://ec.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ss.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ag.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gp.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pa.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://qo.hnjuh.cn

Ruby: arr.sort
来源：http://fw.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://az.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://bm.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://du.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://ah.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cg.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yl.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sp.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ct.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://le.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cy.lnxyls.cn

[N04] 斐波那契数列
来源：http://cg.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kb.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rk.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pc.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zn.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mj.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oj.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kd.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sk.huixinmuqiang.cn

[N05] 最大公约数
来源：http://vy.colortex.cn

Py:   math.gcd(a, b)
来源：http://jk.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dl.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kf.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vw.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tv.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lh.shxzukj.cn

Ruby: a.gcd(b)
来源：http://zg.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ue.wgjwhj.cn

[N06] 判断回文字符串
来源：http://ca.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ym.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://ni.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://gx.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://sa.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://db.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://uq.newstarts.cn


<!-- 参考信息 -->