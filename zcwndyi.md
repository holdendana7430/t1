代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lt.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yc.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vi.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://bx.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ag.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ap.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://il.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vf.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://al.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://px.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vc.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hg.jianghongdianzi.cn

================================================================================
来源：http://ru.yuexingan06.cn

K. JSON 与序列化
来源：http://jg.nicolike.cn

================================================================================
来源：http://mx.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://wu.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gk.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bv.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ta.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://sm.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zq.521024.cn

Go:   json.Marshal(obj)
来源：http://ly.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nx.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mu.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://bm.newstarts.cn

Py:   json.loads(s)
来源：http://mi.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zl.lnxyls.cn

JS:   JSON.parse(s)
来源：http://pc.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://ap.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://et.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://iv.colortex.cn

Ruby: JSON.parse(s)
来源：http://zo.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zp.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ey.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fs.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kw.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ie.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mr.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rt.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://on.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zp.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pg.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://cr.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://po.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qu.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dg.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qz.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://se.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ad.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wj.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sq.gzmigu.cn

[K05] 深拷贝对象
来源：http://uy.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://ob.hnjuh.cn

PHP:  unserialize(serialize($obj));
来源：http://fc.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://uj.newstarts.cn

TS:   structuredClone(obj)
来源：http://sb.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qm.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jy.huanxung.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pi.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ft.asd995.cn

[K06] 解析 URL 查询串
来源：http://tu.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jb.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gw.jctech888.com.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zr.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vd.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cf.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qb.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gv.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xf.chemitech.net.cn

[K07] 进制转换
来源：http://ed.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ap.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kj.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dd.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vj.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cc.newstarts.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nn.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gr.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gs.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://ds.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://vi.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ma.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://km.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://rn.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bw.wgjwhj.cn

Go:   encoding/gob
来源：http://az.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://tq.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gs.hahajie.cn

================================================================================
来源：http://uw.shxzukj.cn

L. 网络请求
来源：http://yy.asd995.cn

================================================================================
来源：http://fr.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://pp.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yr.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ez.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://ci.shxzukj.cn

TS:   await fetch(url)
来源：http://fu.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ty.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://yk.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ti.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tm.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://vn.muxihuayi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://py.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zg.colortex.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yp.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bf.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sm.nicolike.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tw.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fk.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mv.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://hg.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vn.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bs.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bm.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ez.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lb.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pi.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bv.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gf.newstarts.cn

[L04] 设置超时
来源：http://tj.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://ap.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://do.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wl.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qg.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mh.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xl.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sp.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sq.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://wy.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://is.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fa.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ug.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ga.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gq.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rw.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kf.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qv.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://sg.521024.cn

Py:   resp.json()
来源：http://ee.nszjky.cn

PHP:  json_decode($body, true);
来源：http://rj.shtwfgs.cn

JS:   await resp.json()
来源：http://iy.jctech888.com.cn

TS:   await resp.json()
来源：http://tj.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bz.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wd.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://wr.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bs.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://kc.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://me.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bo.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://kd.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://zh.lnxyls.cn

Java: resp.statusCode()
来源：http://ph.521024.cn

Go:   resp.StatusCode
来源：http://cs.shxzukj.cn

Ruby: resp.code.to_i
来源：http://ag.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://er.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://gl.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ru.muxihuayi.cn

PHP:  curl_multi_init() 系列
来源：http://dx.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aq.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dg.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jr.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uv.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qo.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ri.lnxyls.cn

================================================================================
来源：http://dm.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://gz.muxihuayi.cn

================================================================================
来源：http://qs.shxzskj.cn

[M01] 读取命令行参数
来源：http://yy.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://dp.jianghongdianzi.cn

PHP:  $argv;  $argc;
来源：http://xj.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ey.asd995.cn

TS:   process.argv.slice(2)
来源：http://re.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://dk.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://fw.wgjwhj.cn

Ruby: ARGV
来源：http://jy.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://jx.hahajie.cn

[M02] 读取环境变量
来源：http://kx.asd995.cn

