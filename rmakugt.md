代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tr.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xr.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tm.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ko.hahajie.cn

================================================================================
来源：http://jw.nszjky.cn

K. JSON 与序列化
来源：http://no.bjjhwx.cn

================================================================================
来源：http://rk.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ud.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://db.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ts.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://ek.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://pq.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mh.nicolike.cn

Go:   json.Marshal(obj)
来源：http://yl.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bc.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nj.521024.cn

[K02] JSON 字符串转对象
来源：http://yd.muxihuayi.cn

Py:   json.loads(s)
来源：http://tw.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mg.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://jv.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://oa.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ug.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://jp.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://ot.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://em.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://dx.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gc.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gt.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ki.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zs.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eb.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kg.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nn.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://au.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://nr.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ic.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ua.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rx.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pk.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bb.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aj.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://su.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tp.shxzukj.cn

[K05] 深拷贝对象
来源：http://wu.yuntaijiaju.cn

Py:   copy.deepcopy(obj)
来源：http://cd.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://zw.9csxet.cn

JS:   structuredClone(obj)
来源：http://ty.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://ks.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://df.9csxet.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gy.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pk.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vj.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://sl.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mg.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qj.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rg.colortex.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qd.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uk.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://um.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ok.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ok.colortex.cn

[K07] 进制转换
来源：http://qc.lnxyls.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hc.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ik.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hb.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mc.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cj.haigaiapp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://do.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://in.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kr.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qc.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://rk.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tk.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://if.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://in.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tq.newstarts.cn

Go:   encoding/gob
来源：http://us.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://yl.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hh.bookmarksfly.cn

================================================================================
来源：http://os.hnjuh.cn

L. 网络请求
来源：http://aj.bjjhwx.cn

================================================================================
来源：http://qu.shxzukj.cn

[L01] 发送 GET 请求
来源：http://dm.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gu.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fx.yuexingan06.cn

JS:   await fetch(url)
来源：http://jl.nicolike.cn

TS:   await fetch(url)
来源：http://pe.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ba.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://jp.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jm.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yv.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ks.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bt.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ll.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oh.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ac.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ph.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vw.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ro.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://op.shxzukj.cn

[L03] 设置自定义请求头
来源：http://kk.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uy.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wu.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pp.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ba.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tk.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iq.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xk.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://um.wgjwhj.cn

[L04] 设置超时
来源：http://qm.bookmarksfly.cn

Py:   requests.get(url, timeout=5)
来源：http://mt.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pa.gzmigu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gx.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sk.panjiajie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nt.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ju.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mz.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fw.hahajie.cn

[L05] 上传文件（multipart）
来源：http://dd.huanxung.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ah.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sv.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ez.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dz.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ax.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uh.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wr.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hv.lnxyls.cn

[L06] 解析响应为 JSON
来源：http://qc.yuexingan06.cn

Py:   resp.json()
来源：http://gl.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://vt.chemitech.net.cn

JS:   await resp.json()
来源：http://xb.shxzskj.cn

TS:   await resp.json()
来源：http://ne.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dv.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://el.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://vg.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://id.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://kr.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://we.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rd.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://zd.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://wv.hnjuh.cn

Java: resp.statusCode()
来源：http://yt.521024.cn

Go:   resp.StatusCode
来源：http://gh.szsharing.cn

Ruby: resp.code.to_i
来源：http://rd.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://hl.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://px.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://au.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://go.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qb.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bc.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vx.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xw.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ld.521024.cn

================================================================================
来源：http://yd.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://vv.shxzskj.cn

================================================================================
来源：http://pl.gzmigu.cn

[M01] 读取命令行参数
来源：http://ee.nicolike.cn

Py:   sys.argv[1:]
来源：http://vy.nszjky.cn

PHP:  $argv;  $argc;
来源：http://xw.colortex.cn

JS:   process.argv.slice(2)
来源：http://uw.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://aa.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ty.shxzukj.cn

Go:   os.Args[1:]
来源：http://jl.yuexingan06.cn

Ruby: ARGV
来源：http://rt.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://vc.chemitech.net.cn

[M02] 读取环境变量
来源：http://pp.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://nu.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gf.muxihuayi.cn

