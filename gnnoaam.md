代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://un.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ex.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://af.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pl.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oe.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ki.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wv.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vk.colortex.cn

================================================================================
来源：http://rs.521024.cn

K. JSON 与序列化
来源：http://ni.hahajie.cn

================================================================================
来源：http://mw.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://ip.hahajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ai.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://am.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://uw.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://rg.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lw.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://eu.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wf.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nj.colortex.cn

[K02] JSON 字符串转对象
来源：http://jl.521024.cn

Py:   json.loads(s)
来源：http://yn.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eh.nszjky.cn

JS:   JSON.parse(s)
来源：http://ty.nicolike.cn

TS:   JSON.parse(s)
来源：http://oi.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vd.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://oj.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://hf.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jm.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://pz.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xh.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fl.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pk.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qn.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dp.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://be.szsharing.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rk.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zn.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://fl.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bq.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ui.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pd.newstarts.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dt.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wb.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qq.bjjhwx.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tz.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ge.huanxung.cn

[K05] 深拷贝对象
来源：http://eb.szsharing.cn

Py:   copy.deepcopy(obj)
来源：http://le.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://bu.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://xf.muxihuayi.cn

TS:   structuredClone(obj)
来源：http://wu.521024.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uu.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ed.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tb.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dp.521024.cn

[K06] 解析 URL 查询串
来源：http://si.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ri.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ji.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eg.wgjwhj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hl.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hl.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jf.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vp.shtwfgs.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tv.muxihuayi.cn

[K07] 进制转换
来源：http://xe.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://js.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uz.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bn.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zy.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vj.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ju.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://we.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zz.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qq.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ty.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ng.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://ao.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://vd.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nd.asd995.cn

Go:   encoding/gob
来源：http://mq.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://wm.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cb.bjjhwx.cn

================================================================================
来源：http://se.panjiajie.cn

L. 网络请求
来源：http://cz.521024.cn

================================================================================
来源：http://ce.asd995.cn

[L01] 发送 GET 请求
来源：http://wb.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iz.9csxet.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zy.chemitech.net.cn

JS:   await fetch(url)
来源：http://ok.shxzskj.cn

TS:   await fetch(url)
来源：http://ac.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pw.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://nm.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://an.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yc.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ph.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xl.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mp.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qh.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sa.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://au.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tz.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://am.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lh.szsharing.cn

[L03] 设置自定义请求头
来源：http://mk.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lu.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qv.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ac.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hy.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oj.newstarts.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nh.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://my.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cs.shxzskj.cn

[L04] 设置超时
来源：http://hp.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://no.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://la.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ez.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zw.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ll.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yy.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ki.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ls.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://vn.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qm.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xs.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://il.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vl.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ix.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xl.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xt.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ai.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sw.shtwfgs.cn

Py:   resp.json()
来源：http://ck.newstarts.cn

PHP:  json_decode($body, true);
来源：http://ef.lnxyls.cn

JS:   await resp.json()
来源：http://ti.nicolike.cn

TS:   await resp.json()
来源：http://aw.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zs.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://kr.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ap.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://rc.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fz.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://db.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://mg.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://nu.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://xi.szsharing.cn

Go:   resp.StatusCode
来源：http://vi.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://ew.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://zk.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://tr.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hk.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://kh.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ht.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mf.haigaiapp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nj.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kw.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gy.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yj.bookmarksfly.cn

================================================================================
来源：http://gd.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://cb.shtwfgs.cn

================================================================================
来源：http://cw.muxihuayi.cn

[M01] 读取命令行参数
来源：http://qb.newstarts.cn

Py:   sys.argv[1:]
来源：http://jw.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://vk.521024.cn

JS:   process.argv.slice(2)
来源：http://qv.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://mw.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://rf.hnjuh.cn

Go:   os.Args[1:]
来源：http://nz.yuexingan06.cn

Ruby: ARGV
来源：http://wf.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://cx.yuexingan06.cn

