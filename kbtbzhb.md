代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kv.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://if.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sk.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eu.hahajie.cn

================================================================================
来源：http://il.9csxet.cn

K. JSON 与序列化
来源：http://td.muxihuayi.cn

================================================================================
来源：http://vh.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://nd.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mt.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ic.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ww.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://rw.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://ct.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lt.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nm.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://zw.shtwfgs.cn

Py:   json.loads(s)
来源：http://cz.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://qb.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://gw.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fk.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://wc.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://ke.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://an.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://dt.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vu.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kc.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mu.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vv.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gl.9csxet.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vl.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nc.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cm.szsharing.cn

[K04] 读取 JSON 文件
来源：http://vo.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vz.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dw.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ig.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ig.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vr.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kq.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ts.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vq.wgjwhj.cn

[K05] 深拷贝对象
来源：http://ox.chemitech.net.cn

Py:   copy.deepcopy(obj)
来源：http://yf.nszjky.cn

PHP:  unserialize(serialize($obj));
来源：http://ih.shxzskj.cn

JS:   structuredClone(obj)
来源：http://nu.nicolike.cn

TS:   structuredClone(obj)
来源：http://ch.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lp.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pb.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ya.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qj.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://xj.huanxung.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ve.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gl.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xz.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xg.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bu.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qb.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zb.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qg.jctech888.com.cn

[K07] 进制转换
来源：http://cs.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gr.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jr.newstarts.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bs.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jg.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bh.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xg.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kg.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lt.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://gl.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://vk.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cd.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://ue.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://vp.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pw.haigaiapp.cn

Go:   encoding/gob
来源：http://bl.521024.cn

Ruby: Marshal.dump(obj)
来源：http://nn.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cx.gzmigu.cn

================================================================================
来源：http://xn.hahajie.cn

L. 网络请求
来源：http://bu.yuntaijiaju.cn

================================================================================
来源：http://xj.nszjky.cn

[L01] 发送 GET 请求
来源：http://ak.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hg.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dd.nicolike.cn

JS:   await fetch(url)
来源：http://qn.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://at.wgjwhj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qq.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://hs.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ka.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qb.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://qr.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rw.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ka.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qz.nszjky.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mk.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cd.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pq.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kc.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ej.shxzskj.cn

[L03] 设置自定义请求头
来源：http://fm.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://au.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ja.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ui.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://it.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://az.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://da.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qo.nicolike.cn

[L04] 设置超时
来源：http://ll.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://ae.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ag.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mo.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ul.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sp.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://au.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cs.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ph.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ml.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dd.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ea.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://py.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ai.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qc.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bt.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://it.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://qp.haigaiapp.cn

Py:   resp.json()
来源：http://rp.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://zy.nicolike.cn

JS:   await resp.json()
来源：http://ft.bookmarksfly.cn

TS:   await resp.json()
来源：http://mk.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lm.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vi.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://ty.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rw.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://cs.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hy.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://av.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://jj.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://vi.szsharing.cn

Java: resp.statusCode()
来源：http://ky.gzmigu.cn

Go:   resp.StatusCode
来源：http://kp.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://zo.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://kx.colortex.cn

[L08] 并发请求多个地址
来源：http://cy.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://be.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://ps.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gu.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nb.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ue.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pw.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ol.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ed.521024.cn

================================================================================
来源：http://ha.521024.cn

M. 命令行 / 进程 / 环境
来源：http://gq.wgjwhj.cn

================================================================================
来源：http://ng.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://en.hahajie.cn

Py:   sys.argv[1:]
来源：http://as.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://tl.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://xg.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://jk.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://lz.yuexingan06.cn

Go:   os.Args[1:]
来源：http://pn.asd995.cn

Ruby: ARGV
来源：http://hz.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://sj.shxzukj.cn

[M02] 读取环境变量
来源：http://iv.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://dg.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://al.9csxet.cn

