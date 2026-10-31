代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://qx.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wz.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dv.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rv.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bp.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fi.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ox.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jw.nicolike.cn

================================================================================
来源：http://lb.wgjwhj.cn

K. JSON 与序列化
来源：http://ok.huixinmuqiang.cn

================================================================================
来源：http://ts.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://ub.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bj.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gh.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://ex.521024.cn

TS:   JSON.stringify(obj)
来源：http://fh.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ix.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://jc.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wg.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yw.asd995.cn

[K02] JSON 字符串转对象
来源：http://hs.colortex.cn

Py:   json.loads(s)
来源：http://sl.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cs.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://oe.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://vi.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sb.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://ad.szsharing.cn

Ruby: JSON.parse(s)
来源：http://tb.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lv.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://ze.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wh.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fj.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wp.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ye.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wg.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wl.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ut.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xt.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://pc.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jk.hahajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ta.shxzukj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://io.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tc.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yq.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hd.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bv.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://xp.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://nd.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://je.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://hq.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://ca.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://be.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uy.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jz.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ew.szsharing.cn

[K06] 解析 URL 查询串
来源：http://ki.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ti.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qi.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kg.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://se.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yu.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pm.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yn.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ia.huixinmuqiang.cn

[K07] 进制转换
来源：http://kz.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://on.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ep.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mk.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fg.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ls.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xn.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mu.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wk.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://bw.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://by.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hc.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://om.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://vo.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dc.9csxet.cn

Go:   encoding/gob
来源：http://sz.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://us.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pd.yuexingan06.cn

================================================================================
来源：http://ru.bookmarksfly.cn

L. 网络请求
来源：http://eu.jctech888.com.cn

================================================================================
来源：http://zn.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://gb.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fd.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bl.521024.cn

JS:   await fetch(url)
来源：http://cj.hahajie.cn

TS:   await fetch(url)
来源：http://sm.shxzskj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fl.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://ck.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ya.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fp.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://hd.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://md.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hu.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oy.bookmarksfly.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mf.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ik.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://df.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ec.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yu.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://sw.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vg.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tk.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qr.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xb.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yx.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vq.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ln.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fz.lnxyls.cn

[L04] 设置超时
来源：http://hf.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://gf.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uu.gzmigu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fk.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uz.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ix.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ax.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hq.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://vn.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ty.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://za.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yf.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://od.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ap.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ku.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xj.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nm.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ad.chemitech.net.cn

Py:   resp.json()
来源：http://of.nicolike.cn

PHP:  json_decode($body, true);
来源：http://uq.hnjuh.cn

JS:   await resp.json()
来源：http://yi.szxytkj.cn

TS:   await resp.json()
来源：http://rb.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dx.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://me.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://eh.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tl.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://tb.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pn.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ul.521024.cn

JS:   resp.ok;  resp.status
来源：http://pl.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://zk.bjjhwx.cn

Java: resp.statusCode()
来源：http://jd.gzmigu.cn

Go:   resp.StatusCode
来源：http://of.asd995.cn

Ruby: resp.code.to_i
来源：http://ol.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://xy.nszjky.cn

[L08] 并发请求多个地址
来源：http://fu.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sa.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://yr.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://us.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://at.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dt.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cr.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wu.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yd.yuntaijiaju.cn

================================================================================
来源：http://jv.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://bw.chemitech.net.cn

================================================================================
来源：http://vo.szxytkj.cn

[M01] 读取命令行参数
来源：http://qm.nicolike.cn

Py:   sys.argv[1:]
来源：http://hi.shtwfgs.cn

PHP:  $argv;  $argc;
来源：http://pw.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://uu.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://lg.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://my.nicolike.cn

Go:   os.Args[1:]
来源：http://nw.colortex.cn

Ruby: ARGV
来源：http://tl.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://fj.gzmigu.cn

[M02] 读取环境变量
来源：http://lp.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://br.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jr.shxzskj.cn

JS:   process.env.HOME
来源：http://xc.wgjwhj.cn

TS:   process.env.HOME
来源：http://as.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://zk.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wt.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://qi.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pa.gzmigu.cn

