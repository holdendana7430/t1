代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xb.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nv.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qd.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xv.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://em.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ba.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bq.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://se.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wc.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://up.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lc.huanxung.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ym.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ou.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vn.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sv.shxzskj.cn

================================================================================
来源：http://ee.colortex.cn

K. JSON 与序列化
来源：http://hs.shtwfgs.cn

================================================================================
来源：http://lv.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://yv.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eu.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lk.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://id.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://yh.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mu.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://bl.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jp.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kn.asd995.cn

[K02] JSON 字符串转对象
来源：http://wi.muxihuayi.cn

Py:   json.loads(s)
来源：http://ep.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ab.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ri.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://kt.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cl.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://qx.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://eo.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qm.nicolike.cn

[K03] JSON 美化输出（带缩进）
来源：http://jv.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nm.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://do.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bw.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uc.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wi.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gc.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ji.hahajie.cn

[K04] 读取 JSON 文件
来源：http://vu.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lj.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gr.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ai.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tt.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ia.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fy.hnjuh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ni.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uj.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://fr.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://fm.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://ir.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://rv.colortex.cn

TS:   structuredClone(obj)
来源：http://db.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ka.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dl.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kf.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xm.huanxung.cn

[K06] 解析 URL 查询串
来源：http://pr.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wq.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ic.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oy.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hr.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ac.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hl.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lh.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ja.yuntaijiaju.cn

[K07] 进制转换
来源：http://uz.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rj.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pe.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zz.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ey.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pl.shtwfgs.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ak.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://np.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iv.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://cm.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://nv.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xm.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://go.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://gg.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dp.hnjuh.cn

Go:   encoding/gob
来源：http://kk.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://bf.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ca.chemitech.net.cn

================================================================================
来源：http://yc.shtwfgs.cn

L. 网络请求
来源：http://yn.huixinmuqiang.cn

================================================================================
来源：http://bp.panjiajie.cn

[L01] 发送 GET 请求
来源：http://gg.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ob.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tm.shxzukj.cn

JS:   await fetch(url)
来源：http://ur.gzmigu.cn

TS:   await fetch(url)
来源：http://mm.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uh.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://nc.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kb.shtwfgs.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.521024.cn

[L02] 发送 POST JSON
来源：http://et.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nm.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ru.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://je.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vz.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yy.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jh.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ha.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xf.szsharing.cn

[L03] 设置自定义请求头
来源：http://zn.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ap.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nb.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vw.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pj.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sw.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wa.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xq.jianghongdianzi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ll.szsharing.cn

[L04] 设置超时
来源：http://ty.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://as.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ou.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://di.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vn.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zn.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rb.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mm.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://he.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://ei.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ru.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ak.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hm.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wz.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fq.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ao.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xw.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qa.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://iw.panjiajie.cn

Py:   resp.json()
来源：http://yp.9csxet.cn

PHP:  json_decode($body, true);
来源：http://zd.colortex.cn

JS:   await resp.json()
来源：http://ld.hahajie.cn

TS:   await resp.json()
来源：http://oh.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nd.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gz.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://tm.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tk.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://ji.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ed.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nf.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://fq.asd995.cn

TS:   resp.ok;  resp.status
来源：http://zj.wgjwhj.cn

Java: resp.statusCode()
来源：http://go.huanxung.cn

Go:   resp.StatusCode
来源：http://pf.colortex.cn

Ruby: resp.code.to_i
来源：http://jh.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://se.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://yt.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gz.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://rw.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rh.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mn.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kf.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ox.yuntaijiaju.cn

================================================================================
来源：http://kg.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://td.nicolike.cn

================================================================================
来源：http://hv.jctech888.com.cn

[M01] 读取命令行参数
来源：http://kd.newstarts.cn

Py:   sys.argv[1:]
来源：http://et.9csxet.cn

PHP:  $argv;  $argc;
来源：http://xq.huanxung.cn

