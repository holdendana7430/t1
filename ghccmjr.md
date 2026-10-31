代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cn.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pk.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://cc.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://ab.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mg.nicolike.cn

Go:   json.Marshal(obj)
来源：http://ab.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yo.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fh.newstarts.cn

[K02] JSON 字符串转对象
来源：http://gj.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://ln.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ai.asd995.cn

JS:   JSON.parse(s)
来源：http://gs.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://zv.9csxet.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hw.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://ny.hnjuh.cn

Ruby: JSON.parse(s)
来源：http://wz.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jk.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://il.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lj.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ly.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dx.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qa.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ic.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ye.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://im.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xm.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://oo.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kj.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wg.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ox.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vu.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ae.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nm.shxzskj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wf.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pl.lnxyls.cn

[K05] 深拷贝对象
来源：http://mb.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://mx.huanxung.cn

PHP:  unserialize(serialize($obj));
来源：http://ax.szxytkj.cn

JS:   structuredClone(obj)
来源：http://mf.szsharing.cn

TS:   structuredClone(obj)
来源：http://gu.gzmigu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://st.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ro.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://he.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gr.521024.cn

[K06] 解析 URL 查询串
来源：http://md.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://us.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kg.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vz.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tx.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ph.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://co.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vz.bookmarksfly.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oj.bjjhwx.cn

[K07] 进制转换
来源：http://wz.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wf.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pa.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://of.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pd.lnxyls.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ga.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fz.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jc.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oj.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://qf.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://kx.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wx.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://nn.huanxung.cn

TS:   v8.serialize(obj)        // Node
来源：http://rf.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vg.wgjwhj.cn

Go:   encoding/gob
来源：http://ol.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://pv.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ip.huanxung.cn

================================================================================
来源：http://eg.panjiajie.cn

L. 网络请求
来源：http://is.jianghongdianzi.cn

================================================================================
来源：http://ji.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ld.shxzskj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tz.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ro.colortex.cn

JS:   await fetch(url)
来源：http://cc.shxzskj.cn

TS:   await fetch(url)
来源：http://au.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jn.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://cl.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bx.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xn.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://vy.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://su.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uo.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ps.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ai.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nv.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hv.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sj.colortex.cn

[L03] 设置自定义请求头
来源：http://io.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kk.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wo.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sk.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sa.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kn.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kd.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sw.9csxet.cn

[L04] 设置超时
来源：http://sp.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://rk.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://of.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cz.haigaiapp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://se.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://px.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eu.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rd.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://si.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://wi.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xy.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://du.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gg.jctech888.com.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kr.bjjhwx.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wo.bjjhwx.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sa.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ij.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://xz.bjjhwx.cn

Py:   resp.json()
来源：http://ow.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://xm.nicolike.cn

JS:   await resp.json()
来源：http://zu.newstarts.cn

TS:   await resp.json()
来源：http://kn.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ow.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://re.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://bq.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ay.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://xc.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hu.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cn.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://yg.colortex.cn

TS:   resp.ok;  resp.status
来源：http://az.muxihuayi.cn

Java: resp.statusCode()
来源：http://pg.haigaiapp.cn

Go:   resp.StatusCode
来源：http://nl.nicolike.cn

Ruby: resp.code.to_i
来源：http://kn.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://df.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://jz.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kn.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://jn.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dd.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://be.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jd.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cl.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jm.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zu.szxytkj.cn

================================================================================
来源：http://cq.panjiajie.cn

M. 命令行 / 进程 / 环境
来源：http://ve.lnxyls.cn

================================================================================
来源：http://jw.9csxet.cn

[M01] 读取命令行参数
来源：http://sr.panjiajie.cn

Py:   sys.argv[1:]
来源：http://km.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://mc.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://iw.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://ux.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://yf.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ta.nszjky.cn

Ruby: ARGV
来源：http://dg.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://fz.shxzskj.cn

[M02] 读取环境变量
来源：http://jq.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://hw.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ef.521024.cn

JS:   process.env.HOME
来源：http://kh.shtwfgs.cn

TS:   process.env.HOME
来源：http://hj.hnjuh.cn

Java: System.getenv("HOME")
来源：http://wp.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://io.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://xp.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kw.lnxyls.cn

[M03] 执行外部命令
来源：http://ks.9csxet.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pb.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yj.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zf.muxihuayi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ck.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hd.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rz.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qs.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://zk.panjiajie.cn

