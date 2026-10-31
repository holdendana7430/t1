代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uk.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hw.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ld.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zy.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://od.chemitech.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sa.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zv.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://xi.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gn.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yf.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fq.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://df.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rb.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://la.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xg.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kk.nszjky.cn

================================================================================
来源：http://ld.9csxet.cn

K. JSON 与序列化
来源：http://ra.bjjhwx.cn

================================================================================
来源：http://qy.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://pq.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mq.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oj.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://ml.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://lt.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gd.nszjky.cn

Go:   json.Marshal(obj)
来源：http://qg.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kh.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wq.colortex.cn

[K02] JSON 字符串转对象
来源：http://sm.nicolike.cn

Py:   json.loads(s)
来源：http://vq.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xg.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://eo.nicolike.cn

TS:   JSON.parse(s)
来源：http://tf.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wh.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://mh.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://zo.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qx.521024.cn

[K03] JSON 美化输出（带缩进）
来源：http://ft.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zo.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wk.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zx.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://to.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ha.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pz.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://go.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ek.9csxet.cn

[K04] 读取 JSON 文件
来源：http://tf.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mr.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rm.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wu.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qf.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yg.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fz.bookmarksfly.cn

[K05] 深拷贝对象
来源：http://zy.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://cs.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://eq.shxzskj.cn

JS:   structuredClone(obj)
来源：http://by.chemitech.net.cn

TS:   structuredClone(obj)
来源：http://bz.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fo.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sv.shxzskj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cp.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vl.colortex.cn

[K06] 解析 URL 查询串
来源：http://jz.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ng.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yv.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sh.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ix.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gv.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yl.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bj.lnxyls.cn

[K07] 进制转换
来源：http://mb.shtwfgs.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wt.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xb.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ix.bookmarksfly.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qb.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gx.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nk.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ew.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qv.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://jn.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://uj.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ao.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://rx.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://ds.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pq.yuexingan06.cn

Go:   encoding/gob
来源：http://ma.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://gy.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://js.wgjwhj.cn

================================================================================
来源：http://bj.bookmarksfly.cn

L. 网络请求
来源：http://ka.asd995.cn

================================================================================
来源：http://jo.nicolike.cn

[L01] 发送 GET 请求
来源：http://wq.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jp.yuntaijiaju.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ij.colortex.cn

JS:   await fetch(url)
来源：http://dc.szxytkj.cn

TS:   await fetch(url)
来源：http://fc.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yb.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://qd.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cu.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sz.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://xv.shtwfgs.cn

Py:   requests.post(url, json={"a": 1})
来源：http://db.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yl.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cm.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kn.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hq.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oy.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fj.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vc.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://ca.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zv.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bo.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nn.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ir.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wh.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gz.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lx.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ki.haigaiapp.cn

[L04] 设置超时
来源：http://rn.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://mo.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ug.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vu.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eh.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fr.9csxet.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ns.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zo.nszjky.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oy.asd995.cn

[L05] 上传文件（multipart）
来源：http://gc.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kl.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cj.gzmigu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rn.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nj.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ck.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://so.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://np.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gt.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://qc.yuntaijiaju.cn

Py:   resp.json()
来源：http://fv.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://mk.asd995.cn

JS:   await resp.json()
来源：http://ij.huixinmuqiang.cn

TS:   await resp.json()
来源：http://ju.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lg.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rj.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://jn.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iy.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://hx.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://db.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ah.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://or.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://uh.9csxet.cn

Java: resp.statusCode()
来源：http://fz.nszjky.cn

Go:   resp.StatusCode
来源：http://oo.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://bb.szxytkj.cn

C#:   (int)resp.StatusCode
来源：http://ls.nszjky.cn

[L08] 并发请求多个地址
来源：http://jv.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rc.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://wt.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://we.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bq.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iw.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kd.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://um.jctech888.com.cn

================================================================================
来源：http://ez.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://be.shxzskj.cn

================================================================================
来源：http://gl.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://xq.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://pi.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://up.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://ep.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://gg.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://hf.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://yn.521024.cn