[M03] 执行外部命令
来源：http://rx.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ee.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://az.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ch.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cr.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mt.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jf.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qi.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://tn.szsharing.cn

[M04] 获取当前工作目录
来源：http://oo.haigaiapp.cn

Py:   os.getcwd()
来源：http://ti.haigaiapp.cn

PHP:  getcwd();
来源：http://lw.huixiangedu.cn

JS:   process.cwd()
来源：http://sl.haigaiapp.cn

TS:   process.cwd()
来源：http://av.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://gc.hnjuh.cn

Go:   os.Getwd()
来源：http://vu.haigaiapp.cn

Ruby: Dir.pwd
来源：http://aq.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eu.szsharing.cn

[M05] 设置退出码
来源：http://vg.nszjky.cn

Py:   sys.exit(1)
来源：http://zz.chemitech.net.cn

PHP:  exit(1);
来源：http://gc.521024.cn

JS:   process.exit(1)
来源：http://li.wgjwhj.cn

TS:   process.exit(1)
来源：http://rv.newstarts.cn

Java: System.exit(1)
来源：http://vw.asd995.cn

Go:   os.Exit(1)
来源：http://po.bjjhwx.cn

Ruby: exit 1
来源：http://jc.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://te.muxihuayi.cn

[M06] 向标准错误输出
来源：http://rt.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://lz.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kz.shtwfgs.cn

JS:   console.error("err")
来源：http://dj.chemitech.net.cn

TS:   console.error("err")
来源：http://nt.521024.cn

Java: System.err.println("err")
来源：http://lu.lnxyls.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tu.hnjuh.cn

Ruby: warn "err"
来源：http://yr.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://mo.shxzukj.cn

[M07] 判断是否为主入口
来源：http://ty.asd995.cn

Py:   if __name__ == "__main__":
来源：http://ci.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iw.asd995.cn

JS:   require.main === module
来源：http://yc.jianghongdianzi.cn

TS:   require.main === module
来源：http://uk.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://lr.bjjhwx.cn

Go:   func main()
来源：http://yr.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vc.szsharing.cn

C#:   static void Main(string[] args)
来源：http://xn.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://ug.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ak.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://gj.colortex.cn

JS:   process.platform;  process.version
来源：http://cm.shxzukj.cn

TS:   process.platform;  process.version
来源：http://fk.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bq.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ws.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qc.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yw.newstarts.cn

================================================================================
来源：http://hq.huixinmuqiang.cn

N. 数据结构与算法
来源：http://cc.521024.cn

================================================================================
来源：http://cc.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://kj.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rm.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ni.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pr.jctech888.com.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://on.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vq.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://zx.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tu.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kp.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://ss.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://gf.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ci.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oo.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qx.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gb.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://nn.9csxet.cn

Ruby: arr.sort
来源：http://gx.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qh.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://wr.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kr.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://wp.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ne.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yt.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lg.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rv.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wk.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fl.haigaiapp.cn

[N04] 斐波那契数列
来源：http://om.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tq.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ly.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ef.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cl.shxzskj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hu.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qj.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://in.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ye.shtwfgs.cn

[N05] 最大公约数
来源：http://hr.szsharing.cn

Py:   math.gcd(a, b)
来源：http://ds.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xk.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lf.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://np.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jp.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://py.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://sr.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oj.huanxung.cn

[N06] 判断回文字符串
来源：http://hx.jctech888.com.cn

Py:   s == s[::-1]
来源：http://ki.asd995.cn

PHP:  $s === strrev($s);
来源：http://tq.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://gg.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://cu.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zu.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://mc.colortex.cn

Ruby: s == s.reverse
来源：http://jt.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bf.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://cn.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tf.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ju.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ia.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ci.hnjuh.cn

Java: // 手写 HashMap
来源：http://nb.newstarts.cn

Go:   // 手写 map[int]int
来源：http://hd.szxytkj.cn

Ruby: // 手写 Hash
来源：http://mp.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cv.asd995.cn

[N08] 生成全排列
来源：http://ey.nicolike.cn


<!-- 参考信息 -->