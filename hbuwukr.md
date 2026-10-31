代发 wailian999

[J07] 比较两个日期
来源：http://mh.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://xs.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gm.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ej.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kt.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ed.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sw.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pj.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://vf.szxytkj.cn

[J08] 提取年月日与星期
来源：http://uf.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cv.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ft.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sw.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bf.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bu.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oj.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ne.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wq.shxzukj.cn

[J09] 时区处理
来源：http://eu.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gr.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fl.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lg.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ci.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://te.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jl.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xs.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zu.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://jy.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wp.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fp.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yo.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://li.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fe.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fv.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wa.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://la.huanxung.cn

================================================================================
来源：http://ya.hnjuh.cn

K. JSON 与序列化
来源：http://sp.nicolike.cn

================================================================================
来源：http://pr.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://pa.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vt.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ip.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://jt.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ns.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sh.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://ti.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cs.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ac.szsharing.cn

[K02] JSON 字符串转对象
来源：http://uf.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://yd.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iu.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ef.asd995.cn

TS:   JSON.parse(s)
来源：http://mu.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://th.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://wy.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://gn.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://re.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ky.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mt.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://za.bookmarksfly.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bm.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ln.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iq.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nt.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://am.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pm.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://ep.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vr.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uj.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jx.szxytkj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qm.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lz.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nd.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vg.asd995.cn

[K05] 深拷贝对象
来源：http://aw.muxihuayi.cn

Py:   copy.deepcopy(obj)
来源：http://do.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://uf.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://kn.szxytkj.cn

TS:   structuredClone(obj)
来源：http://nr.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xm.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rn.szsharing.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jf.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://va.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://na.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yy.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://er.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xg.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tj.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rr.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ur.muxihuayi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://he.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bp.colortex.cn

[K07] 进制转换
来源：http://jv.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jj.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aw.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vy.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nj.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zf.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://il.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sx.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xw.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://le.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://gt.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hk.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://ju.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://lq.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sq.szxytkj.cn

Go:   encoding/gob
来源：http://nr.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://rh.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ws.shxzskj.cn

================================================================================
来源：http://pp.nicolike.cn

L. 网络请求
来源：http://kh.huanxung.cn

================================================================================
来源：http://fb.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://rh.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ih.nszjky.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ky.muxihuayi.cn

JS:   await fetch(url)
来源：http://hm.huanxung.cn

TS:   await fetch(url)
来源：http://xi.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tc.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://tm.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zc.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jr.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://zq.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zz.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ga.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hk.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oo.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hf.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nd.9csxet.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ck.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pj.hahajie.cn

[L03] 设置自定义请求头
来源：http://px.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://py.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://in.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dy.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gg.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nf.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gh.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qi.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kz.gzmigu.cn

[L04] 设置超时
来源：http://jd.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://ex.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hn.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aw.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fc.hahajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://de.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zi.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fd.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rv.szsharing.cn

[L05] 上传文件（multipart）
来源：http://sh.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yw.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://we.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://od.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tu.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sn.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ix.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kq.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lu.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://hk.gzmigu.cn

Py:   resp.json()
来源：http://ua.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://jj.jctech888.com.cn

JS:   await resp.json()
来源：http://ha.asd995.cn

TS:   await resp.json()
来源：http://up.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://db.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wc.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://rf.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iw.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://qi.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qn.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ex.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://ch.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://aj.nicolike.cn

Java: resp.statusCode()
来源：http://id.szxytkj.cn

Go:   resp.StatusCode
来源：http://lj.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://go.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://cq.colortex.cn

[L08] 并发请求多个地址
来源：http://uc.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gj.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://ts.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pm.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yw.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tr.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://df.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ny.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ux.lnxyls.cn

================================================================================
来源：http://lx.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ze.shxzukj.cn

================================================================================
来源：http://nq.lnxyls.cn

[M01] 读取命令行参数
来源：http://gm.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://of.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://jz.newstarts.cn

JS:   process.argv.slice(2)
来源：http://lk.huanxung.cn

TS:   process.argv.slice(2)
来源：http://kj.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://qq.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://dy.lnxyls.cn

Ruby: ARGV
来源：http://xi.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://wv.muxihuayi.cn

[M02] 读取环境变量
来源：http://ua.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://ca.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wq.lnxyls.cn

JS:   process.env.HOME
来源：http://gu.shxzskj.cn

TS:   process.env.HOME
来源：http://ou.521024.cn

Java: System.getenv("HOME")
来源：http://mf.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yl.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://kg.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qk.hahajie.cn

[M03] 执行外部命令
来源：http://te.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vb.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nx.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gi.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ct.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ut.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jq.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aj.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://sn.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ru.muxihuayi.cn

Py:   os.getcwd()
来源：http://jq.hahajie.cn

PHP:  getcwd();
来源：http://zr.szxytkj.cn

JS:   process.cwd()
来源：http://fh.szsharing.cn

TS:   process.cwd()
来源：http://me.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://kn.haigaiapp.cn

Go:   os.Getwd()
来源：http://vu.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://rm.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dl.shtwfgs.cn

[M05] 设置退出码
来源：http://td.haigaiapp.cn

Py:   sys.exit(1)
来源：http://pc.shxzskj.cn

PHP:  exit(1);
来源：http://ce.jctech888.com.cn

JS:   process.exit(1)
来源：http://et.jctech888.com.cn

TS:   process.exit(1)
来源：http://ls.bjjhwx.cn

Java: System.exit(1)
来源：http://lv.gzmigu.cn

Go:   os.Exit(1)
来源：http://vi.shxzskj.cn

Ruby: exit 1
来源：http://zv.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ws.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://iy.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://fp.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yy.521024.cn

JS:   console.error("err")
来源：http://hl.521024.cn

TS:   console.error("err")
来源：http://ip.hahajie.cn

Java: System.err.println("err")
来源：http://fv.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zi.asd995.cn

Ruby: warn "err"
来源：http://fq.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://py.colortex.cn

[M07] 判断是否为主入口
来源：http://au.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://xx.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://im.nicolike.cn

JS:   require.main === module
来源：http://dk.asd995.cn

TS:   require.main === module
来源：http://lm.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://jp.haigaiapp.cn

Go:   func main()
来源：http://om.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kz.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://px.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://xj.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://qd.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://sr.hnjuh.cn

JS:   process.platform;  process.version
来源：http://ot.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://tw.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pv.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lb.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wb.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jq.hahajie.cn

================================================================================
来源：http://ia.asd995.cn

N. 数据结构与算法
来源：http://yx.yuntaijiaju.cn

================================================================================
来源：http://nn.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://ct.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yg.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yc.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rp.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gn.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mx.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://pu.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wr.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vt.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://kg.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://fc.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xm.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wf.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jg.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ct.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://wj.huanxung.cn

Ruby: arr.sort
来源：http://ap.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xz.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://mm.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qa.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://wn.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ko.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sy.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iv.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ac.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ix.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lk.521024.cn

[N04] 斐波那契数列
来源：http://tb.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vn.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uq.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rx.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fa.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jb.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ts.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hj.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oh.yuexingan06.cn


<!-- 参考信息 -->