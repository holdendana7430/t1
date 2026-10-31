代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zb.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vq.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zl.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qa.nszjky.cn

================================================================================
来源：http://fe.panjiajie.cn

K. JSON 与序列化
来源：http://uj.colortex.cn

================================================================================
来源：http://cb.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://kx.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cv.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://us.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://sa.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://nk.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://de.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://bz.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dm.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sn.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://le.asd995.cn

Py:   json.loads(s)
来源：http://qu.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ky.szsharing.cn

JS:   JSON.parse(s)
来源：http://oc.nszjky.cn

TS:   JSON.parse(s)
来源：http://fz.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fz.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://rx.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://cn.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gm.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.colortex.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nb.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pj.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ha.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vl.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pv.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cw.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yi.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://rs.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ln.bookmarksfly.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mt.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://up.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bp.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xj.nszjky.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xh.nszjky.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zu.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ej.hahajie.cn

[K05] 深拷贝对象
来源：http://up.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://di.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ip.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://cw.szsharing.cn

TS:   structuredClone(obj)
来源：http://pq.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pq.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wk.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://my.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dm.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://ch.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pr.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kd.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mu.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jz.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qi.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://im.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://la.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://id.haigaiapp.cn

[K07] 进制转换
来源：http://wx.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vp.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tb.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ns.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hf.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gq.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gq.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ck.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lc.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://wq.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ev.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ci.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://mz.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://th.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://po.lnxyls.cn

Go:   encoding/gob
来源：http://hj.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://yo.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lj.nszjky.cn

================================================================================
来源：http://tu.szxytkj.cn

L. 网络请求
来源：http://pv.yuexingan06.cn

================================================================================
来源：http://lu.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://dq.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://md.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kn.szsharing.cn

JS:   await fetch(url)
来源：http://jn.colortex.cn

TS:   await fetch(url)
来源：http://dt.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rq.521024.cn

Go:   resp, err := http.Get(url)
来源：http://yl.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gp.yuexingan06.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vs.9csxet.cn

[L02] 发送 POST JSON
来源：http://aq.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bt.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ju.lnxyls.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gm.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hn.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hi.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://es.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ge.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://hh.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qz.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xw.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lq.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sw.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mq.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nh.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lu.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hw.9csxet.cn

[L04] 设置超时
来源：http://qq.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://fx.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ef.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://we.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ab.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://on.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iy.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://if.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ko.521024.cn

[L05] 上传文件（multipart）
来源：http://wo.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yy.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ao.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uf.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sv.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://db.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oe.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ee.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iu.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://vj.jianghongdianzi.cn

Py:   resp.json()
来源：http://xr.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://fz.haigaiapp.cn

JS:   await resp.json()
来源：http://zg.huanxung.cn

TS:   await resp.json()
来源：http://aw.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mw.lnxyls.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hv.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://jq.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gc.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://aj.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cx.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cd.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://lv.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://jj.nszjky.cn

Java: resp.statusCode()
来源：http://la.szxytkj.cn

Go:   resp.StatusCode
来源：http://bw.colortex.cn

Ruby: resp.code.to_i
来源：http://yf.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://me.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://ep.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kz.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://hf.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qh.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jq.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ti.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mi.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://md.hnjuh.cn

================================================================================
来源：http://qu.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://rx.yuexingan06.cn

================================================================================
来源：http://nf.yuexingan06.cn

[M01] 读取命令行参数
来源：http://th.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ox.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://xs.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://wv.asd995.cn

TS:   process.argv.slice(2)
来源：http://ix.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://ac.panjiajie.cn

Go:   os.Args[1:]
来源：http://cl.chemitech.net.cn

Ruby: ARGV
来源：http://gg.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://qg.jctech888.com.cn

[M02] 读取环境变量
来源：http://jm.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://ig.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xk.haigaiapp.cn

JS:   process.env.HOME
来源：http://fv.szsharing.cn

TS:   process.env.HOME
来源：http://kt.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://um.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eu.nszjky.cn

