代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zm.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lp.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tp.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dr.shxzskj.cn

================================================================================
来源：http://rk.muxihuayi.cn

K. JSON 与序列化
来源：http://tj.newstarts.cn

================================================================================
来源：http://ko.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://gu.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zb.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yv.panjiajie.cn

JS:   JSON.stringify(obj)
来源：http://zz.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://iz.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vi.asd995.cn

Go:   json.Marshal(obj)
来源：http://jz.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xh.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vt.hahajie.cn

[K02] JSON 字符串转对象
来源：http://jc.521024.cn

Py:   json.loads(s)
来源：http://eb.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zc.nszjky.cn

JS:   JSON.parse(s)
来源：http://ex.huanxung.cn

TS:   JSON.parse(s)
来源：http://sx.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fe.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wp.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://pk.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iq.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://oe.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mk.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ux.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ds.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ht.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zs.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://og.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qt.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://py.hahajie.cn

[K04] 读取 JSON 文件
来源：http://bp.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ep.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://da.huixiangedu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ed.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dj.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xh.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ry.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ic.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ch.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://ko.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://qm.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://xz.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://wb.asd995.cn

TS:   structuredClone(obj)
来源：http://jd.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fi.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vh.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xx.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tv.nicolike.cn

[K06] 解析 URL 查询串
来源：http://ni.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uh.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qs.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ra.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ds.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dm.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cn.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gx.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://he.nicolike.cn

[K07] 进制转换
来源：http://xu.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zs.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dk.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://un.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ao.huixiangedu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vk.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vm.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://el.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mx.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://jq.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://gb.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cx.newstarts.cn

JS:   v8.serialize(obj)        // Node
来源：http://jy.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://tv.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rs.wgjwhj.cn

Go:   encoding/gob
来源：http://cm.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://ps.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mw.nszjky.cn

================================================================================
来源：http://gs.muxihuayi.cn

L. 网络请求
来源：http://mv.shtwfgs.cn

================================================================================
来源：http://yk.hnjuh.cn

[L01] 发送 GET 请求
来源：http://nc.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vv.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ad.bookmarksfly.cn

JS:   await fetch(url)
来源：http://ws.hnjuh.cn

TS:   await fetch(url)
来源：http://qn.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tx.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://sd.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eu.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nh.9csxet.cn

[L02] 发送 POST JSON
来源：http://pp.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ga.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eq.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mj.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sk.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ds.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lv.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pk.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mz.huanxung.cn

[L03] 设置自定义请求头
来源：http://jj.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hh.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uw.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ti.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bg.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uf.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dr.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xh.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.huixiangedu.cn

[L04] 设置超时
来源：http://wu.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://go.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pw.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hr.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://he.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://se.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fs.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ly.huanxung.cn

[L05] 上传文件（multipart）
来源：http://hy.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dv.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ll.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yu.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nb.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://or.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lv.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bj.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xy.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://wx.jctech888.com.cn

Py:   resp.json()
来源：http://qa.huanxung.cn

PHP:  json_decode($body, true);
来源：http://by.shtwfgs.cn

JS:   await resp.json()
来源：http://ao.shxzukj.cn

TS:   await resp.json()
来源：http://vg.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qr.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://au.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://jt.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://le.yuexingan06.cn

[L07] 处理 HTTP 状态码
来源：http://yy.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zk.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ey.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://wh.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://ce.szsharing.cn

Java: resp.statusCode()
来源：http://to.colortex.cn

Go:   resp.StatusCode
来源：http://ei.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://hb.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://wh.colortex.cn

[L08] 并发请求多个地址
来源：http://nn.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qr.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://xx.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rv.newstarts.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://as.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ln.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iv.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lv.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mq.shxzukj.cn

================================================================================
来源：http://vq.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://je.asd995.cn

================================================================================
来源：http://am.shxzskj.cn

[M01] 读取命令行参数
来源：http://up.lnxyls.cn

Py:   sys.argv[1:]
来源：http://sy.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://yh.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://ym.colortex.cn

TS:   process.argv.slice(2)
来源：http://mb.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://rq.nszjky.cn

Go:   os.Args[1:]
来源：http://mi.huixiangedu.cn

Ruby: ARGV
来源：http://rp.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://qo.bjjhwx.cn

[M02] 读取环境变量
来源：http://eg.521024.cn

