代发 wailian999

================================================================================
来源：http://kw.hahajie.cn

K. JSON 与序列化
来源：http://vq.newstarts.cn

================================================================================
来源：http://fc.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://eu.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qw.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ut.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://ml.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://mb.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nt.huanxung.cn

Go:   json.Marshal(obj)
来源：http://dm.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sk.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gi.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://fd.shxzukj.cn

Py:   json.loads(s)
来源：http://pi.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hk.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://zm.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://hd.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://on.szsharing.cn

Go:   json.Unmarshal(data, &v)
来源：http://ax.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://dm.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uk.shxzskj.cn

[K03] JSON 美化输出（带缩进）
来源：http://qe.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pl.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pe.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mv.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yv.shxzukj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jv.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://og.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wh.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ux.shtwfgs.cn

[K04] 读取 JSON 文件
来源：http://fj.colortex.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vv.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wa.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bx.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ng.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ro.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fr.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yz.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bg.chemitech.net.cn

[K05] 深拷贝对象
来源：http://ci.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://oz.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://fv.szsharing.cn

JS:   structuredClone(obj)
来源：http://gm.hahajie.cn

TS:   structuredClone(obj)
来源：http://gr.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yf.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cz.szxytkj.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://if.shxzskj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ad.nszjky.cn

[K06] 解析 URL 查询串
来源：http://ng.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vx.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://li.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lw.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gd.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dm.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ct.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qj.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fn.szxytkj.cn

[K07] 进制转换
来源：http://ly.muxihuayi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tn.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qv.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xp.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yc.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hv.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yp.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ur.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ej.jctech888.com.cn

[K08] 二进制序列化（非 JSON）
来源：http://ec.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://ij.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qo.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://vc.hahajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mg.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bs.yuntaijiaju.cn

Go:   encoding/gob
来源：http://rg.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://xa.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://or.hahajie.cn

================================================================================
来源：http://rj.haigaiapp.cn

L. 网络请求
来源：http://an.szsharing.cn

================================================================================
来源：http://pk.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://hw.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qz.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cv.9csxet.cn

JS:   await fetch(url)
来源：http://ir.szsharing.cn

TS:   await fetch(url)
来源：http://az.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uh.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://gx.szsharing.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ej.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gt.shxzukj.cn

[L02] 发送 POST JSON
来源：http://rr.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bj.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xj.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dv.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hp.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wj.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://je.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aw.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xa.hnjuh.cn

[L03] 设置自定义请求头
来源：http://px.yuntaijiaju.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dp.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bz.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vg.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ua.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nm.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gv.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ct.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ta.gzmigu.cn

[L04] 设置超时
来源：http://td.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://lm.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xj.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qc.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://el.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qr.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sj.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gl.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oh.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://yg.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qb.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ei.huanxung.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ka.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sk.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wr.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ai.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kx.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kg.nicolike.cn

[L06] 解析响应为 JSON
来源：http://di.jctech888.com.cn

Py:   resp.json()
来源：http://db.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://cf.shtwfgs.cn

JS:   await resp.json()
来源：http://mk.szxytkj.cn

TS:   await resp.json()
来源：http://jo.yuntaijiaju.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sk.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yu.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://lz.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tk.chemitech.net.cn

[L07] 处理 HTTP 状态码
来源：http://rm.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uu.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hd.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://ce.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://gb.wgjwhj.cn

Java: resp.statusCode()
来源：http://fo.szxytkj.cn

Go:   resp.StatusCode
来源：http://bq.nszjky.cn

Ruby: resp.code.to_i
来源：http://tg.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://qh.panjiajie.cn

[L08] 并发请求多个地址
来源：http://ne.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oe.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://zr.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ib.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sw.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hs.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zk.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://og.jctech888.com.cn

================================================================================
来源：http://nt.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://ks.yuntaijiaju.cn

================================================================================
来源：http://xz.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://ke.panjiajie.cn

Py:   sys.argv[1:]
来源：http://zi.colortex.cn

PHP:  $argv;  $argc;
来源：http://oc.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://tf.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://id.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://gw.hnjuh.cn

Go:   os.Args[1:]
来源：http://fn.newstarts.cn

Ruby: ARGV
来源：http://yl.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://ro.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://si.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ci.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fm.bjjhwx.cn

JS:   process.env.HOME
来源：http://xk.newstarts.cn

TS:   process.env.HOME
来源：http://kf.szsharing.cn

Java: System.getenv("HOME")
来源：http://sf.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fa.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://qf.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uo.bookmarksfly.cn

