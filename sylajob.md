代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oy.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ay.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wx.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kb.panjiajie.cn

================================================================================
来源：http://kg.hahajie.cn

K. JSON 与序列化
来源：http://hn.huixiangedu.cn

================================================================================
来源：http://zi.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ks.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qb.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vh.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://hc.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://gl.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ip.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://xd.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lj.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gp.nszjky.cn

[K02] JSON 字符串转对象
来源：http://ev.muxihuayi.cn

Py:   json.loads(s)
来源：http://ji.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pb.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://of.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://vd.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eb.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://tp.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://zv.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cp.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://fw.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ri.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gt.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://di.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cm.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vg.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://af.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jw.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://to.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://ol.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vw.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kv.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pg.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zt.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uv.gzmigu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jr.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ay.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yx.panjiajie.cn

[K05] 深拷贝对象
来源：http://qa.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://wq.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://ub.shxzskj.cn

JS:   structuredClone(obj)
来源：http://ll.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://xm.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hv.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yn.jianghongdianzi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mf.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qf.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://rz.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pu.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ua.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gv.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kt.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ut.szxytkj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ng.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fu.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pn.yuexingan06.cn

[K07] 进制转换
来源：http://qv.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wc.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pg.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://go.szsharing.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vp.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vm.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yp.jctech888.com.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wt.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nf.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://rs.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://hx.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sq.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ql.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://fn.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ww.bjjhwx.cn

Go:   encoding/gob
来源：http://kj.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://ni.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zx.shxzskj.cn

================================================================================
来源：http://rq.panjiajie.cn

L. 网络请求
来源：http://wv.yuntaijiaju.cn

================================================================================
来源：http://bx.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://yl.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tq.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rr.hahajie.cn

JS:   await fetch(url)
来源：http://bm.panjiajie.cn

TS:   await fetch(url)
来源：http://mi.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://df.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://xw.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ba.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zi.szsharing.cn

[L02] 发送 POST JSON
来源：http://gy.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rr.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qk.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kq.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pe.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oi.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zl.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ea.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mk.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://en.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uo.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pe.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vx.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mg.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ib.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://un.nszjky.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kq.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://px.colortex.cn

[L04] 设置超时
来源：http://jj.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://tp.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zd.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fs.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hb.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://da.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gx.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qe.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gg.colortex.cn

[L05] 上传文件（multipart）
来源：http://nb.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nr.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fp.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rq.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yu.yuexingan06.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ed.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sy.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ti.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nz.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://nu.wgjwhj.cn

Py:   resp.json()
来源：http://qz.nicolike.cn

PHP:  json_decode($body, true);
来源：http://yi.521024.cn

JS:   await resp.json()
来源：http://qp.521024.cn

TS:   await resp.json()
来源：http://zo.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fw.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sx.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://la.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ui.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://ev.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rb.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cx.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://mq.colortex.cn

TS:   resp.ok;  resp.status
来源：http://up.hnjuh.cn

Java: resp.statusCode()
来源：http://zs.asd995.cn

Go:   resp.StatusCode
来源：http://fc.colortex.cn

Ruby: resp.code.to_i
来源：http://wi.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ed.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://aw.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ow.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://vj.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yz.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xx.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bq.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rh.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://re.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wy.haigaiapp.cn

================================================================================
来源：http://eq.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://sz.colortex.cn

================================================================================
来源：http://fv.yuexingan06.cn

[M01] 读取命令行参数
来源：http://eh.huanxung.cn

Py:   sys.argv[1:]
来源：http://fi.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://xh.9csxet.cn

JS:   process.argv.slice(2)
来源：http://jb.9csxet.cn

TS:   process.argv.slice(2)
来源：http://oh.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://mh.hnjuh.cn

Go:   os.Args[1:]
来源：http://dv.huanxung.cn

Ruby: ARGV
来源：http://lw.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://xp.shtwfgs.cn

[M02] 读取环境变量
来源：http://nj.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://qn.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gx.shxzskj.cn

JS:   process.env.HOME
来源：http://dy.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://ty.colortex.cn

Java: System.getenv("HOME")
来源：http://vm.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bt.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://ug.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tu.hnjuh.cn

