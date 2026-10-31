代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hb.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vs.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cg.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zo.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://to.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qg.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fl.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xx.huanxung.cn

================================================================================
来源：http://ye.shxzskj.cn

K. JSON 与序列化
来源：http://yz.gzmigu.cn

================================================================================
来源：http://px.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://kw.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wc.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hw.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://vv.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://ti.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pq.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://uu.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dv.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ri.9csxet.cn

[K02] JSON 字符串转对象
来源：http://qa.nszjky.cn

Py:   json.loads(s)
来源：http://my.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mj.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://rn.panjiajie.cn

TS:   JSON.parse(s)
来源：http://ik.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ud.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://tv.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://kz.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xk.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://pp.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lo.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gm.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ba.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jr.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ks.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yx.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hn.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://py.huanxung.cn

[K04] 读取 JSON 文件
来源：http://ph.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kn.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yf.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://az.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://el.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lh.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oo.shxzukj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wv.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zg.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://rc.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://zc.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://tu.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://gd.asd995.cn

TS:   structuredClone(obj)
来源：http://qx.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zr.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gl.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ao.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zo.hahajie.cn

[K06] 解析 URL 查询串
来源：http://rb.huixinmuqiang.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gt.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bi.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://db.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://va.521024.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aj.shxzukj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yn.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cr.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dp.gzmigu.cn

[K07] 进制转换
来源：http://st.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mr.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://al.nszjky.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wx.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fp.szsharing.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dq.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://va.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jy.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vf.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://mn.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://pw.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ta.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://fa.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://wo.hahajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ww.szxytkj.cn

Go:   encoding/gob
来源：http://xs.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://rk.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mn.hnjuh.cn

================================================================================
来源：http://tr.hahajie.cn

L. 网络请求
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://cx.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://tb.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cl.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ba.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://fy.nicolike.cn

TS:   await fetch(url)
来源：http://nx.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kd.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://ah.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ol.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ce.panjiajie.cn

[L02] 发送 POST JSON
来源：http://uw.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://us.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wu.wgjwhj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tn.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cp.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wp.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://km.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yp.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eb.newstarts.cn

[L03] 设置自定义请求头
来源：http://jp.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bx.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ws.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cw.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xq.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ga.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sm.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cm.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vu.huanxung.cn

[L04] 设置超时
来源：http://rv.jctech888.com.cn

Py:   requests.get(url, timeout=5)
来源：http://yv.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nh.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rx.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bx.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qw.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://no.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ok.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nw.newstarts.cn

[L05] 上传文件（multipart）
来源：http://dr.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://de.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jp.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bt.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fl.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ci.yuexingan06.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xm.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ev.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.newstarts.cn

[L06] 解析响应为 JSON
来源：http://ls.bookmarksfly.cn

Py:   resp.json()
来源：http://py.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://vn.hnjuh.cn

JS:   await resp.json()
来源：http://lo.muxihuayi.cn

TS:   await resp.json()
来源：http://cv.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hj.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pt.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://nb.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ai.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://tq.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yz.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fg.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://wc.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://bx.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://ga.huixiangedu.cn

Go:   resp.StatusCode
来源：http://ow.colortex.cn

Ruby: resp.code.to_i
来源：http://ll.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://ps.huanxung.cn

[L08] 并发请求多个地址
来源：http://ta.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ls.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://rd.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tt.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kf.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kt.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xx.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jz.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bj.huixiangedu.cn

================================================================================
来源：http://sj.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://ha.chemitech.net.cn

================================================================================
来源：http://du.huixiangedu.cn

[M01] 读取命令行参数
来源：http://eo.shxzukj.cn

Py:   sys.argv[1:]
来源：http://gr.szsharing.cn

PHP:  $argv;  $argc;
来源：http://cs.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://yz.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://id.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://hm.yuntaijiaju.cn

Go:   os.Args[1:]
来源：http://vh.gzmigu.cn

Ruby: ARGV
来源：http://rw.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://ch.panjiajie.cn

[M02] 读取环境变量
来源：http://ww.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://rp.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uh.jctech888.com.cn

