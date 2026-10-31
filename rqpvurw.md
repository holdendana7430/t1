代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ew.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bc.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://en.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://vv.muxihuayi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://li.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://pk.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hk.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rj.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://ru.shxzukj.cn

Py:   json.loads(s)
来源：http://aw.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pi.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ua.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://cm.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ot.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://qv.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://oj.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bu.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://mq.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dg.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rz.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kl.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xh.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://de.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ha.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wd.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hr.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://tl.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wz.9csxet.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kb.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vr.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yn.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rh.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ve.haigaiapp.cn

[K05] 深拷贝对象
来源：http://ox.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://ml.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://ck.szxytkj.cn

JS:   structuredClone(obj)
来源：http://rw.9csxet.cn

TS:   structuredClone(obj)
来源：http://ab.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xr.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kn.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://au.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tk.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://cd.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zo.szsharing.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mr.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kn.jianghongdianzi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xv.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sl.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cf.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wm.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oe.jctech888.com.cn

[K07] 进制转换
来源：http://ik.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iq.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uj.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xg.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zx.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qq.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xb.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ky.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dd.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://gw.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://dy.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ll.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://fx.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://mg.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qd.newstarts.cn

Go:   encoding/gob
来源：http://tx.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://tg.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vg.szxytkj.cn

================================================================================
来源：http://hr.521024.cn

L. 网络请求
来源：http://fw.bjjhwx.cn

================================================================================
来源：http://kc.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://do.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dc.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fi.shxzskj.cn

JS:   await fetch(url)
来源：http://lr.yuexingan06.cn

TS:   await fetch(url)
来源：http://lr.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://as.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://bo.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dx.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cf.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ff.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xt.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://or.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://er.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fh.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tp.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yn.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ra.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qx.nszjky.cn

[L03] 设置自定义请求头
来源：http://si.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yt.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gf.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wh.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ip.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kx.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ss.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hn.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fa.huixinmuqiang.cn

[L04] 设置超时
来源：http://rl.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://zt.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tw.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eb.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rd.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fb.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://te.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nj.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://og.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://yz.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jh.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nw.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://am.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dl.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ok.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fn.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hh.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sd.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://zg.panjiajie.cn

Py:   resp.json()
来源：http://rj.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://pb.shxzukj.cn

JS:   await resp.json()
来源：http://rg.colortex.cn

TS:   await resp.json()
来源：http://dg.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gm.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xa.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://uw.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ym.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://dv.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ty.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vg.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://ft.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://eq.lnxyls.cn

Java: resp.statusCode()
来源：http://pq.szxytkj.cn

Go:   resp.StatusCode
来源：http://bn.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://rl.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://kk.colortex.cn

[L08] 并发请求多个地址
来源：http://nh.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xf.lnxyls.cn

PHP:  curl_multi_init() 系列
来源：http://xj.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fu.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ax.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tw.yuntaijiaju.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gz.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sd.nszjky.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eo.huixinmuqiang.cn

================================================================================
来源：http://hz.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://nb.yuntaijiaju.cn

================================================================================
来源：http://ue.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ma.szxytkj.cn

Py:   sys.argv[1:]
来源：http://wp.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://su.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://la.hahajie.cn

TS:   process.argv.slice(2)
来源：http://jz.colortex.cn

Java: args 数组（main 方法参数）
来源：http://ip.colortex.cn

Go:   os.Args[1:]
来源：http://wu.yuntaijiaju.cn

Ruby: ARGV
来源：http://nv.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://qt.huixiangedu.cn

[M02] 读取环境变量
来源：http://qu.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://vg.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ol.lnxyls.cn

JS:   process.env.HOME
来源：http://fs.nszjky.cn

TS:   process.env.HOME
来源：http://mv.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://uk.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ci.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://gu.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mf.huixiangedu.cn

[M03] 执行外部命令
来源：http://bl.shxzskj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kx.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ng.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aq.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uy.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yf.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ff.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dv.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://cv.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://ar.chemitech.net.cn

Py:   os.getcwd()
来源：http://ra.shxzskj.cn

PHP:  getcwd();
来源：http://bu.huixiangedu.cn

JS:   process.cwd()
来源：http://rf.hnjuh.cn