[M03] 执行外部命令
来源：http://ca.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vi.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bj.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pj.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qb.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vu.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eo.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vp.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://xd.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://lu.jctech888.com.cn

Py:   os.getcwd()
来源：http://wl.shtwfgs.cn

PHP:  getcwd();
来源：http://ft.huixinmuqiang.cn

JS:   process.cwd()
来源：http://um.muxihuayi.cn

TS:   process.cwd()
来源：http://uw.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://bj.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://mn.nszjky.cn

Ruby: Dir.pwd
来源：http://jd.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nw.jianghongdianzi.cn

[M05] 设置退出码
来源：http://up.huixiangedu.cn

Py:   sys.exit(1)
来源：http://rw.nicolike.cn

PHP:  exit(1);
来源：http://kx.asd995.cn

JS:   process.exit(1)
来源：http://rx.shxzskj.cn

TS:   process.exit(1)
来源：http://fn.muxihuayi.cn

Java: System.exit(1)
来源：http://yj.szxytkj.cn

Go:   os.Exit(1)
来源：http://kb.hahajie.cn

Ruby: exit 1
来源：http://as.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tq.lnxyls.cn

[M06] 向标准错误输出
来源：http://le.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://dq.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qj.muxihuayi.cn

JS:   console.error("err")
来源：http://in.chemitech.net.cn

TS:   console.error("err")
来源：http://mq.bookmarksfly.cn

Java: System.err.println("err")
来源：http://nx.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pc.yuntaijiaju.cn

Ruby: warn "err"
来源：http://rx.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://ul.shxzskj.cn

[M07] 判断是否为主入口
来源：http://wc.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://vb.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ud.haigaiapp.cn

JS:   require.main === module
来源：http://az.nszjky.cn

TS:   require.main === module
来源：http://iq.hnjuh.cn

Java: public static void main(String[] args)
来源：http://ux.wgjwhj.cn

Go:   func main()
来源：http://ka.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oh.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://qe.gzmigu.cn

[M08] 获取系统与运行时信息
来源：http://wj.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ur.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://nk.colortex.cn

JS:   process.platform;  process.version
来源：http://gj.hahajie.cn

TS:   process.platform;  process.version
来源：http://wr.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nb.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ui.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wa.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fu.muxihuayi.cn

================================================================================
来源：http://rn.nszjky.cn

N. 数据结构与算法
来源：http://el.shxzskj.cn

================================================================================
来源：http://lo.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://gx.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sf.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qp.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bb.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oi.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xl.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://zg.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://az.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xs.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://sk.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://lg.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ym.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nl.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jx.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pu.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://ue.huanxung.cn

Ruby: arr.sort
来源：http://fc.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zp.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://ey.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bp.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://jx.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fg.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tb.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uk.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dy.szxytkj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fs.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vn.wgjwhj.cn

[N04] 斐波那契数列
来源：http://yj.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ut.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wl.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xx.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://om.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dt.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hr.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://as.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://de.gzmigu.cn

[N05] 最大公约数
来源：http://by.muxihuayi.cn

Py:   math.gcd(a, b)
来源：http://py.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cq.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eb.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mx.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hw.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://er.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://pu.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ke.muxihuayi.cn

[N06] 判断回文字符串
来源：http://rs.hahajie.cn

Py:   s == s[::-1]
来源：http://nu.asd995.cn

PHP:  $s === strrev($s);
来源：http://id.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://aw.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://iq.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nl.9csxet.cn

Go:   // 双指针从两端比较
来源：http://oq.jctech888.com.cn

Ruby: s == s.reverse
来源：http://rg.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pk.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://mg.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://if.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wg.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jp.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://mg.wgjwhj.cn

Java: // 手写 HashMap
来源：http://mv.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://ax.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://ym.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qy.wgjwhj.cn

[N08] 生成全排列
来源：http://sf.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://uw.521024.cn

PHP:  // 手写递归交换
来源：http://uf.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://cm.szxytkj.cn

TS:   // 手写回溯递归
来源：http://au.shxzukj.cn


<!-- 参考信息 -->