[M04] 获取当前工作目录
来源：http://iw.chemitech.net.cn

Py:   os.getcwd()
来源：http://vg.huixinmuqiang.cn

PHP:  getcwd();
来源：http://yd.huixiangedu.cn

JS:   process.cwd()
来源：http://ot.lnxyls.cn

TS:   process.cwd()
来源：http://fj.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://wg.shxzukj.cn

Go:   os.Getwd()
来源：http://wu.wgjwhj.cn

Ruby: Dir.pwd
来源：http://fk.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ss.bjjhwx.cn

[M05] 设置退出码
来源：http://mi.gzmigu.cn

Py:   sys.exit(1)
来源：http://mf.jctech888.com.cn

PHP:  exit(1);
来源：http://gp.nicolike.cn

JS:   process.exit(1)
来源：http://gi.haigaiapp.cn

TS:   process.exit(1)
来源：http://uj.szxytkj.cn

Java: System.exit(1)
来源：http://bf.asd995.cn

Go:   os.Exit(1)
来源：http://wq.yuntaijiaju.cn

Ruby: exit 1
来源：http://cz.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fw.shtwfgs.cn

[M06] 向标准错误输出
来源：http://mk.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://hg.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ru.asd995.cn

JS:   console.error("err")
来源：http://ds.yuntaijiaju.cn

TS:   console.error("err")
来源：http://yb.huixiangedu.cn

Java: System.err.println("err")
来源：http://tv.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nk.yuexingan06.cn

Ruby: warn "err"
来源：http://vs.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://yq.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://fr.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://ay.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sp.chemitech.net.cn

JS:   require.main === module
来源：http://je.asd995.cn

TS:   require.main === module
来源：http://za.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://yg.shxzukj.cn

Go:   func main()
来源：http://qr.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xp.colortex.cn

C#:   static void Main(string[] args)
来源：http://tj.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://dh.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://ip.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://su.newstarts.cn

JS:   process.platform;  process.version
来源：http://ee.gzmigu.cn

TS:   process.platform;  process.version
来源：http://iz.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pa.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xu.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ho.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tt.muxihuayi.cn

================================================================================
来源：http://rv.nicolike.cn

N. 数据结构与算法
来源：http://vs.jctech888.com.cn

================================================================================
来源：http://bj.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://dq.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wm.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pv.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vs.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lv.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ru.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://yy.huixinmuqiang.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yy.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fs.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://vo.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://vi.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ou.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mv.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://op.yuexingan06.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eq.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://wl.szsharing.cn

Ruby: arr.sort
来源：http://og.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oz.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://zq.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gj.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://tn.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ln.chemitech.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ih.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zq.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vg.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://it.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vz.asd995.cn

[N04] 斐波那契数列
来源：http://jv.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ey.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zp.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ww.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ng.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://np.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wn.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://us.hahajie.cn

[N05] 最大公约数
来源：http://zo.nicolike.cn

Py:   math.gcd(a, b)
来源：http://xu.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xi.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qw.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oe.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rh.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uu.asd995.cn

Ruby: a.gcd(b)
来源：http://ah.chemitech.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vz.jctech888.com.cn

[N06] 判断回文字符串
来源：http://qv.bjjhwx.cn

Py:   s == s[::-1]
来源：http://hw.szsharing.cn

PHP:  $s === strrev($s);
来源：http://ee.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://lq.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://jd.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xw.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://jx.shxzukj.cn

Ruby: s == s.reverse
来源：http://fk.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://av.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ul.9csxet.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aa.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jg.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hp.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://ni.hahajie.cn

Java: // 手写 HashMap
来源：http://tu.asd995.cn

Go:   // 手写 map[int]int
来源：http://br.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://ys.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sf.muxihuayi.cn

[N08] 生成全排列
来源：http://yx.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://lj.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://vo.lnxyls.cn

JS:   // 手写回溯递归
来源：http://nk.szsharing.cn

TS:   // 手写回溯递归
来源：http://bw.szsharing.cn

Java: // 手写回溯递归
来源：http://yp.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://du.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://tf.colortex.cn

C#:   // 手写回溯递归
来源：http://ig.bjjhwx.cn

[N09] 栈与队列
来源：http://ih.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tw.nszjky.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pl.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oc.huanxung.cn


<!-- 参考信息 -->