Py:   os.environ.get("HOME")
来源：http://cq.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yp.shtwfgs.cn

JS:   process.env.HOME
来源：http://ua.bjjhwx.cn

TS:   process.env.HOME
来源：http://li.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://jq.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yy.colortex.cn

Ruby: ENV["HOME"]
来源：http://gc.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fz.newstarts.cn

[M03] 执行外部命令
来源：http://gs.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xn.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cx.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hy.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tq.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ez.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qz.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qi.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://bc.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://zp.jctech888.com.cn

Py:   os.getcwd()
来源：http://qo.panjiajie.cn

PHP:  getcwd();
来源：http://fb.lnxyls.cn

JS:   process.cwd()
来源：http://cn.lnxyls.cn

TS:   process.cwd()
来源：http://wb.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://pn.shtwfgs.cn

Go:   os.Getwd()
来源：http://mm.jctech888.com.cn

Ruby: Dir.pwd
来源：http://sv.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bp.shtwfgs.cn

[M05] 设置退出码
来源：http://yb.shxzukj.cn

Py:   sys.exit(1)
来源：http://za.shxzukj.cn

PHP:  exit(1);
来源：http://gm.shxzskj.cn

JS:   process.exit(1)
来源：http://ov.huixiangedu.cn

TS:   process.exit(1)
来源：http://wb.lnxyls.cn

Java: System.exit(1)
来源：http://lx.huixinmuqiang.cn

Go:   os.Exit(1)
来源：http://eh.hnjuh.cn

Ruby: exit 1
来源：http://gd.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xa.bjjhwx.cn

[M06] 向标准错误输出
来源：http://xl.haigaiapp.cn

Py:   print("err", file=sys.stderr)
来源：http://bn.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qh.nicolike.cn

JS:   console.error("err")
来源：http://ro.lnxyls.cn

TS:   console.error("err")
来源：http://md.nicolike.cn

Java: System.err.println("err")
来源：http://eb.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zb.newstarts.cn

Ruby: warn "err"
来源：http://fo.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://gj.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://ct.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://fe.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gd.szxytkj.cn

JS:   require.main === module
来源：http://bx.asd995.cn

TS:   require.main === module
来源：http://mn.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://oc.jctech888.com.cn

Go:   func main()
来源：http://vl.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mn.9csxet.cn

C#:   static void Main(string[] args)
来源：http://zd.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://mu.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://ub.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://aw.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://td.nicolike.cn

TS:   process.platform;  process.version
来源：http://ug.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lc.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pj.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ng.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ni.asd995.cn

================================================================================
来源：http://ct.yuntaijiaju.cn

N. 数据结构与算法
来源：http://zw.newstarts.cn

================================================================================
来源：http://lf.newstarts.cn

[N01] 二分查找（有序数组）
来源：http://jd.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wp.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ce.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zc.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hf.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xy.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://qp.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gx.jianghongdianzi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fk.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ms.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qu.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uo.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wm.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://su.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hi.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://id.muxihuayi.cn

Ruby: arr.sort
来源：http://gx.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yi.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://ug.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mf.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://ey.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pg.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://io.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ur.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rm.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iy.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hy.hnjuh.cn

[N04] 斐波那契数列
来源：http://zi.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kd.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ci.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fa.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wg.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://an.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tm.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rx.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://da.panjiajie.cn

[N05] 最大公约数
来源：http://ab.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://vn.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jc.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zp.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vx.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ny.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lt.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://yg.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rg.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://ii.szxytkj.cn

Py:   s == s[::-1]
来源：http://dz.hahajie.cn

PHP:  $s === strrev($s);
来源：http://vq.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://my.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://hw.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ul.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://wc.shtwfgs.cn

Ruby: s == s.reverse
来源：http://dt.newstarts.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zb.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://vf.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yj.521024.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://le.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uv.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ls.asd995.cn

Java: // 手写 HashMap
来源：http://xc.wgjwhj.cn


<!-- 参考信息 -->