[M03] 执行外部命令
来源：http://gt.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cw.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uv.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://te.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://js.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yc.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ok.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iv.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://ow.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://fj.nicolike.cn

Py:   os.getcwd()
来源：http://ek.shxzskj.cn

PHP:  getcwd();
来源：http://hj.jctech888.com.cn

JS:   process.cwd()
来源：http://jd.huixinmuqiang.cn

TS:   process.cwd()
来源：http://jg.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://jd.huanxung.cn

Go:   os.Getwd()
来源：http://ab.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://md.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jr.panjiajie.cn

[M05] 设置退出码
来源：http://lw.huanxung.cn

Py:   sys.exit(1)
来源：http://io.shxzskj.cn

PHP:  exit(1);
来源：http://oc.huanxung.cn

JS:   process.exit(1)
来源：http://jl.bjjhwx.cn

TS:   process.exit(1)
来源：http://yh.bookmarksfly.cn

Java: System.exit(1)
来源：http://ew.panjiajie.cn

Go:   os.Exit(1)
来源：http://ov.hnjuh.cn

Ruby: exit 1
来源：http://ce.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xa.yuexingan06.cn

[M06] 向标准错误输出
来源：http://fo.521024.cn

Py:   print("err", file=sys.stderr)
来源：http://za.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bg.bjjhwx.cn

JS:   console.error("err")
来源：http://kc.newstarts.cn

TS:   console.error("err")
来源：http://bg.haigaiapp.cn

Java: System.err.println("err")
来源：http://fw.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ji.szxytkj.cn

Ruby: warn "err"
来源：http://md.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://fr.lnxyls.cn

[M07] 判断是否为主入口
来源：http://fe.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://gd.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://af.asd995.cn

JS:   require.main === module
来源：http://jx.bookmarksfly.cn

TS:   require.main === module
来源：http://bw.nszjky.cn

Java: public static void main(String[] args)
来源：http://rx.newstarts.cn

Go:   func main()
来源：http://zk.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eb.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xd.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://ia.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://rm.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://rc.nicolike.cn

JS:   process.platform;  process.version
来源：http://co.shxzukj.cn

TS:   process.platform;  process.version
来源：http://nz.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wb.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rq.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wg.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://op.huixinmuqiang.cn

================================================================================
来源：http://no.szxytkj.cn

N. 数据结构与算法
来源：http://ng.lnxyls.cn

================================================================================
来源：http://le.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://kg.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xs.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://co.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ui.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vt.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jw.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://vn.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zp.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://de.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://rc.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://gw.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zi.huanxung.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://py.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ds.nszjky.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://om.huanxung.cn

Go:   slices.Sort(arr)
来源：http://sx.bookmarksfly.cn

Ruby: arr.sort
来源：http://kf.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pw.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://os.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nu.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://dx.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://in.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cd.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zi.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://at.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://og.huixiangedu.cn

[N04] 斐波那契数列
来源：http://me.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qv.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wo.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wx.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bw.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gx.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ql.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cu.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mv.nszjky.cn

[N05] 最大公约数
来源：http://ub.asd995.cn

Py:   math.gcd(a, b)
来源：http://lf.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://of.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rl.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ki.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://id.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rf.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://ab.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sw.shtwfgs.cn

[N06] 判断回文字符串
来源：http://ca.haigaiapp.cn

Py:   s == s[::-1]
来源：http://ny.asd995.cn

PHP:  $s === strrev($s);
来源：http://gm.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://nh.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://tb.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bf.asd995.cn

Go:   // 双指针从两端比较
来源：http://bx.shxzskj.cn

Ruby: s == s.reverse
来源：http://zm.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qs.panjiajie.cn

[N07] 两数之和（返回下标）
来源：http://jg.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://km.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vz.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tg.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://fw.wgjwhj.cn

Java: // 手写 HashMap
来源：http://ew.nszjky.cn

Go:   // 手写 map[int]int
来源：http://tj.9csxet.cn

Ruby: // 手写 Hash
来源：http://ao.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wx.panjiajie.cn

[N08] 生成全排列
来源：http://sv.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://kn.newstarts.cn

PHP:  // 手写递归交换
来源：http://ig.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://xk.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://vl.521024.cn

Java: // 手写回溯递归
来源：http://tw.shxzukj.cn

Go:   // 手写回溯递归
来源：http://bm.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://cz.521024.cn

C#:   // 手写回溯递归
来源：http://wm.wgjwhj.cn


<!-- 参考信息 -->