Ruby: ARGV
来源：http://dh.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://lv.lnxyls.cn

[M02] 读取环境变量
来源：http://nc.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://mt.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wf.bjjhwx.cn

JS:   process.env.HOME
来源：http://lk.muxihuayi.cn

TS:   process.env.HOME
来源：http://rv.lnxyls.cn

Java: System.getenv("HOME")
来源：http://gl.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tk.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://yy.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pn.shxzskj.cn

[M03] 执行外部命令
来源：http://jl.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yt.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ip.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tu.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rh.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vx.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xo.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://am.shxzukj.cn

C#:   Process.Start("ls", "-l");
来源：http://uo.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://to.jctech888.com.cn

Py:   os.getcwd()
来源：http://hj.jctech888.com.cn

PHP:  getcwd();
来源：http://zz.shxzukj.cn

JS:   process.cwd()
来源：http://dg.shtwfgs.cn

TS:   process.cwd()
来源：http://bv.shxzskj.cn

Java: Path.of("").toAbsolutePath()
来源：http://cr.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ej.nszjky.cn

Ruby: Dir.pwd
来源：http://ri.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zn.wgjwhj.cn

[M05] 设置退出码
来源：http://pp.colortex.cn

Py:   sys.exit(1)
来源：http://fx.jianghongdianzi.cn

PHP:  exit(1);
来源：http://jl.lnxyls.cn

JS:   process.exit(1)
来源：http://aj.colortex.cn

TS:   process.exit(1)
来源：http://bu.521024.cn

Java: System.exit(1)
来源：http://dl.jctech888.com.cn

Go:   os.Exit(1)
来源：http://ut.colortex.cn

Ruby: exit 1
来源：http://co.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wi.hahajie.cn

[M06] 向标准错误输出
来源：http://qr.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://sy.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qq.colortex.cn

JS:   console.error("err")
来源：http://xg.muxihuayi.cn

TS:   console.error("err")
来源：http://dm.huixiangedu.cn

Java: System.err.println("err")
来源：http://kr.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cu.hahajie.cn

Ruby: warn "err"
来源：http://ys.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://cl.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://xo.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ff.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://do.huixinmuqiang.cn

JS:   require.main === module
来源：http://ba.newstarts.cn

TS:   require.main === module
来源：http://jm.9csxet.cn

Java: public static void main(String[] args)
来源：http://lu.nszjky.cn

Go:   func main()
来源：http://cw.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ys.shtwfgs.cn

C#:   static void Main(string[] args)
来源：http://gm.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://cu.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://pa.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ei.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://gf.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://dd.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lv.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cl.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nz.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vc.lnxyls.cn

================================================================================
来源：http://zc.jianghongdianzi.cn

N. 数据结构与算法
来源：http://dz.bjjhwx.cn

================================================================================
来源：http://hk.asd995.cn

[N01] 二分查找（有序数组）
来源：http://at.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mu.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cb.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cd.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xd.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://uk.hnjuh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fb.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qo.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://at.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://qx.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tj.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ha.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ba.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tl.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://cv.bjjhwx.cn

Ruby: arr.sort
来源：http://wu.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jo.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ko.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ni.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://kw.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vs.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xf.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nr.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mq.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lb.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sx.hnjuh.cn

[N04] 斐波那契数列
来源：http://dm.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gq.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tj.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uz.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hj.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ds.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ke.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zk.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bg.hahajie.cn

[N05] 最大公约数
来源：http://bq.huanxung.cn

Py:   math.gcd(a, b)
来源：http://ab.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jm.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://up.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vs.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://up.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ad.asd995.cn

Ruby: a.gcd(b)
来源：http://tk.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pl.huixiangedu.cn

[N06] 判断回文字符串
来源：http://za.chemitech.net.cn

Py:   s == s[::-1]
来源：http://pj.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://jo.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://fx.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://tw.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://am.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://en.chemitech.net.cn

Ruby: s == s.reverse
来源：http://xd.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nq.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://oy.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wb.521024.cn


<!-- 参考信息 -->