[M02] 读取环境变量
来源：http://qc.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://ic.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ju.lnxyls.cn

JS:   process.env.HOME
来源：http://oc.521024.cn

TS:   process.env.HOME
来源：http://ir.521024.cn

Java: System.getenv("HOME")
来源：http://jj.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ye.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://cj.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wx.panjiajie.cn

[M03] 执行外部命令
来源：http://iv.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://di.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vs.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nz.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ll.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://td.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xd.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://do.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://js.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://nx.huixiangedu.cn

Py:   os.getcwd()
来源：http://oa.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ts.szxytkj.cn

JS:   process.cwd()
来源：http://kc.yuexingan06.cn

TS:   process.cwd()
来源：http://kd.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ol.hahajie.cn

Go:   os.Getwd()
来源：http://ax.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://zr.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pu.9csxet.cn

[M05] 设置退出码
来源：http://yl.gzmigu.cn

Py:   sys.exit(1)
来源：http://mg.lnxyls.cn

PHP:  exit(1);
来源：http://gr.jctech888.com.cn

JS:   process.exit(1)
来源：http://tk.panjiajie.cn

TS:   process.exit(1)
来源：http://zj.shxzskj.cn

Java: System.exit(1)
来源：http://yr.gzmigu.cn

Go:   os.Exit(1)
来源：http://fg.asd995.cn

Ruby: exit 1
来源：http://uf.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://es.huixiangedu.cn

[M06] 向标准错误输出
来源：http://hi.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://di.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lz.chemitech.net.cn

JS:   console.error("err")
来源：http://pq.huixinmuqiang.cn

TS:   console.error("err")
来源：http://cs.jctech888.com.cn

Java: System.err.println("err")
来源：http://oc.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ly.521024.cn

Ruby: warn "err"
来源：http://wg.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://oj.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://bl.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://yy.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lr.jctech888.com.cn

JS:   require.main === module
来源：http://mq.hahajie.cn

TS:   require.main === module
来源：http://fl.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://er.huixiangedu.cn

Go:   func main()
来源：http://rv.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fn.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://la.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://zh.colortex.cn

Py:   platform.system();  platform.python_version()
来源：http://qx.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://qb.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://dv.shxzskj.cn

TS:   process.platform;  process.version
来源：http://vc.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kq.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bu.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mu.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pk.521024.cn

================================================================================
来源：http://yi.shxzukj.cn

N. 数据结构与算法
来源：http://nv.bookmarksfly.cn

================================================================================
来源：http://zz.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://tj.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yf.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jl.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rd.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ok.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kr.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://wv.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://me.yuexingan06.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gf.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://nq.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ap.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bp.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kb.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jj.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jt.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://md.newstarts.cn

Ruby: arr.sort
来源：http://gb.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xg.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://no.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ch.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://bl.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vg.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fl.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gn.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bc.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zh.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://md.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://is.shxzskj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sw.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fr.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yi.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ay.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qh.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://io.newstarts.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://na.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dy.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ph.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ie.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lx.asd995.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hx.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mw.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oe.gzmigu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ua.newstarts.cn

Ruby: a.gcd(b)
来源：http://ux.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hx.newstarts.cn

[N06] 判断回文字符串
来源：http://om.hnjuh.cn

Py:   s == s[::-1]
来源：http://sn.huanxung.cn

PHP:  $s === strrev($s);
来源：http://zu.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://kx.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://bg.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eo.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://tp.nszjky.cn

Ruby: s == s.reverse
来源：http://jr.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cf.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://bc.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ic.haigaiapp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://na.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oe.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://ze.shxzukj.cn

Java: // 手写 HashMap
来源：http://jm.nicolike.cn

Go:   // 手写 map[int]int
来源：http://cy.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://kc.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aa.shxzskj.cn

[N08] 生成全排列
来源：http://ng.shxzukj.cn


<!-- 参考信息 -->