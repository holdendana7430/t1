代发 wailian999

[J07] 比较两个日期
来源：http://ll.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yr.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ph.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gy.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lk.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xi.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bt.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vr.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://km.hahajie.cn

[J08] 提取年月日与星期
来源：http://rd.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ik.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eu.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ao.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dn.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xc.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://he.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ha.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bv.bookmarksfly.cn

[J09] 时区处理
来源：http://wq.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xq.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iu.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ao.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qa.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eq.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kj.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vd.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://yu.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jy.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rc.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ed.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tp.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://du.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tc.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kc.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sd.haigaiapp.cn

================================================================================
来源：http://ci.jianghongdianzi.cn

K. JSON 与序列化
来源：http://ky.colortex.cn

================================================================================
来源：http://di.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://qb.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sn.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ac.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://qw.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ta.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zj.asd995.cn

Go:   json.Marshal(obj)
来源：http://cu.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dq.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://si.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ey.newstarts.cn

Py:   json.loads(s)
来源：http://kr.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vy.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://wo.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://kv.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oy.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://lp.9csxet.cn

Ruby: JSON.parse(s)
来源：http://gh.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qz.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://xo.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hb.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vx.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aq.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yp.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sq.hnjuh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rx.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://py.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uo.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://lt.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://do.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nz.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ys.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ph.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://by.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hd.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rc.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wi.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://wt.huixinmuqiang.cn

Py:   copy.deepcopy(obj)
来源：http://ww.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://rt.asd995.cn

JS:   structuredClone(obj)
来源：http://oz.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://av.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ye.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yk.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fo.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vm.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://xd.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yh.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tg.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nl.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ty.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vm.jctech888.com.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ri.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sv.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vs.chemitech.net.cn

[K07] 进制转换
来源：http://so.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jz.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zo.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wu.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://za.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nt.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ns.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bj.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tu.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://kz.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://jx.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jx.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://om.yuexingan06.cn

TS:   v8.serialize(obj)        // Node
来源：http://op.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ot.asd995.cn

Go:   encoding/gob
来源：http://vg.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://bp.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mi.shtwfgs.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

L. 网络请求
来源：http://kq.hahajie.cn

================================================================================
来源：http://lo.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://am.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pk.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iu.haigaiapp.cn

JS:   await fetch(url)
来源：http://ds.yuexingan06.cn

TS:   await fetch(url)
来源：http://ls.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jn.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://ng.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rs.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cv.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://xn.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lc.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://up.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ae.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gd.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ad.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bx.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ax.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kh.panjiajie.cn

[L03] 设置自定义请求头
来源：http://hx.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ib.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ge.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ok.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uc.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dr.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nw.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ab.newstarts.cn

[L04] 设置超时
来源：http://ex.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://tz.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pd.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yx.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yg.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://of.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ql.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ad.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cd.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://ae.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ge.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://do.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qa.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://im.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wi.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ag.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eh.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qt.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ak.asd995.cn

Py:   resp.json()
来源：http://xp.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://wa.hnjuh.cn

JS:   await resp.json()
来源：http://mb.lnxyls.cn

TS:   await resp.json()
来源：http://nl.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://or.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://re.9csxet.cn

Ruby: JSON.parse(resp.body)
来源：http://uo.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fp.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://hz.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://py.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ax.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://br.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://ij.hahajie.cn

Java: resp.statusCode()
来源：http://bu.521024.cn

Go:   resp.StatusCode
来源：http://qs.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://cn.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://et.shxzskj.cn

[L08] 并发请求多个地址
来源：http://my.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wl.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ir.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://au.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xj.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ve.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nz.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://du.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gj.jianghongdianzi.cn

================================================================================
来源：http://qp.wgjwhj.cn

M. 命令行 / 进程 / 环境
来源：http://qd.nicolike.cn

================================================================================
来源：http://ud.hahajie.cn

[M01] 读取命令行参数
来源：http://bn.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://hk.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://wb.521024.cn

JS:   process.argv.slice(2)
来源：http://cd.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://vf.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://sz.gzmigu.cn

Go:   os.Args[1:]
来源：http://od.hnjuh.cn

Ruby: ARGV
来源：http://kp.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://op.9csxet.cn

[M02] 读取环境变量
来源：http://sq.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://fe.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yo.shtwfgs.cn

JS:   process.env.HOME
来源：http://lt.newstarts.cn

TS:   process.env.HOME
来源：http://jk.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://cl.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lg.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://pl.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://so.panjiajie.cn

[M03] 执行外部命令
来源：http://op.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qn.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fa.shtwfgs.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ty.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mv.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pk.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wr.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://al.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://wz.9csxet.cn

[M04] 获取当前工作目录
来源：http://yz.shxzukj.cn

Py:   os.getcwd()
来源：http://yp.hnjuh.cn

PHP:  getcwd();
来源：http://iy.huixinmuqiang.cn

JS:   process.cwd()
来源：http://tz.yuntaijiaju.cn

TS:   process.cwd()
来源：http://wt.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://gy.lnxyls.cn

Go:   os.Getwd()
来源：http://pj.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://so.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oj.9csxet.cn

[M05] 设置退出码
来源：http://py.521024.cn

Py:   sys.exit(1)
来源：http://nq.jianghongdianzi.cn

PHP:  exit(1);
来源：http://vj.521024.cn

JS:   process.exit(1)
来源：http://vd.shtwfgs.cn

TS:   process.exit(1)
来源：http://kl.shtwfgs.cn

Java: System.exit(1)
来源：http://kh.bjjhwx.cn

Go:   os.Exit(1)
来源：http://ox.gzmigu.cn

Ruby: exit 1
来源：http://el.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ic.haigaiapp.cn

[M06] 向标准错误输出
来源：http://gt.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://zh.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fc.lnxyls.cn

JS:   console.error("err")
来源：http://dw.haigaiapp.cn

TS:   console.error("err")
来源：http://vs.newstarts.cn

Java: System.err.println("err")
来源：http://mf.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tp.newstarts.cn

Ruby: warn "err"
来源：http://le.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://jq.szsharing.cn

[M07] 判断是否为主入口
来源：http://jf.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://cu.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kv.gzmigu.cn

JS:   require.main === module
来源：http://ex.huixiangedu.cn

TS:   require.main === module
来源：http://dh.9csxet.cn

Java: public static void main(String[] args)
来源：http://sc.nszjky.cn

Go:   func main()
来源：http://pt.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kb.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://lc.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://wi.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://xs.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://pk.hnjuh.cn

JS:   process.platform;  process.version
来源：http://bs.asd995.cn

TS:   process.platform;  process.version
来源：http://bq.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zy.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nw.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uz.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fb.haigaiapp.cn

================================================================================
来源：http://uy.szsharing.cn

N. 数据结构与算法
来源：http://jj.shxzukj.cn

================================================================================
来源：http://ez.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://dd.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ao.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://of.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pd.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ue.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gd.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://cp.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mb.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ga.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://da.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://kh.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xr.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lk.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fa.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ft.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://on.shxzukj.cn

Ruby: arr.sort
来源：http://ra.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xe.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://hr.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zd.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://mx.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dt.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bd.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://il.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zf.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dd.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qv.hahajie.cn

[N04] 斐波那契数列
来源：http://mp.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://br.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://de.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hu.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qn.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eg.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cx.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bk.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cr.shxzukj.cn


<!-- 参考信息 -->