Py:   os.environ.get("HOME")
来源：http://zf.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yw.muxihuayi.cn

JS:   process.env.HOME
来源：http://xz.gzmigu.cn

TS:   process.env.HOME
来源：http://nt.hahajie.cn

Java: System.getenv("HOME")
来源：http://fj.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kc.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://yw.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cb.chemitech.net.cn

[M03] 执行外部命令
来源：http://xb.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://le.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lq.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vc.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jv.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nt.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://td.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ay.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://dh.hnjuh.cn

[M04] 获取当前工作目录
来源：http://if.bookmarksfly.cn

Py:   os.getcwd()
来源：http://gb.yuexingan06.cn

PHP:  getcwd();
来源：http://mm.wgjwhj.cn

JS:   process.cwd()
来源：http://td.yuexingan06.cn

TS:   process.cwd()
来源：http://fc.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kc.newstarts.cn

Go:   os.Getwd()
来源：http://kf.lnxyls.cn

Ruby: Dir.pwd
来源：http://mq.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sc.asd995.cn

[M05] 设置退出码
来源：http://ms.gzmigu.cn

Py:   sys.exit(1)
来源：http://ff.lnxyls.cn

PHP:  exit(1);
来源：http://de.muxihuayi.cn

JS:   process.exit(1)
来源：http://dx.yuexingan06.cn

TS:   process.exit(1)
来源：http://ut.jctech888.com.cn

Java: System.exit(1)
来源：http://xz.shxzskj.cn

Go:   os.Exit(1)
来源：http://ab.muxihuayi.cn

Ruby: exit 1
来源：http://sf.shxzukj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pv.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ia.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://pn.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://di.9csxet.cn

JS:   console.error("err")
来源：http://we.panjiajie.cn

TS:   console.error("err")
来源：http://gb.9csxet.cn

Java: System.err.println("err")
来源：http://qq.yuntaijiaju.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bb.newstarts.cn

Ruby: warn "err"
来源：http://kl.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://cc.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://pq.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://rh.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://il.chemitech.net.cn

JS:   require.main === module
来源：http://ue.yuexingan06.cn

TS:   require.main === module
来源：http://jv.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://nt.yuexingan06.cn

Go:   func main()
来源：http://pq.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://en.newstarts.cn

C#:   static void Main(string[] args)
来源：http://dz.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://he.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://lm.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://tn.shxzskj.cn

JS:   process.platform;  process.version
来源：http://dp.nszjky.cn

TS:   process.platform;  process.version
来源：http://xz.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fg.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wl.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://az.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dn.bjjhwx.cn

================================================================================
来源：http://ww.jianghongdianzi.cn

N. 数据结构与算法
来源：http://qs.hnjuh.cn

================================================================================
来源：http://yb.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://fd.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sk.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://si.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lp.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vs.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://od.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://km.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cm.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wl.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://kj.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://lb.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nr.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ko.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mv.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gb.yuntaijiaju.cn

Go:   slices.Sort(arr)
来源：http://xf.521024.cn

Ruby: arr.sort
来源：http://mg.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ie.asd995.cn

[N03] 快速排序（分治示例）
来源：http://ys.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ta.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ir.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fj.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mj.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://te.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jp.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ni.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tp.newstarts.cn

[N04] 斐波那契数列
来源：http://xr.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vn.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aq.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ii.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lk.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gc.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qv.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ni.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mn.haigaiapp.cn

[N05] 最大公约数
来源：http://us.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://dm.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fb.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kd.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://px.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nw.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xo.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://nf.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yh.lnxyls.cn

[N06] 判断回文字符串
来源：http://ok.asd995.cn

Py:   s == s[::-1]
来源：http://fd.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ht.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://mt.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://bd.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hu.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://qg.gzmigu.cn

Ruby: s == s.reverse
来源：http://kc.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cs.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://db.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qe.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ga.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vt.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://hd.hahajie.cn

Java: // 手写 HashMap
来源：http://dr.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://ci.hahajie.cn

Ruby: // 手写 Hash
来源：http://ch.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kg.newstarts.cn

[N08] 生成全排列
来源：http://ik.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://pj.hahajie.cn

PHP:  // 手写递归交换
来源：http://db.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://wa.hnjuh.cn

TS:   // 手写回溯递归
来源：http://qq.colortex.cn


<!-- 参考信息 -->