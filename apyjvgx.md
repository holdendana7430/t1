代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ee.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ct.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://eb.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://pl.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gt.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://zf.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oq.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mr.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://wx.nszjky.cn

Py:   json.loads(s)
来源：http://sq.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zi.gzmigu.cn

JS:   JSON.parse(s)
来源：http://tr.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://il.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dl.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://yt.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://ys.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ld.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://dh.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fg.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gi.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xw.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qv.hnjuh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oj.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ea.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lw.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kk.jctech888.com.cn

[K04] 读取 JSON 文件
来源：http://nt.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://br.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nf.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wk.huixinmuqiang.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yw.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sf.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ss.shtwfgs.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wk.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ko.bjjhwx.cn

[K05] 深拷贝对象
来源：http://mp.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://fs.bookmarksfly.cn

PHP:  unserialize(serialize($obj));
来源：http://xi.9csxet.cn

JS:   structuredClone(obj)
来源：http://he.wgjwhj.cn

TS:   structuredClone(obj)
来源：http://nj.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pt.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://no.yuntaijiaju.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xx.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fg.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://mj.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oc.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ov.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://re.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vt.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dk.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vy.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gi.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jd.huixiangedu.cn

[K07] 进制转换
来源：http://us.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zr.haigaiapp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tr.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pm.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rh.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ee.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jd.chemitech.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://em.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hg.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ei.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ai.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bw.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://ir.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://of.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qh.muxihuayi.cn

Go:   encoding/gob
来源：http://zx.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://wc.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fx.yuexingan06.cn

================================================================================
来源：http://rf.yuexingan06.cn

L. 网络请求
来源：http://uc.haigaiapp.cn

================================================================================
来源：http://jj.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://tn.newstarts.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fd.huanxung.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nn.panjiajie.cn

JS:   await fetch(url)
来源：http://nw.gzmigu.cn

TS:   await fetch(url)
来源：http://hn.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jc.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://as.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ad.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rs.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://fz.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gm.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tg.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zf.panjiajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pl.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wa.huixiangedu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cp.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pf.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oh.panjiajie.cn

[L03] 设置自定义请求头
来源：http://cp.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wm.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yk.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://au.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pu.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sw.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ux.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qx.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ic.nszjky.cn

[L04] 设置超时
来源：http://kz.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://ut.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sx.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ji.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wo.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qz.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mm.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ov.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://od.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://ht.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qw.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://em.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jq.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://en.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yc.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yt.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ti.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jm.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://bq.huixiangedu.cn

Py:   resp.json()
来源：http://cr.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://ti.gzmigu.cn

JS:   await resp.json()
来源：http://aq.nicolike.cn

TS:   await resp.json()
来源：http://et.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ox.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pa.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://uw.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ao.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://ts.haigaiapp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dm.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://me.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://tk.521024.cn

TS:   resp.ok;  resp.status
来源：http://do.newstarts.cn

Java: resp.statusCode()
来源：http://xa.panjiajie.cn

Go:   resp.StatusCode
来源：http://cj.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://hg.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ws.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://os.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yr.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://cf.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nn.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kd.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ak.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fb.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mg.asd995.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wx.nszjky.cn

================================================================================
来源：http://kt.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://ne.wgjwhj.cn

================================================================================
来源：http://ra.colortex.cn

[M01] 读取命令行参数
来源：http://wk.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://kk.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://zi.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://vt.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ke.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://de.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ye.nicolike.cn

Ruby: ARGV
来源：http://me.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://bk.szxytkj.cn

[M02] 读取环境变量
来源：http://yt.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://qs.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ov.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://rd.newstarts.cn

TS:   process.env.HOME
来源：http://zg.gzmigu.cn

Java: System.getenv("HOME")
来源：http://to.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ic.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ve.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gh.lnxyls.cn

[M03] 执行外部命令
来源：http://dm.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lf.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xn.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yd.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zt.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ed.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vk.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mt.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ck.szxytkj.cn

[M04] 获取当前工作目录
来源：http://px.haigaiapp.cn

