代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xu.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lu.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jh.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yi.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qo.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qf.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://el.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jn.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wo.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sg.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bk.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ue.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dm.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://er.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jh.hahajie.cn

================================================================================
来源：http://nh.panjiajie.cn

K. JSON 与序列化
来源：http://rs.shxzskj.cn

================================================================================
来源：http://ky.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://yk.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tn.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://se.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ss.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://na.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jn.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://jc.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qd.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://db.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://ds.haigaiapp.cn

Py:   json.loads(s)
来源：http://og.bjjhwx.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xh.szxytkj.cn

JS:   JSON.parse(s)
来源：http://ae.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ic.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hl.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://bb.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://qf.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zv.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://cb.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lh.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://or.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ek.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yb.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rb.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xr.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zq.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sx.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://dd.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kj.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fp.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kq.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ef.9csxet.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rw.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vw.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bn.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://km.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ar.lnxyls.cn

Py:   copy.deepcopy(obj)
来源：http://tu.shxzskj.cn

PHP:  unserialize(serialize($obj));
来源：http://ad.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://rf.shtwfgs.cn

TS:   structuredClone(obj)
来源：http://ik.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://op.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ww.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lh.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cx.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://iv.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rx.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ms.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jv.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tm.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xt.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lq.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wt.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://os.colortex.cn

[K07] 进制转换
来源：http://as.newstarts.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://km.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cj.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xh.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bq.bookmarksfly.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eh.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ry.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sl.nszjky.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wu.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://go.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://ws.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ao.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://ss.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://nd.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://to.szsharing.cn

Go:   encoding/gob
来源：http://qv.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://ot.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xz.muxihuayi.cn

================================================================================
来源：http://vj.huixinmuqiang.cn

L. 网络请求
来源：http://cg.panjiajie.cn

================================================================================
来源：http://nb.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://sa.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://we.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uc.szxytkj.cn

JS:   await fetch(url)
来源：http://rl.9csxet.cn

TS:   await fetch(url)
来源：http://mx.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ug.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://gn.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xs.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ym.shxzskj.cn

[L02] 发送 POST JSON
来源：http://hp.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://st.shxzskj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hb.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lr.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://so.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zg.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jr.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ow.shxzukj.cn

[L03] 设置自定义请求头
来源：http://vj.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nb.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ml.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kx.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eg.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://og.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xl.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kz.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fo.hnjuh.cn

[L04] 设置超时
来源：http://tm.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://nz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iu.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oj.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wr.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://up.bjjhwx.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nf.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ly.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nc.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://gu.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rn.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ih.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mx.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://er.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://as.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ct.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://en.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://yq.panjiajie.cn

Py:   resp.json()
来源：http://qe.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://ac.yuntaijiaju.cn

JS:   await resp.json()
来源：http://wc.wgjwhj.cn

TS:   await resp.json()
来源：http://ir.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zt.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://se.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://xf.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sw.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://aa.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nf.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jf.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://yh.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://no.huanxung.cn

Java: resp.statusCode()
来源：http://jr.jctech888.com.cn

Go:   resp.StatusCode
来源：http://yu.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://hx.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://jm.shxzskj.cn

[L08] 并发请求多个地址
来源：http://di.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jw.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://jz.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jt.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ra.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://er.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kh.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gt.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sx.panjiajie.cn

================================================================================
来源：http://bv.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://iy.jctech888.com.cn

================================================================================
来源：http://zr.panjiajie.cn

[M01] 读取命令行参数
来源：http://hj.szsharing.cn

Py:   sys.argv[1:]
来源：http://qx.hahajie.cn

PHP:  $argv;  $argc;
来源：http://dy.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://am.szsharing.cn

TS:   process.argv.slice(2)
来源：http://lu.chemitech.net.cn

Java: args 数组（main 方法参数）
来源：http://vu.chemitech.net.cn

Go:   os.Args[1:]
来源：http://vk.nicolike.cn

Ruby: ARGV
来源：http://ll.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://jo.newstarts.cn

