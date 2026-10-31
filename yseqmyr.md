代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://yw.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ri.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cu.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pb.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oh.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sm.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lw.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ci.asd995.cn

================================================================================
来源：http://je.huixiangedu.cn

K. JSON 与序列化
来源：http://ee.huanxung.cn

================================================================================
来源：http://bq.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://pn.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://js.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ex.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://gb.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://op.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jf.9csxet.cn

Go:   json.Marshal(obj)
来源：http://la.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://az.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fd.9csxet.cn

[K02] JSON 字符串转对象
来源：http://fv.asd995.cn

Py:   json.loads(s)
来源：http://bw.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ai.hnjuh.cn

JS:   JSON.parse(s)
来源：http://jh.nicolike.cn

TS:   JSON.parse(s)
来源：http://ga.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mw.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://sh.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://qe.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oj.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://mv.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oi.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lq.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qx.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ap.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fq.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gb.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://if.9csxet.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zw.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://hv.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fx.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://go.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yw.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bz.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://in.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ip.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gp.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vs.9csxet.cn

[K05] 深拷贝对象
来源：http://ch.shtwfgs.cn

Py:   copy.deepcopy(obj)
来源：http://rk.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://eg.huixinmuqiang.cn

JS:   structuredClone(obj)
来源：http://au.521024.cn

TS:   structuredClone(obj)
来源：http://wz.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vm.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eu.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uw.jctech888.com.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://up.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://uu.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://va.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zv.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sc.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kq.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uq.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lf.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mv.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vq.asd995.cn

[K07] 进制转换
来源：http://ke.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xc.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xz.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lp.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nc.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bp.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dc.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xh.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mx.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://tj.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://cp.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lx.gzmigu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gi.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://wn.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ji.nicolike.cn

Go:   encoding/gob
来源：http://kj.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://rl.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qm.jianghongdianzi.cn

================================================================================
来源：http://qo.9csxet.cn

L. 网络请求
来源：http://bg.colortex.cn

================================================================================
来源：http://vr.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://te.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xy.szsharing.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gr.szxytkj.cn

JS:   await fetch(url)
来源：http://kf.colortex.cn

TS:   await fetch(url)
来源：http://kv.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yv.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://ri.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fx.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hc.shxzskj.cn

[L02] 发送 POST JSON
来源：http://xx.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xy.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kw.panjiajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ve.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pv.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gs.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hk.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nb.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jx.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://ym.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xq.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ne.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cs.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sn.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zo.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gm.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oh.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mg.chemitech.net.cn

[L04] 设置超时
来源：http://pj.gzmigu.cn

Py:   requests.get(url, timeout=5)
来源：http://pe.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://db.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mg.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mm.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lv.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xb.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ww.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ol.9csxet.cn

[L05] 上传文件（multipart）
来源：http://wf.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sr.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dm.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pw.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ew.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gr.muxihuayi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fj.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kq.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ok.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://pv.9csxet.cn

Py:   resp.json()
来源：http://qo.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://py.wgjwhj.cn

JS:   await resp.json()
来源：http://mb.bookmarksfly.cn

TS:   await resp.json()
来源：http://ti.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hq.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ow.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://wd.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gg.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ld.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://va.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ay.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://ix.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://rv.521024.cn

Java: resp.statusCode()
来源：http://mm.shxzskj.cn

Go:   resp.StatusCode
来源：http://qq.lnxyls.cn

Ruby: resp.code.to_i
来源：http://zc.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://qq.colortex.cn

[L08] 并发请求多个地址
来源：http://do.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nn.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://bi.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vq.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://en.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zk.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xf.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ko.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ao.huanxung.cn

================================================================================
来源：http://ui.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://ng.lnxyls.cn

================================================================================
来源：http://fm.haigaiapp.cn

[M01] 读取命令行参数
来源：http://cv.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://un.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ge.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://ej.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://cc.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://hz.muxihuayi.cn

Go:   os.Args[1:]
来源：http://dx.newstarts.cn

Ruby: ARGV
来源：http://tt.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://jj.shxzukj.cn

