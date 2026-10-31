代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jb.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yb.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lk.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://rn.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qu.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pw.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://or.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fi.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://me.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pm.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sy.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yc.haigaiapp.cn

================================================================================
来源：http://hc.haigaiapp.cn

K. JSON 与序列化
来源：http://jg.bookmarksfly.cn

================================================================================
来源：http://il.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://ia.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://et.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bo.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://jc.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://ps.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ff.nszjky.cn

Go:   json.Marshal(obj)
来源：http://ns.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ns.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ej.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://vv.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://oc.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qx.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ls.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://mv.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hu.jianghongdianzi.cn

Go:   json.Unmarshal(data, &v)
来源：http://iu.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://yc.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gs.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://rl.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rl.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sz.yuexingan06.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ll.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bo.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kk.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://so.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mt.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mb.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://nj.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yu.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ap.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ds.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mi.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fw.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yn.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bt.nicolike.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ne.shxzskj.cn

[K05] 深拷贝对象
来源：http://mz.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://rd.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://qk.hahajie.cn

JS:   structuredClone(obj)
来源：http://so.jianghongdianzi.cn

TS:   structuredClone(obj)
来源：http://qi.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rh.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ww.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lw.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ms.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://oq.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rn.szxytkj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ow.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iq.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dq.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bk.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iq.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yf.wgjwhj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ez.9csxet.cn

[K07] 进制转换
来源：http://gd.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ld.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fu.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fb.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://el.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qo.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vb.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://py.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xg.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://zo.asd995.cn

Py:   pickle.dumps(obj)
来源：http://hr.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pp.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://tb.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://sg.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://re.colortex.cn

Go:   encoding/gob
来源：http://xw.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://bi.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fq.wgjwhj.cn

================================================================================
来源：http://th.szsharing.cn

L. 网络请求
来源：http://ht.bookmarksfly.cn

================================================================================
来源：http://ul.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://fq.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ds.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://me.colortex.cn

JS:   await fetch(url)
来源：http://rg.shxzukj.cn

TS:   await fetch(url)
来源：http://pw.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vv.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://re.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ni.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xx.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://be.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://od.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yr.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lb.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uo.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wv.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eg.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hc.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bm.newstarts.cn

[L03] 设置自定义请求头
来源：http://kq.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://va.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jy.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://su.521024.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yb.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wp.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ca.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ld.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bd.yuntaijiaju.cn

[L04] 设置超时
来源：http://uz.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ha.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ki.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rz.nicolike.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://og.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yd.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bo.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ri.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://mh.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://un.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jn.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dg.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bx.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bi.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ey.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://od.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xl.521024.cn

[L06] 解析响应为 JSON
来源：http://sr.lnxyls.cn

Py:   resp.json()
来源：http://zy.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://vl.nicolike.cn

JS:   await resp.json()
来源：http://cy.nicolike.cn

TS:   await resp.json()
来源：http://nn.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ws.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vr.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://tv.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qb.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://xy.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sd.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ok.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://ty.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://mz.muxihuayi.cn

Java: resp.statusCode()
来源：http://wt.nszjky.cn

Go:   resp.StatusCode
来源：http://mo.gzmigu.cn

Ruby: resp.code.to_i
来源：http://bb.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://ft.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://cr.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kg.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://iu.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zl.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oz.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ts.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pq.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://og.9csxet.cn

================================================================================
来源：http://dt.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ah.hnjuh.cn

================================================================================
来源：http://xc.hnjuh.cn

[M01] 读取命令行参数
来源：http://bo.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://on.asd995.cn

PHP:  $argv;  $argc;
来源：http://xv.yuexingan06.cn

JS:   process.argv.slice(2)
来源：http://kp.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://sw.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://px.wgjwhj.cn

Go:   os.Args[1:]
来源：http://lq.huixiangedu.cn

Ruby: ARGV
来源：http://ax.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://uk.haigaiapp.cn

[M02] 读取环境变量
来源：http://fr.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://bx.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ih.chemitech.net.cn

JS:   process.env.HOME
来源：http://qk.shxzukj.cn

TS:   process.env.HOME
来源：http://ha.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://oq.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qc.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ls.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uo.asd995.cn

[M03] 执行外部命令
来源：http://ge.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fi.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jn.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zz.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cj.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://di.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ik.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://eo.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://mz.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://hz.szxytkj.cn

Py:   os.getcwd()
来源：http://tt.muxihuayi.cn

PHP:  getcwd();
来源：http://sb.huixiangedu.cn

JS:   process.cwd()
来源：http://bp.nszjky.cn

TS:   process.cwd()
来源：http://kh.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://jp.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://pj.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ud.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cw.asd995.cn

[M05] 设置退出码
来源：http://vn.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://gm.colortex.cn

PHP:  exit(1);
来源：http://um.gzmigu.cn

JS:   process.exit(1)
来源：http://cr.huanxung.cn

TS:   process.exit(1)
来源：http://kf.newstarts.cn

Java: System.exit(1)
来源：http://st.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://zu.asd995.cn

Ruby: exit 1
来源：http://lw.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bm.colortex.cn

[M06] 向标准错误输出
来源：http://zj.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://qn.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sy.muxihuayi.cn

JS:   console.error("err")
来源：http://jj.yuntaijiaju.cn

TS:   console.error("err")
来源：http://vl.asd995.cn

Java: System.err.println("err")
来源：http://iv.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fl.9csxet.cn

Ruby: warn "err"
来源：http://xr.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://bm.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://lc.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://vu.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fx.shxzukj.cn

JS:   require.main === module
来源：http://ym.shxzukj.cn

TS:   require.main === module
来源：http://qb.nszjky.cn

Java: public static void main(String[] args)
来源：http://rq.colortex.cn

Go:   func main()
来源：http://io.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ve.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://jn.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://aa.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://dc.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://pa.521024.cn

JS:   process.platform;  process.version
来源：http://zf.521024.cn

TS:   process.platform;  process.version
来源：http://ho.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xa.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ig.521024.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://un.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sc.bookmarksfly.cn

================================================================================
来源：http://an.colortex.cn

N. 数据结构与算法
来源：http://bz.huanxung.cn

================================================================================
来源：http://fs.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://xu.hnjuh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ql.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ho.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uy.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ao.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eo.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://kl.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vu.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ij.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://lp.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fy.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hf.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dy.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kc.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kx.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://lk.yuntaijiaju.cn

Ruby: arr.sort
来源：http://fu.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ee.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://hl.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cm.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://pf.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ma.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yv.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://it.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kn.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oo.wgjwhj.cn

[N04] 斐波那契数列
来源：http://as.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ve.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cl.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nt.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pg.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fr.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bu.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sf.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qd.gzmigu.cn

[N05] 最大公约数
来源：http://il.9csxet.cn

Py:   math.gcd(a, b)
来源：http://yb.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ml.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yv.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wo.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://av.newstarts.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hk.hahajie.cn

Ruby: a.gcd(b)
来源：http://ya.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ag.gzmigu.cn

[N06] 判断回文字符串
来源：http://is.chemitech.net.cn

Py:   s == s[::-1]
来源：http://ok.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://gj.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://br.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://bo.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kt.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://nx.muxihuayi.cn

Ruby: s == s.reverse
来源：http://wz.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iy.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://wz.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dw.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cg.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pe.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://ai.colortex.cn

Java: // 手写 HashMap
来源：http://pr.bjjhwx.cn


<!-- 参考信息 -->