JS:   process.env.HOME
来源：http://ka.nszjky.cn

TS:   process.env.HOME
来源：http://pa.521024.cn

Java: System.getenv("HOME")
来源：http://cr.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ca.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://xq.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vl.9csxet.cn

[M03] 执行外部命令
来源：http://po.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wc.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pe.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dr.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rk.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ju.jianghongdianzi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fu.bookmarksfly.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fo.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://pd.shxzskj.cn

[M04] 获取当前工作目录
来源：http://qa.shxzukj.cn

Py:   os.getcwd()
来源：http://mp.asd995.cn

PHP:  getcwd();
来源：http://zi.shtwfgs.cn

JS:   process.cwd()
来源：http://rl.shxzukj.cn

TS:   process.cwd()
来源：http://jl.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://cv.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://in.bjjhwx.cn

Ruby: Dir.pwd
来源：http://wd.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zc.wgjwhj.cn

[M05] 设置退出码
来源：http://vu.asd995.cn

Py:   sys.exit(1)
来源：http://ap.szsharing.cn

PHP:  exit(1);
来源：http://qt.521024.cn

JS:   process.exit(1)
来源：http://uf.gzmigu.cn

TS:   process.exit(1)
来源：http://xt.szxytkj.cn

Java: System.exit(1)
来源：http://fk.szxytkj.cn

Go:   os.Exit(1)
来源：http://tj.wgjwhj.cn

Ruby: exit 1
来源：http://ja.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lm.jctech888.com.cn

[M06] 向标准错误输出
来源：http://lk.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://vt.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://em.shtwfgs.cn

JS:   console.error("err")
来源：http://cs.yuexingan06.cn

TS:   console.error("err")
来源：http://hd.hnjuh.cn

Java: System.err.println("err")
来源：http://mm.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xx.huixiangedu.cn

Ruby: warn "err"
来源：http://gm.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://vi.9csxet.cn

[M07] 判断是否为主入口
来源：http://al.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://fb.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tj.lnxyls.cn

JS:   require.main === module
来源：http://ut.yuntaijiaju.cn

TS:   require.main === module
来源：http://kz.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://mm.huixiangedu.cn

Go:   func main()
来源：http://im.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xr.521024.cn

C#:   static void Main(string[] args)
来源：http://hs.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://sr.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://do.yuexingan06.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.asd995.cn

JS:   process.platform;  process.version
来源：http://nw.colortex.cn

TS:   process.platform;  process.version
来源：http://xe.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pc.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pd.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sy.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vd.hahajie.cn

================================================================================
来源：http://dc.wgjwhj.cn

N. 数据结构与算法
来源：http://gz.asd995.cn

================================================================================
来源：http://se.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://xv.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vg.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hk.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uv.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gs.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mk.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://wo.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jn.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://op.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://zb.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://xq.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sx.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ix.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://is.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kp.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://ra.newstarts.cn

Ruby: arr.sort
来源：http://or.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lc.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://oq.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://me.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://rc.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uz.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cw.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fx.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://re.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yp.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rh.wgjwhj.cn

[N04] 斐波那契数列
来源：http://by.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lu.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rr.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yx.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ke.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oc.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fd.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dh.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://se.shtwfgs.cn

[N05] 最大公约数
来源：http://me.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://fn.asd995.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wz.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://be.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tc.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iy.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dj.521024.cn

Ruby: a.gcd(b)
来源：http://rb.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://db.shxzukj.cn

[N06] 判断回文字符串
来源：http://po.huixiangedu.cn

Py:   s == s[::-1]
来源：http://yq.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://kh.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://gy.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://ob.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qc.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://kr.hnjuh.cn

Ruby: s == s.reverse
来源：http://ft.haigaiapp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ik.colortex.cn

[N07] 两数之和（返回下标）
来源：http://bf.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nf.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ow.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://js.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://hr.muxihuayi.cn

Java: // 手写 HashMap
来源：http://tv.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://ds.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://gx.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lb.nicolike.cn

[N08] 生成全排列
来源：http://xd.chemitech.net.cn


<!-- 参考信息 -->