代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bj.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ah.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xb.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fn.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ds.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nq.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qa.521024.cn

[J10] 取今天 / 本月第一天
来源：http://nj.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qp.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dy.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sm.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xs.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vv.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gj.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wl.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bn.shxzskj.cn

================================================================================
来源：http://ox.chemitech.net.cn

K. JSON 与序列化
来源：http://np.yuexingan06.cn

================================================================================
来源：http://ys.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://ec.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pf.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xb.colortex.cn

JS:   JSON.stringify(obj)
来源：http://cy.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://lr.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://la.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://lc.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gy.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xh.nszjky.cn

[K02] JSON 字符串转对象
来源：http://cz.nicolike.cn

Py:   json.loads(s)
来源：http://tt.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iy.colortex.cn

JS:   JSON.parse(s)
来源：http://yg.newstarts.cn

TS:   JSON.parse(s)
来源：http://ex.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ir.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://up.nicolike.cn

Ruby: JSON.parse(s)
来源：http://wo.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vn.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://cm.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xc.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mi.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qd.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xy.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dm.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kz.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kr.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ap.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://je.nszjky.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vg.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ry.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yy.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rr.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mh.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ci.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hi.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dt.nszjky.cn

[K05] 深拷贝对象
来源：http://xt.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://tf.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://qg.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://vy.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://wf.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xj.yuntaijiaju.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rw.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qx.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rr.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://cc.yuexingan06.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.haigaiapp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cq.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zg.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kh.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zu.wgjwhj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bk.9csxet.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iz.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vq.yuntaijiaju.cn

[K07] 进制转换
来源：http://bt.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xr.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ch.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nb.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qo.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xi.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kq.newstarts.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://to.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yp.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://cd.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://sh.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kq.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://sf.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://nd.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fp.yuntaijiaju.cn

Go:   encoding/gob
来源：http://no.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://gm.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bh.wgjwhj.cn

================================================================================
来源：http://rg.szsharing.cn

L. 网络请求
来源：http://er.huixinmuqiang.cn

================================================================================
来源：http://zl.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://sk.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ti.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xi.hahajie.cn

JS:   await fetch(url)
来源：http://jm.haigaiapp.cn

TS:   await fetch(url)
来源：http://sn.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yu.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://uh.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kx.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ou.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ju.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hm.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rf.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yi.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mt.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lw.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zo.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nj.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shxzskj.cn

[L03] 设置自定义请求头
来源：http://oi.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gv.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qj.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qx.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tb.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xz.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lt.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kb.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ht.muxihuayi.cn

[L04] 设置超时
来源：http://vj.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://ne.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dt.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://os.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yr.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uk.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://so.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qq.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://du.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://ww.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wb.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://or.hahajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bn.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xi.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://si.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wb.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wi.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wj.521024.cn

[L06] 解析响应为 JSON
来源：http://cf.shxzskj.cn

Py:   resp.json()
来源：http://dd.9csxet.cn

PHP:  json_decode($body, true);
来源：http://ya.chemitech.net.cn

JS:   await resp.json()
来源：http://ft.wgjwhj.cn

TS:   await resp.json()
来源：http://zy.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cp.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yy.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://wj.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yz.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://vw.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sc.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yo.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://jw.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ar.szsharing.cn

Java: resp.statusCode()
来源：http://ka.9csxet.cn

Go:   resp.StatusCode
来源：http://dp.nszjky.cn

Ruby: resp.code.to_i
来源：http://sb.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://wx.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://za.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dp.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://ql.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ty.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fp.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tc.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gz.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dy.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wb.hnjuh.cn

================================================================================
来源：http://ih.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://hs.521024.cn

================================================================================
来源：http://pr.muxihuayi.cn

[M01] 读取命令行参数
来源：http://us.nszjky.cn

Py:   sys.argv[1:]
来源：http://xc.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://zw.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://oz.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://nm.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://wo.jctech888.com.cn

Go:   os.Args[1:]
来源：http://tr.szsharing.cn