Ruby: ENV["HOME"]
来源：http://nu.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xi.hnjuh.cn

[M03] 执行外部命令
来源：http://nr.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qk.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nv.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gz.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jo.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vy.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pk.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zv.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://ca.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://ec.colortex.cn

Py:   os.getcwd()
来源：http://cd.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ud.chemitech.net.cn

JS:   process.cwd()
来源：http://ut.bjjhwx.cn

TS:   process.cwd()
来源：http://cq.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://ga.lnxyls.cn

Go:   os.Getwd()
来源：http://cj.chemitech.net.cn

Ruby: Dir.pwd
来源：http://ed.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vr.hnjuh.cn

[M05] 设置退出码
来源：http://pd.bjjhwx.cn

Py:   sys.exit(1)
来源：http://vr.colortex.cn

PHP:  exit(1);
来源：http://om.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://yx.chemitech.net.cn

TS:   process.exit(1)
来源：http://vw.yuexingan06.cn

Java: System.exit(1)
来源：http://rn.szsharing.cn

Go:   os.Exit(1)
来源：http://qm.huanxung.cn

Ruby: exit 1
来源：http://pk.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://es.hnjuh.cn

[M06] 向标准错误输出
来源：http://tb.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://vl.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dw.chemitech.net.cn

JS:   console.error("err")
来源：http://xt.newstarts.cn

TS:   console.error("err")
来源：http://ne.huixinmuqiang.cn

Java: System.err.println("err")
来源：http://nm.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pv.huixinmuqiang.cn

Ruby: warn "err"
来源：http://gl.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://jr.shxzukj.cn

[M07] 判断是否为主入口
来源：http://jg.521024.cn

Py:   if __name__ == "__main__":
来源：http://dw.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yg.muxihuayi.cn

JS:   require.main === module
来源：http://zs.huanxung.cn

TS:   require.main === module
来源：http://cc.shtwfgs.cn

Java: public static void main(String[] args)
来源：http://af.huixiangedu.cn

Go:   func main()
来源：http://ta.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://av.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://cg.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://yd.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://cp.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://cp.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://yz.szxytkj.cn

TS:   process.platform;  process.version
来源：http://gh.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iz.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ex.muxihuayi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uj.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lg.lnxyls.cn

================================================================================
来源：http://yi.szsharing.cn

N. 数据结构与算法
来源：http://wb.bjjhwx.cn

================================================================================
来源：http://ik.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://hh.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ke.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nq.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qv.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xo.shxzskj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pd.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://fi.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://da.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ad.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://mk.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ic.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vk.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cb.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fi.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yc.nszjky.cn

Go:   slices.Sort(arr)
来源：http://by.shxzskj.cn

Ruby: arr.sort
来源：http://sr.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dx.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://wp.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ba.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://az.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mf.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ty.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lu.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vk.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mg.panjiajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ai.lnxyls.cn

[N04] 斐波那契数列
来源：http://vp.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uy.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mb.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://os.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gf.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://la.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gb.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fg.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dq.haigaiapp.cn

[N05] 最大公约数
来源：http://vq.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://ma.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dq.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ef.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zf.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wj.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://at.shxzukj.cn

Ruby: a.gcd(b)
来源：http://pv.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rd.nszjky.cn

[N06] 判断回文字符串
来源：http://zj.wgjwhj.cn

Py:   s == s[::-1]
来源：http://wf.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://fm.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://gt.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://xm.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hx.huanxung.cn

Go:   // 双指针从两端比较
来源：http://so.gzmigu.cn

Ruby: s == s.reverse
来源：http://au.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ln.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://zv.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sj.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vy.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oq.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://rc.szsharing.cn

Java: // 手写 HashMap
来源：http://nu.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://xq.newstarts.cn

Ruby: // 手写 Hash
来源：http://bt.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fb.hahajie.cn

[N08] 生成全排列
来源：http://mg.asd995.cn

Py:   itertools.permutations(arr)
来源：http://uk.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://do.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://jk.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://cr.lnxyls.cn


<!-- 参考信息 -->