[M02] 读取环境变量
来源：http://ak.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://vj.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bf.huanxung.cn

JS:   process.env.HOME
来源：http://ds.shxzskj.cn

TS:   process.env.HOME
来源：http://pz.colortex.cn

Java: System.getenv("HOME")
来源：http://xo.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vw.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://fd.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pm.wgjwhj.cn

[M03] 执行外部命令
来源：http://dn.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xs.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://om.huanxung.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gz.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wo.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yi.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kc.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zd.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://du.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://hs.shtwfgs.cn

Py:   os.getcwd()
来源：http://jg.jctech888.com.cn

PHP:  getcwd();
来源：http://qo.szxytkj.cn

JS:   process.cwd()
来源：http://ln.shtwfgs.cn

TS:   process.cwd()
来源：http://ib.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://zw.chemitech.net.cn

Go:   os.Getwd()
来源：http://yw.shxzskj.cn

Ruby: Dir.pwd
来源：http://en.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mx.lnxyls.cn

[M05] 设置退出码
来源：http://on.nszjky.cn

Py:   sys.exit(1)
来源：http://ln.hnjuh.cn

PHP:  exit(1);
来源：http://gr.yuexingan06.cn

JS:   process.exit(1)
来源：http://lo.shtwfgs.cn

TS:   process.exit(1)
来源：http://wz.yuntaijiaju.cn

Java: System.exit(1)
来源：http://wt.huixiangedu.cn

Go:   os.Exit(1)
来源：http://qy.hnjuh.cn

Ruby: exit 1
来源：http://hh.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ue.chemitech.net.cn

[M06] 向标准错误输出
来源：http://qo.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://pz.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ge.huanxung.cn

JS:   console.error("err")
来源：http://qq.9csxet.cn

TS:   console.error("err")
来源：http://ff.asd995.cn

Java: System.err.println("err")
来源：http://mb.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.asd995.cn

Ruby: warn "err"
来源：http://jn.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://hh.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://rj.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://qv.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fw.huanxung.cn

JS:   require.main === module
来源：http://of.szxytkj.cn

TS:   require.main === module
来源：http://lz.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://vj.shxzskj.cn

Go:   func main()
来源：http://em.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dv.nicolike.cn

C#:   static void Main(string[] args)
来源：http://hy.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://io.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://xq.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://rq.lnxyls.cn

JS:   process.platform;  process.version
来源：http://sw.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://yl.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gq.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ga.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ar.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gi.szxytkj.cn

================================================================================
来源：http://su.bjjhwx.cn

N. 数据结构与算法
来源：http://cc.lnxyls.cn

================================================================================
来源：http://kg.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://bp.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ea.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kl.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ec.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hn.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xb.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hu.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xq.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://kz.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://lc.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zm.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hk.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bj.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rk.hahajie.cn

Go:   slices.Sort(arr)
来源：http://uo.szsharing.cn

Ruby: arr.sort
来源：http://bw.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xh.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://le.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fr.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://sn.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nn.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sw.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dl.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xm.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fo.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dm.nszjky.cn

[N04] 斐波那契数列
来源：http://da.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://al.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://na.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dv.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ec.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ol.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uq.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pt.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qy.panjiajie.cn

[N05] 最大公约数
来源：http://om.hahajie.cn

Py:   math.gcd(a, b)
来源：http://xr.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dt.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://st.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tm.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cn.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xa.gzmigu.cn

Ruby: a.gcd(b)
来源：http://py.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cr.muxihuayi.cn

[N06] 判断回文字符串
来源：http://sf.jctech888.com.cn

Py:   s == s[::-1]
来源：http://wq.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://ci.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://vu.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://ha.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ge.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://tt.colortex.cn

Ruby: s == s.reverse
来源：http://uv.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yi.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://ij.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pa.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dx.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ki.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://jr.wgjwhj.cn

Java: // 手写 HashMap
来源：http://ha.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://ad.panjiajie.cn

Ruby: // 手写 Hash
来源：http://og.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uw.shxzukj.cn

[N08] 生成全排列
来源：http://tk.bjjhwx.cn


<!-- 参考信息 -->