JS:   process.argv.slice(2)
来源：http://ds.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://eu.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://mt.lnxyls.cn

Go:   os.Args[1:]
来源：http://zn.nszjky.cn

Ruby: ARGV
来源：http://om.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://to.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://kq.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://cs.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rl.9csxet.cn

JS:   process.env.HOME
来源：http://sw.bookmarksfly.cn

TS:   process.env.HOME
来源：http://pp.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://jg.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gy.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://ph.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gv.bjjhwx.cn

[M03] 执行外部命令
来源：http://fk.jctech888.com.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nq.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xh.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gq.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tj.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rv.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eo.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hd.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://gc.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://jb.shtwfgs.cn

Py:   os.getcwd()
来源：http://qo.huixiangedu.cn

PHP:  getcwd();
来源：http://pu.shxzukj.cn

JS:   process.cwd()
来源：http://vs.wgjwhj.cn

TS:   process.cwd()
来源：http://yk.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://jl.muxihuayi.cn

Go:   os.Getwd()
来源：http://xs.colortex.cn

Ruby: Dir.pwd
来源：http://er.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gw.gzmigu.cn

[M05] 设置退出码
来源：http://hw.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://vv.chemitech.net.cn

PHP:  exit(1);
来源：http://uh.521024.cn

JS:   process.exit(1)
来源：http://dx.shxzukj.cn

TS:   process.exit(1)
来源：http://dk.hnjuh.cn

Java: System.exit(1)
来源：http://rc.bjjhwx.cn

Go:   os.Exit(1)
来源：http://jd.nicolike.cn

Ruby: exit 1
来源：http://nm.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vz.haigaiapp.cn

[M06] 向标准错误输出
来源：http://fh.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://oy.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ns.521024.cn

JS:   console.error("err")
来源：http://wo.hahajie.cn

TS:   console.error("err")
来源：http://aq.521024.cn

Java: System.err.println("err")
来源：http://sm.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qv.hnjuh.cn

Ruby: warn "err"
来源：http://pj.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://jh.szsharing.cn

[M07] 判断是否为主入口
来源：http://je.yuntaijiaju.cn

Py:   if __name__ == "__main__":
来源：http://zn.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lh.huanxung.cn

JS:   require.main === module
来源：http://fw.huanxung.cn

TS:   require.main === module
来源：http://bj.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ux.bookmarksfly.cn

Go:   func main()
来源：http://fq.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bm.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://jl.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://fq.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://kc.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://gc.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://ae.shxzskj.cn

TS:   process.platform;  process.version
来源：http://lq.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gq.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zy.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ta.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kq.yuexingan06.cn

================================================================================
来源：http://kd.yuexingan06.cn

N. 数据结构与算法
来源：http://oo.huixinmuqiang.cn

================================================================================
来源：http://wc.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://gz.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uv.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ia.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jl.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pl.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oc.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://oa.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ki.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hb.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://ml.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://cm.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uf.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ah.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aw.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yv.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://gb.jctech888.com.cn

Ruby: arr.sort
来源：http://py.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://eb.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://wo.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ak.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://zg.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mf.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gf.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cd.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mx.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yc.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jd.yuexingan06.cn

[N04] 斐波那契数列
来源：http://sx.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://of.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wr.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cz.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ur.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rs.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ft.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xg.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://so.huixinmuqiang.cn

[N05] 最大公约数
来源：http://ho.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://mq.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uo.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qu.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qt.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yr.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ob.lnxyls.cn

Ruby: a.gcd(b)
来源：http://bc.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gk.shxzskj.cn

[N06] 判断回文字符串
来源：http://xg.muxihuayi.cn

Py:   s == s[::-1]
来源：http://ed.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://rc.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://up.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://wl.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tq.colortex.cn

Go:   // 双指针从两端比较
来源：http://wu.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://uk.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wq.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://kr.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qj.asd995.cn


<!-- 参考信息 -->