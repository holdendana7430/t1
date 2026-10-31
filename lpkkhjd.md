代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vw.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mz.newstarts.cn

[J09] 时区处理
来源：http://yn.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ws.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yu.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zw.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ma.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oj.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jn.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ga.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ho.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://lm.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://br.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ar.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pc.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://on.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oi.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ug.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://du.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cr.521024.cn

================================================================================
来源：http://je.9csxet.cn

K. JSON 与序列化
来源：http://fu.hnjuh.cn

================================================================================
来源：http://kp.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://qv.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://as.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pf.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://ey.521024.cn

TS:   JSON.stringify(obj)
来源：http://xm.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ph.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://uu.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qi.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pg.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://im.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://km.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gg.nszjky.cn

JS:   JSON.parse(s)
来源：http://ub.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://xt.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zc.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://oq.521024.cn

Ruby: JSON.parse(s)
来源：http://ny.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zc.chemitech.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://ul.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uw.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://at.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wn.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jz.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eg.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ao.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sf.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bm.521024.cn

[K04] 读取 JSON 文件
来源：http://dy.szsharing.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hr.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wf.muxihuayi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wv.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ou.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uc.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ll.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://un.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://el.huixiangedu.cn

[K05] 深拷贝对象
来源：http://bb.jctech888.com.cn

Py:   copy.deepcopy(obj)
来源：http://hs.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ag.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://lx.bookmarksfly.cn

TS:   structuredClone(obj)
来源：http://ob.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xx.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bn.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lf.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://it.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://rl.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cl.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nw.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ue.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ll.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://to.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hq.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dl.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vj.jianghongdianzi.cn

[K07] 进制转换
来源：http://rj.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tp.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://or.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sh.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jm.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gq.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cf.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fl.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sm.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://gl.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cd.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://ta.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://op.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zs.yuexingan06.cn

Go:   encoding/gob
来源：http://ud.bookmarksfly.cn

Ruby: Marshal.dump(obj)
来源：http://kz.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://od.yuexingan06.cn

================================================================================
来源：http://uk.muxihuayi.cn

L. 网络请求
来源：http://si.nicolike.cn

================================================================================
来源：http://et.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://vq.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ry.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ke.asd995.cn

JS:   await fetch(url)
来源：http://gv.hnjuh.cn

TS:   await fetch(url)
来源：http://lc.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kp.colortex.cn

Go:   resp, err := http.Get(url)
来源：http://jv.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qq.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nf.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://cx.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lc.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fv.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fo.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nf.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kg.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wl.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eq.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mf.huixinmuqiang.cn

[L03] 设置自定义请求头
来源：http://vm.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oi.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sf.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fx.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bm.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fc.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qo.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ke.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ir.huixiangedu.cn

[L04] 设置超时
来源：http://va.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://ji.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rf.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wr.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uw.nicolike.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jr.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://er.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tg.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bb.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://hk.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bl.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tu.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wx.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oe.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xu.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qm.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cn.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qg.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://cs.shtwfgs.cn

Py:   resp.json()
来源：http://yh.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://hn.shxzukj.cn

JS:   await resp.json()
来源：http://sh.bookmarksfly.cn

TS:   await resp.json()
来源：http://no.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ff.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ya.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://jo.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vt.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://po.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xf.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tb.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://gj.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://tu.lnxyls.cn

Java: resp.statusCode()
来源：http://zi.panjiajie.cn

Go:   resp.StatusCode
来源：http://ap.gzmigu.cn

Ruby: resp.code.to_i
来源：http://py.colortex.cn

C#:   (int)resp.StatusCode
来源：http://at.szxytkj.cn

[L08] 并发请求多个地址
来源：http://zl.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://es.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://fd.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jp.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ax.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ju.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ag.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tq.newstarts.cn

================================================================================
来源：http://ct.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://xg.huixiangedu.cn

================================================================================
来源：http://sv.shxzskj.cn

[M01] 读取命令行参数
来源：http://lz.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://ur.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://xe.asd995.cn

JS:   process.argv.slice(2)
来源：http://wn.521024.cn

TS:   process.argv.slice(2)
来源：http://hh.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://ef.shxzskj.cn

Go:   os.Args[1:]
来源：http://th.9csxet.cn

Ruby: ARGV
来源：http://fv.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://eq.szxytkj.cn

[M02] 读取环境变量
来源：http://nk.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://yu.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://em.hahajie.cn

JS:   process.env.HOME
来源：http://ah.chemitech.net.cn

TS:   process.env.HOME
来源：http://cs.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://ap.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ws.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://pm.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ua.huixiangedu.cn

[M03] 执行外部命令
来源：http://ix.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kz.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nt.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://id.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fm.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gq.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ix.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://it.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://jn.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://lm.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://li.jianghongdianzi.cn

PHP:  getcwd();
来源：http://sp.hnjuh.cn

JS:   process.cwd()
来源：http://lm.muxihuayi.cn

TS:   process.cwd()
来源：http://uv.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ss.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://kv.lnxyls.cn

Ruby: Dir.pwd
来源：http://pm.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ly.shxzukj.cn

[M05] 设置退出码
来源：http://bg.bjjhwx.cn

Py:   sys.exit(1)
来源：http://td.nszjky.cn

PHP:  exit(1);
来源：http://st.szxytkj.cn

JS:   process.exit(1)
来源：http://qu.nszjky.cn

TS:   process.exit(1)
来源：http://my.nszjky.cn

Java: System.exit(1)
来源：http://cg.hnjuh.cn

Go:   os.Exit(1)
来源：http://lz.bjjhwx.cn

Ruby: exit 1
来源：http://bc.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hb.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://pf.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://ze.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hl.jianghongdianzi.cn

JS:   console.error("err")
来源：http://lg.shxzskj.cn

TS:   console.error("err")
来源：http://zz.hnjuh.cn

Java: System.err.println("err")
来源：http://oz.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://om.huixiangedu.cn

Ruby: warn "err"
来源：http://ka.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://wm.9csxet.cn

[M07] 判断是否为主入口
来源：http://vm.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://uv.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gs.hahajie.cn

JS:   require.main === module
来源：http://ke.shxzukj.cn

TS:   require.main === module
来源：http://lx.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ga.shxzukj.cn

Go:   func main()
来源：http://lt.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ph.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://te.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://tn.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://de.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ig.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://of.huanxung.cn

TS:   process.platform;  process.version
来源：http://rl.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zs.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bj.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ms.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pz.9csxet.cn

================================================================================
来源：http://bk.9csxet.cn

N. 数据结构与算法
来源：http://tt.lnxyls.cn

================================================================================
来源：http://ir.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://sg.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rr.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://os.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qs.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aq.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pa.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://qh.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bv.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tc.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://gc.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://qe.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vh.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wl.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mq.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rt.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://to.yuntaijiaju.cn

Ruby: arr.sort
来源：http://fp.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://er.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://mw.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wu.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://ou.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ec.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qb.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://op.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ci.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ph.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://we.panjiajie.cn

[N04] 斐波那契数列
来源：http://se.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ui.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ub.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jk.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ux.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lt.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hg.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://do.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bx.szxytkj.cn

[N05] 最大公约数
来源：http://ox.nicolike.cn

Py:   math.gcd(a, b)
来源：http://nq.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zw.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://an.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tc.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://xa.haigaiapp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ib.szsharing.cn

[N06] 判断回文字符串
来源：http://xh.lnxyls.cn

Py:   s == s[::-1]
来源：http://bs.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ii.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://wm.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://yz.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fx.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://sb.9csxet.cn


<!-- 参考信息 -->