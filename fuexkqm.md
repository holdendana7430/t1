代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://re.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://am.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xz.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jh.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://nr.521024.cn

[J08] 提取年月日与星期
来源：http://uw.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pq.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bi.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eh.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bv.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hx.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ao.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ug.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vu.bjjhwx.cn

[J09] 时区处理
来源：http://dx.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ys.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mm.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://go.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://il.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ki.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ar.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xu.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vi.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://bh.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xo.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mm.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ut.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pq.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://io.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ow.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jn.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uk.muxihuayi.cn

================================================================================
来源：http://ea.yuntaijiaju.cn

K. JSON 与序列化
来源：http://gt.gzmigu.cn

================================================================================
来源：http://ql.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://je.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ut.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pj.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://xr.asd995.cn

TS:   JSON.stringify(obj)
来源：http://xc.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://po.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://fo.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nr.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dr.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://sq.panjiajie.cn

Py:   json.loads(s)
来源：http://ka.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uu.panjiajie.cn

JS:   JSON.parse(s)
来源：http://ny.asd995.cn

TS:   JSON.parse(s)
来源：http://et.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zl.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://sd.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://yj.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xp.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://ag.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mr.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lq.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sr.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fq.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://km.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yo.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gv.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mk.huanxung.cn

[K04] 读取 JSON 文件
来源：http://wd.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zy.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fi.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qf.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zk.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nx.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zc.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yf.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pk.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://xb.nszjky.cn

Py:   copy.deepcopy(obj)
来源：http://jl.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://tf.shxzskj.cn

JS:   structuredClone(obj)
来源：http://qi.shxzskj.cn

TS:   structuredClone(obj)
来源：http://id.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yd.chemitech.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jc.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://en.shtwfgs.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yk.9csxet.cn

[K06] 解析 URL 查询串
来源：http://ud.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dr.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lw.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lr.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fy.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ry.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yc.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ph.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zz.huanxung.cn

[K07] 进制转换
来源：http://mj.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rj.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bc.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ir.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ax.asd995.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wg.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tm.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nt.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rk.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://gm.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://il.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ub.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://jn.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ec.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zs.haigaiapp.cn

Go:   encoding/gob
来源：http://ng.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://sp.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ux.newstarts.cn

================================================================================
来源：http://gz.nszjky.cn

L. 网络请求
来源：http://sv.9csxet.cn

================================================================================
来源：http://pt.shxzukj.cn

[L01] 发送 GET 请求
来源：http://la.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vx.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qw.jctech888.com.cn

JS:   await fetch(url)
来源：http://yi.nszjky.cn

TS:   await fetch(url)
来源：http://mw.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qu.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://et.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vk.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lv.shxzskj.cn

[L02] 发送 POST JSON
来源：http://zm.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dk.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ww.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nx.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fw.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bd.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yq.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yu.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://em.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://yh.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jp.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gg.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ya.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gn.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bl.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ek.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qw.nicolike.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bo.nszjky.cn

[L04] 设置超时
来源：http://oo.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://ek.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yw.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kl.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xl.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tz.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pd.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zk.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mh.nicolike.cn

[L05] 上传文件（multipart）
来源：http://ob.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yw.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dg.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ad.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xi.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vr.nszjky.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ho.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sj.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rs.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://ws.nszjky.cn

Py:   resp.json()
来源：http://xp.huanxung.cn

PHP:  json_decode($body, true);
来源：http://ss.shtwfgs.cn

JS:   await resp.json()
来源：http://hj.huanxung.cn

TS:   await resp.json()
来源：http://pl.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://go.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oo.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://eq.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rd.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://ec.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vk.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rg.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://ss.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://de.nicolike.cn

Java: resp.statusCode()
来源：http://yj.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://dd.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://eo.asd995.cn

C#:   (int)resp.StatusCode
来源：http://tf.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://ra.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ix.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://hw.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://th.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bo.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tn.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cf.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://us.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pa.bjjhwx.cn

================================================================================
来源：http://en.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://vm.haigaiapp.cn

================================================================================
来源：http://zg.yuexingan06.cn

[M01] 读取命令行参数
来源：http://hc.521024.cn

Py:   sys.argv[1:]
来源：http://eo.szsharing.cn

PHP:  $argv;  $argc;
来源：http://qz.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://un.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://ii.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://cs.colortex.cn

Go:   os.Args[1:]
来源：http://ng.bookmarksfly.cn

Ruby: ARGV
来源：http://wr.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://xa.wgjwhj.cn

[M02] 读取环境变量
来源：http://yx.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://rc.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pc.huanxung.cn

JS:   process.env.HOME
来源：http://yx.9csxet.cn

TS:   process.env.HOME
来源：http://gw.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://zd.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qz.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://qm.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mz.yuexingan06.cn

[M03] 执行外部命令
来源：http://vu.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bc.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lp.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jy.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kv.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://la.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cx.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vr.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://lx.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://eo.jctech888.com.cn

Py:   os.getcwd()
来源：http://zk.bjjhwx.cn

PHP:  getcwd();
来源：http://us.szxytkj.cn

JS:   process.cwd()
来源：http://ce.jctech888.com.cn

TS:   process.cwd()
来源：http://ou.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://xs.jctech888.com.cn

Go:   os.Getwd()
来源：http://yo.muxihuayi.cn

Ruby: Dir.pwd
来源：http://vq.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rs.shxzukj.cn

[M05] 设置退出码
来源：http://tu.newstarts.cn

Py:   sys.exit(1)
来源：http://lk.panjiajie.cn

PHP:  exit(1);
来源：http://so.muxihuayi.cn

JS:   process.exit(1)
来源：http://su.bjjhwx.cn

TS:   process.exit(1)
来源：http://iu.gzmigu.cn

Java: System.exit(1)
来源：http://dm.haigaiapp.cn

Go:   os.Exit(1)
来源：http://at.szsharing.cn

Ruby: exit 1
来源：http://oo.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rp.haigaiapp.cn

[M06] 向标准错误输出
来源：http://my.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://uo.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://us.gzmigu.cn

JS:   console.error("err")
来源：http://jk.huanxung.cn

TS:   console.error("err")
来源：http://fo.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ec.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://im.hahajie.cn

Ruby: warn "err"
来源：http://vn.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://qk.lnxyls.cn

[M07] 判断是否为主入口
来源：http://og.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://zz.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zm.szsharing.cn

JS:   require.main === module
来源：http://hy.muxihuayi.cn

TS:   require.main === module
来源：http://vo.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://if.newstarts.cn

Go:   func main()
来源：http://wb.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nw.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://ew.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://qw.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://bx.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://jt.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://fg.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://yx.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jv.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xw.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eb.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dy.shtwfgs.cn

================================================================================
来源：http://bk.huanxung.cn

N. 数据结构与算法
来源：http://fy.521024.cn

================================================================================
来源：http://mf.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://hy.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ae.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jo.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vb.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fi.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://xm.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://to.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kn.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://hs.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://sb.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uw.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fp.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vf.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yj.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://nq.nicolike.cn

Ruby: arr.sort
来源：http://hp.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bq.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://rr.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nh.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://py.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ub.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yh.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fm.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qz.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tw.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qx.9csxet.cn

[N04] 斐波那契数列
来源：http://yh.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yn.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fm.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dm.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nx.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nc.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wa.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uw.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://me.gzmigu.cn

[N05] 最大公约数
来源：http://lf.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://yi.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uq.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tu.bookmarksfly.cn


<!-- 参考信息 -->