TS:   process.cwd()
来源：http://pk.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://or.yuexingan06.cn

Go:   os.Getwd()
来源：http://qx.shtwfgs.cn

Ruby: Dir.pwd
来源：http://qs.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yc.shxzskj.cn

[M05] 设置退出码
来源：http://at.shtwfgs.cn

Py:   sys.exit(1)
来源：http://yw.yuexingan06.cn

PHP:  exit(1);
来源：http://dz.muxihuayi.cn

JS:   process.exit(1)
来源：http://rx.chemitech.net.cn

TS:   process.exit(1)
来源：http://hk.muxihuayi.cn

Java: System.exit(1)
来源：http://jo.huixiangedu.cn

Go:   os.Exit(1)
来源：http://lb.asd995.cn

Ruby: exit 1
来源：http://mn.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yc.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ez.chemitech.net.cn

Py:   print("err", file=sys.stderr)
来源：http://fh.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gc.gzmigu.cn

JS:   console.error("err")
来源：http://tm.jctech888.com.cn

TS:   console.error("err")
来源：http://nr.haigaiapp.cn

Java: System.err.println("err")
来源：http://am.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tu.huanxung.cn

Ruby: warn "err"
来源：http://sm.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://pn.lnxyls.cn

[M07] 判断是否为主入口
来源：http://sg.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://cm.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ai.colortex.cn

JS:   require.main === module
来源：http://oa.jianghongdianzi.cn

TS:   require.main === module
来源：http://ns.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://cb.shtwfgs.cn

Go:   func main()
来源：http://ts.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wk.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://dh.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://hq.lnxyls.cn

Py:   platform.system();  platform.python_version()
来源：http://hf.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://fo.gzmigu.cn

JS:   process.platform;  process.version
来源：http://cw.szsharing.cn

TS:   process.platform;  process.version
来源：http://nv.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ic.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mw.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lq.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://he.jianghongdianzi.cn

================================================================================
来源：http://ng.hnjuh.cn

N. 数据结构与算法
来源：http://wd.panjiajie.cn

================================================================================
来源：http://ji.haigaiapp.cn

[N01] 二分查找（有序数组）
来源：http://mx.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hm.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://db.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zf.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://za.yuntaijiaju.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hl.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://pk.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xs.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nz.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://mc.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://yr.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://li.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vu.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://in.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gr.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://pp.wgjwhj.cn

Ruby: arr.sort
来源：http://vv.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fa.shxzukj.cn

[N03] 快速排序（分治示例）
来源：http://gs.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cg.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://gl.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ab.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kq.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zu.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ls.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ff.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rk.huixiangedu.cn

[N04] 斐波那契数列
来源：http://hr.szxytkj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fo.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hn.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ob.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ae.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wk.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://af.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pd.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uf.9csxet.cn

[N05] 最大公约数
来源：http://di.nszjky.cn

Py:   math.gcd(a, b)
来源：http://jw.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aa.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fp.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cx.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xs.lnxyls.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fu.asd995.cn

Ruby: a.gcd(b)
来源：http://ba.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mh.lnxyls.cn

[N06] 判断回文字符串
来源：http://aw.9csxet.cn

Py:   s == s[::-1]
来源：http://mu.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://ou.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://sp.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://wz.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qs.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://tz.hahajie.cn

Ruby: s == s.reverse
来源：http://sz.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fg.colortex.cn

[N07] 两数之和（返回下标）
来源：http://rv.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qs.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tb.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lm.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://fl.asd995.cn

Java: // 手写 HashMap
来源：http://jr.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://gs.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://qx.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://if.shxzukj.cn

[N08] 生成全排列
来源：http://aq.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://tk.9csxet.cn

PHP:  // 手写递归交换
来源：http://pm.shxzukj.cn

JS:   // 手写回溯递归
来源：http://dg.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://tx.shtwfgs.cn

Java: // 手写回溯递归
来源：http://zu.szxytkj.cn

Go:   // 手写回溯递归
来源：http://fu.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://qj.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://gb.shxzskj.cn

[N09] 栈与队列
来源：http://gc.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qv.yuexingan06.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://il.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dh.nicolike.cn


<!-- 参考信息 -->