JS:   process.env.HOME
来源：http://mh.szxytkj.cn

TS:   process.env.HOME
来源：http://gt.shxzukj.cn

Java: System.getenv("HOME")
来源：http://zi.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://la.9csxet.cn

Ruby: ENV["HOME"]
来源：http://zr.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bi.9csxet.cn

[M03] 执行外部命令
来源：http://uf.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uq.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zz.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sr.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zb.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fu.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gy.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wy.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://cx.lnxyls.cn

[M04] 获取当前工作目录
来源：http://my.huanxung.cn

Py:   os.getcwd()
来源：http://az.wgjwhj.cn

PHP:  getcwd();
来源：http://nw.szxytkj.cn

JS:   process.cwd()
来源：http://ps.shxzukj.cn

TS:   process.cwd()
来源：http://bf.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://ml.wgjwhj.cn

Go:   os.Getwd()
来源：http://zj.521024.cn

Ruby: Dir.pwd
来源：http://gb.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zu.hnjuh.cn

[M05] 设置退出码
来源：http://kk.nicolike.cn

Py:   sys.exit(1)
来源：http://td.yuntaijiaju.cn

PHP:  exit(1);
来源：http://kf.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://mw.colortex.cn

TS:   process.exit(1)
来源：http://av.hahajie.cn

Java: System.exit(1)
来源：http://nk.521024.cn

Go:   os.Exit(1)
来源：http://nv.panjiajie.cn

Ruby: exit 1
来源：http://ma.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ql.bjjhwx.cn

[M06] 向标准错误输出
来源：http://dd.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://yg.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ve.shxzukj.cn

JS:   console.error("err")
来源：http://vy.panjiajie.cn

TS:   console.error("err")
来源：http://ap.colortex.cn

Java: System.err.println("err")
来源：http://vc.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ju.nszjky.cn

Ruby: warn "err"
来源：http://fm.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://db.szsharing.cn

[M07] 判断是否为主入口
来源：http://wh.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://hi.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://il.huanxung.cn

JS:   require.main === module
来源：http://ma.chemitech.net.cn

TS:   require.main === module
来源：http://lu.szxytkj.cn

Java: public static void main(String[] args)
来源：http://th.jctech888.com.cn

Go:   func main()
来源：http://dz.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wn.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://lu.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://ri.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://wv.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://tx.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://vs.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://av.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://am.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://io.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cq.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cy.shxzskj.cn

================================================================================
来源：http://lg.chemitech.net.cn

N. 数据结构与算法
来源：http://wn.bjjhwx.cn

================================================================================
来源：http://gi.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://rf.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uf.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eu.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qu.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sy.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dv.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://be.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pk.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iw.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://va.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://qr.jianghongdianzi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zd.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zl.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fd.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ai.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://rf.gzmigu.cn

Ruby: arr.sort
来源：http://ep.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gr.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://yv.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wt.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://rl.shtwfgs.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://si.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ru.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ix.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://js.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://og.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cx.nicolike.cn

[N04] 斐波那契数列
来源：http://fo.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uc.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jp.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://je.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bs.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pa.chemitech.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tw.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uk.hahajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rr.nicolike.cn

[N05] 最大公约数
来源：http://ep.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://jb.yuntaijiaju.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tq.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ru.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pb.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tf.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://le.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://kt.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://on.gzmigu.cn

[N06] 判断回文字符串
来源：http://nl.szsharing.cn

Py:   s == s[::-1]
来源：http://ow.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://xd.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://jg.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://vx.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eo.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://ng.szxytkj.cn

Ruby: s == s.reverse
来源：http://ba.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gg.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://by.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fm.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cw.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wk.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://rp.shtwfgs.cn

Java: // 手写 HashMap
来源：http://ie.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://iu.nszjky.cn

Ruby: // 手写 Hash
来源：http://ve.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xv.hahajie.cn

[N08] 生成全排列
来源：http://zl.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://ap.newstarts.cn

PHP:  // 手写递归交换
来源：http://bg.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://ti.newstarts.cn

TS:   // 手写回溯递归
来源：http://kx.nicolike.cn


<!-- 参考信息 -->