JS:   process.env.HOME
来源：http://nz.nicolike.cn

TS:   process.env.HOME
来源：http://by.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://ri.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fx.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://ma.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bn.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://xz.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cb.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cw.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://th.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rd.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qe.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://td.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cx.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://dm.hnjuh.cn

[M04] 获取当前工作目录
来源：http://uc.bjjhwx.cn

Py:   os.getcwd()
来源：http://yb.hnjuh.cn

PHP:  getcwd();
来源：http://yt.lnxyls.cn

JS:   process.cwd()
来源：http://gc.jctech888.com.cn

TS:   process.cwd()
来源：http://vf.colortex.cn

Java: Path.of("").toAbsolutePath()
来源：http://sa.bookmarksfly.cn

Go:   os.Getwd()
来源：http://pz.shxzukj.cn

Ruby: Dir.pwd
来源：http://mp.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oz.colortex.cn

[M05] 设置退出码
来源：http://py.hahajie.cn

Py:   sys.exit(1)
来源：http://uj.jctech888.com.cn

PHP:  exit(1);
来源：http://ui.haigaiapp.cn

JS:   process.exit(1)
来源：http://pl.nszjky.cn

TS:   process.exit(1)
来源：http://hw.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ds.yuexingan06.cn

Go:   os.Exit(1)
来源：http://op.hahajie.cn

Ruby: exit 1
来源：http://wo.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mo.shxzukj.cn

[M06] 向标准错误输出
来源：http://eq.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://ht.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ik.szsharing.cn

JS:   console.error("err")
来源：http://oy.panjiajie.cn

TS:   console.error("err")
来源：http://pz.wgjwhj.cn

Java: System.err.println("err")
来源：http://uj.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rv.chemitech.net.cn

Ruby: warn "err"
来源：http://jr.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://gl.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://dx.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://oy.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zg.lnxyls.cn

JS:   require.main === module
来源：http://kd.haigaiapp.cn

TS:   require.main === module
来源：http://cq.9csxet.cn

Java: public static void main(String[] args)
来源：http://rg.nszjky.cn

Go:   func main()
来源：http://iw.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ru.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://jn.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://hd.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://is.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://cd.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://gj.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://rj.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ra.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ed.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mx.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nh.asd995.cn

================================================================================
来源：http://ia.nszjky.cn

N. 数据结构与算法
来源：http://wz.asd995.cn

================================================================================
来源：http://je.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://pw.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://br.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ep.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kx.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dt.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://on.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://qi.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mh.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yz.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://bh.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://we.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ae.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kk.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kr.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tj.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://tb.chemitech.net.cn

Ruby: arr.sort
来源：http://ao.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dd.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://rw.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gi.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://pw.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dv.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ni.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dv.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ns.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zy.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vp.9csxet.cn

[N04] 斐波那契数列
来源：http://xf.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://do.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ub.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kd.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ic.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sb.bookmarksfly.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ai.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gv.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oo.haigaiapp.cn

[N05] 最大公约数
来源：http://is.huanxung.cn

Py:   math.gcd(a, b)
来源：http://jm.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fi.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://js.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nq.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yy.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://py.lnxyls.cn

Ruby: a.gcd(b)
来源：http://bi.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fm.huanxung.cn

[N06] 判断回文字符串
来源：http://za.chemitech.net.cn

Py:   s == s[::-1]
来源：http://in.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://us.huanxung.cn

JS:   s === [...s].reverse().join("")
来源：http://ye.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://an.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fr.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://kx.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://sr.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://en.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://ci.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://re.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wv.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zw.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://ef.szsharing.cn

Java: // 手写 HashMap
来源：http://cn.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://qg.asd995.cn

Ruby: // 手写 Hash
来源：http://vm.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ic.521024.cn

[N08] 生成全排列
来源：http://su.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://xi.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://oa.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://vn.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://ew.nicolike.cn


<!-- 参考信息 -->