Py:   os.getcwd()
来源：http://es.521024.cn

PHP:  getcwd();
来源：http://iv.colortex.cn

JS:   process.cwd()
来源：http://oe.muxihuayi.cn

TS:   process.cwd()
来源：http://ap.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://uk.hahajie.cn

Go:   os.Getwd()
来源：http://qi.huanxung.cn

Ruby: Dir.pwd
来源：http://xb.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oh.szxytkj.cn

[M05] 设置退出码
来源：http://jy.huanxung.cn

Py:   sys.exit(1)
来源：http://ly.chemitech.net.cn

PHP:  exit(1);
来源：http://eq.yuntaijiaju.cn

JS:   process.exit(1)
来源：http://aw.huanxung.cn

TS:   process.exit(1)
来源：http://pg.bookmarksfly.cn

Java: System.exit(1)
来源：http://eb.shxzukj.cn

Go:   os.Exit(1)
来源：http://vk.panjiajie.cn

Ruby: exit 1
来源：http://ee.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nt.lnxyls.cn

[M06] 向标准错误输出
来源：http://bs.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ps.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xt.yuntaijiaju.cn

JS:   console.error("err")
来源：http://bz.muxihuayi.cn

TS:   console.error("err")
来源：http://me.9csxet.cn

Java: System.err.println("err")
来源：http://uv.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ks.521024.cn

Ruby: warn "err"
来源：http://ct.gzmigu.cn

C#:   Console.Error.WriteLine("err")
来源：http://kz.szsharing.cn

[M07] 判断是否为主入口
来源：http://ld.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://wh.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gl.shxzukj.cn

JS:   require.main === module
来源：http://uv.huixiangedu.cn

TS:   require.main === module
来源：http://vx.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://nx.shtwfgs.cn

Go:   func main()
来源：http://uj.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tl.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://eq.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://ut.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://br.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://tr.newstarts.cn

JS:   process.platform;  process.version
来源：http://wk.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ul.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eq.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xn.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sp.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jy.colortex.cn

================================================================================
来源：http://fb.lnxyls.cn

N. 数据结构与算法
来源：http://xk.szsharing.cn

================================================================================
来源：http://gr.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://pg.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cc.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ca.huixinmuqiang.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xl.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wp.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cz.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://sg.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gm.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rj.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ug.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://st.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://it.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kh.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fp.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xk.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://wo.jctech888.com.cn

Ruby: arr.sort
来源：http://pw.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uc.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://qx.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://us.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://ew.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mr.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ch.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tj.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eg.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bz.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kg.521024.cn

[N04] 斐波那契数列
来源：http://eq.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nt.chemitech.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fr.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zb.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mk.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sq.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://id.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qz.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uv.yuntaijiaju.cn

[N05] 最大公约数
来源：http://zi.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://kj.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ez.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lu.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xf.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gd.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tm.521024.cn

Ruby: a.gcd(b)
来源：http://ok.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gk.nszjky.cn

[N06] 判断回文字符串
来源：http://bw.huanxung.cn

Py:   s == s[::-1]
来源：http://og.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://qf.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://hl.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://jt.asd995.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ot.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://jz.asd995.cn

Ruby: s == s.reverse
来源：http://su.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sg.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://bn.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vc.jctech888.com.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ky.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fp.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://jt.shxzukj.cn

Java: // 手写 HashMap
来源：http://gn.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://mc.panjiajie.cn

Ruby: // 手写 Hash
来源：http://xb.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://db.wgjwhj.cn

[N08] 生成全排列
来源：http://qr.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://jw.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://ez.hahajie.cn

JS:   // 手写回溯递归
来源：http://gd.asd995.cn

TS:   // 手写回溯递归
来源：http://st.shxzskj.cn

Java: // 手写回溯递归
来源：http://da.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://dy.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://gw.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://lp.shtwfgs.cn

[N09] 栈与队列
来源：http://kb.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rb.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dh.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kh.huixinmuqiang.cn


<!-- 参考信息 -->