Ruby: ARGV
来源：http://ze.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://yv.521024.cn

[M02] 读取环境变量
来源：http://aj.asd995.cn

Py:   os.environ.get("HOME")
来源：http://kc.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cg.521024.cn

JS:   process.env.HOME
来源：http://lw.huixiangedu.cn

TS:   process.env.HOME
来源：http://af.hahajie.cn

Java: System.getenv("HOME")
来源：http://dg.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bu.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://gj.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sv.shxzskj.cn

[M03] 执行外部命令
来源：http://ff.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mv.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wj.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nt.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rp.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rw.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mc.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xo.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://pt.colortex.cn

[M04] 获取当前工作目录
来源：http://rf.haigaiapp.cn

Py:   os.getcwd()
来源：http://bc.huixiangedu.cn

PHP:  getcwd();
来源：http://vd.wgjwhj.cn

JS:   process.cwd()
来源：http://qp.haigaiapp.cn

TS:   process.cwd()
来源：http://xm.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://jk.nszjky.cn

Go:   os.Getwd()
来源：http://rp.muxihuayi.cn

Ruby: Dir.pwd
来源：http://ef.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ud.lnxyls.cn

[M05] 设置退出码
来源：http://ko.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://mo.jianghongdianzi.cn

PHP:  exit(1);
来源：http://gx.gzmigu.cn

JS:   process.exit(1)
来源：http://lf.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://ho.muxihuayi.cn

Java: System.exit(1)
来源：http://qx.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://eb.huixiangedu.cn

Ruby: exit 1
来源：http://rr.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ao.hnjuh.cn

[M06] 向标准错误输出
来源：http://xd.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://mo.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cl.shxzukj.cn

JS:   console.error("err")
来源：http://qm.521024.cn

TS:   console.error("err")
来源：http://pi.lnxyls.cn

Java: System.err.println("err")
来源：http://es.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://po.asd995.cn

Ruby: warn "err"
来源：http://xp.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://xz.shxzskj.cn

[M07] 判断是否为主入口
来源：http://wn.521024.cn

Py:   if __name__ == "__main__":
来源：http://cj.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bi.bookmarksfly.cn

JS:   require.main === module
来源：http://jv.huixiangedu.cn

TS:   require.main === module
来源：http://wi.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://wg.9csxet.cn

Go:   func main()
来源：http://je.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aw.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://tm.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ub.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://vp.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://ps.newstarts.cn

JS:   process.platform;  process.version
来源：http://av.szxytkj.cn

TS:   process.platform;  process.version
来源：http://sb.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dg.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lu.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fu.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ap.shxzskj.cn

================================================================================
来源：http://vi.gzmigu.cn

N. 数据结构与算法
来源：http://bc.bookmarksfly.cn

================================================================================
来源：http://ba.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://kk.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zd.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lb.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lu.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ch.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aa.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://ii.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://at.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lb.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://le.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bt.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://as.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dj.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dj.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ql.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://gm.szxytkj.cn

Ruby: arr.sort
来源：http://ya.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kk.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://ls.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lj.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ps.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zt.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://go.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yu.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oj.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ln.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bt.nicolike.cn

[N04] 斐波那契数列
来源：http://kw.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ev.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ar.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dm.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xe.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oa.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vl.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sz.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vi.panjiajie.cn

[N05] 最大公约数
来源：http://sm.colortex.cn

Py:   math.gcd(a, b)
来源：http://hk.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nd.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rk.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hs.haigaiapp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fe.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fl.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://mm.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ef.shxzukj.cn

[N06] 判断回文字符串
来源：http://jr.gzmigu.cn

Py:   s == s[::-1]
来源：http://kj.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://av.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://ty.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://zz.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pf.asd995.cn

Go:   // 双指针从两端比较
来源：http://kq.nicolike.cn

Ruby: s == s.reverse
来源：http://pw.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cl.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://uz.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gl.hnjuh.cn


<!-- 参考信息 -->