[M02] 读取环境变量
来源：http://in.asd995.cn

Py:   os.environ.get("HOME")
来源：http://hw.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://py.bookmarksfly.cn

JS:   process.env.HOME
来源：http://iz.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://eg.9csxet.cn

Java: System.getenv("HOME")
来源：http://kr.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pn.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://by.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eg.newstarts.cn

[M03] 执行外部命令
来源：http://ax.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bw.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zp.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vf.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cg.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tt.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wg.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pv.muxihuayi.cn

C#:   Process.Start("ls", "-l");
来源：http://da.gzmigu.cn

[M04] 获取当前工作目录
来源：http://wi.hahajie.cn

Py:   os.getcwd()
来源：http://gt.hnjuh.cn

PHP:  getcwd();
来源：http://rz.shtwfgs.cn

JS:   process.cwd()
来源：http://qq.hahajie.cn

TS:   process.cwd()
来源：http://nq.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://uf.hnjuh.cn

Go:   os.Getwd()
来源：http://ly.gzmigu.cn

Ruby: Dir.pwd
来源：http://iy.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wo.521024.cn

[M05] 设置退出码
来源：http://ep.nicolike.cn

Py:   sys.exit(1)
来源：http://kw.nszjky.cn

PHP:  exit(1);
来源：http://kd.shtwfgs.cn

JS:   process.exit(1)
来源：http://sj.panjiajie.cn

TS:   process.exit(1)
来源：http://tz.szsharing.cn

Java: System.exit(1)
来源：http://eh.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://ak.huixiangedu.cn

Ruby: exit 1
来源：http://cy.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ls.gzmigu.cn

[M06] 向标准错误输出
来源：http://qi.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://sw.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nm.hahajie.cn

JS:   console.error("err")
来源：http://oz.bjjhwx.cn

TS:   console.error("err")
来源：http://fu.shxzskj.cn

Java: System.err.println("err")
来源：http://bg.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mw.newstarts.cn

Ruby: warn "err"
来源：http://hq.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://da.shxzukj.cn

[M07] 判断是否为主入口
来源：http://ei.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://eg.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ie.shtwfgs.cn

JS:   require.main === module
来源：http://tc.lnxyls.cn

TS:   require.main === module
来源：http://tg.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ev.yuntaijiaju.cn

Go:   func main()
来源：http://um.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ek.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://rc.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://gs.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://lm.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://sm.hahajie.cn

JS:   process.platform;  process.version
来源：http://tg.szsharing.cn

TS:   process.platform;  process.version
来源：http://jn.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bw.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ib.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fb.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ju.hahajie.cn

================================================================================
来源：http://or.hnjuh.cn

N. 数据结构与算法
来源：http://fs.huanxung.cn

================================================================================
来源：http://kb.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://rd.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rt.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ti.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ka.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ej.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://da.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://ty.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zx.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ns.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://og.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vj.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ua.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tu.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ow.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gn.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://mw.hahajie.cn

Ruby: arr.sort
来源：http://la.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iq.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://wr.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xv.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://ug.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tn.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nt.newstarts.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tr.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rp.hnjuh.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fl.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://og.huanxung.cn

[N04] 斐波那契数列
来源：http://hq.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nm.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qj.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jd.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ki.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wp.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xi.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uy.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ek.9csxet.cn

[N05] 最大公约数
来源：http://ro.newstarts.cn

Py:   math.gcd(a, b)
来源：http://ry.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jw.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jp.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wq.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cw.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dw.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ac.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rw.panjiajie.cn

[N06] 判断回文字符串
来源：http://ts.panjiajie.cn

Py:   s == s[::-1]
来源：http://ab.jianghongdianzi.cn

PHP:  $s === strrev($s);
来源：http://ue.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://ol.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://vd.shtwfgs.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cc.newstarts.cn

Go:   // 双指针从两端比较
来源：http://kw.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://iz.szxytkj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lc.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://tz.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ce.shxzukj.cn


<!-- 参考信息 -->