代发 wailian999

================================================================================
来源：http://iv.521024.cn

K. JSON 与序列化
来源：http://kr.hnjuh.cn

================================================================================
来源：http://ai.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://nk.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rw.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tc.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://qf.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://dn.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jn.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://rr.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ke.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vb.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://jy.huixinmuqiang.cn

Py:   json.loads(s)
来源：http://zi.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://th.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://as.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://mi.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rt.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://dk.colortex.cn

Ruby: JSON.parse(s)
来源：http://xc.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vt.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://jc.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://de.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pf.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://or.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bj.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lu.521024.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zz.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bb.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fy.nszjky.cn

[K04] 读取 JSON 文件
来源：http://iv.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zn.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ct.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tr.nicolike.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vs.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://er.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vc.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mo.hahajie.cn

[K05] 深拷贝对象
来源：http://gp.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://od.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://vz.szxytkj.cn

JS:   structuredClone(obj)
来源：http://gb.9csxet.cn

TS:   structuredClone(obj)
来源：http://mi.lnxyls.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ol.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ly.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vc.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://im.521024.cn

[K06] 解析 URL 查询串
来源：http://yg.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vj.9csxet.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ve.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vh.gzmigu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zf.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hw.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cr.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bm.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gj.nicolike.cn

[K07] 进制转换
来源：http://rc.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gv.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ij.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://so.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iv.hahajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ft.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nr.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://of.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://on.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://gq.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://rt.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dx.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://vt.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://vw.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zz.szsharing.cn

Go:   encoding/gob
来源：http://kt.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ls.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ae.bjjhwx.cn

================================================================================
来源：http://qe.huanxung.cn

L. 网络请求
来源：http://ni.nszjky.cn

================================================================================
来源：http://qw.hnjuh.cn

[L01] 发送 GET 请求
来源：http://up.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://af.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://he.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://qd.asd995.cn

TS:   await fetch(url)
来源：http://be.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gj.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://ka.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ck.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hv.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://nr.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://we.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eb.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://no.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lb.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tu.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fo.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eq.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zk.huanxung.cn

[L03] 设置自定义请求头
来源：http://cg.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wh.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sz.panjiajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kx.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://us.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aq.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ng.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zh.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pm.huixiangedu.cn

[L04] 设置超时
来源：http://gi.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://qt.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wn.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://su.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wq.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lj.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fi.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fv.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kr.9csxet.cn

[L05] 上传文件（multipart）
来源：http://qr.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://um.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://si.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oz.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bn.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://th.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iq.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zs.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://si.jctech888.com.cn

Py:   resp.json()
来源：http://nc.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ih.muxihuayi.cn

JS:   await resp.json()
来源：http://me.huanxung.cn

TS:   await resp.json()
来源：http://yk.wgjwhj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://px.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ys.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://vg.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cs.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://fv.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ay.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wa.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://ar.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://er.yuexingan06.cn

Java: resp.statusCode()
来源：http://ac.szsharing.cn

Go:   resp.StatusCode
来源：http://tc.nicolike.cn

Ruby: resp.code.to_i
来源：http://jy.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://kh.newstarts.cn

[L08] 并发请求多个地址
来源：http://ac.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://on.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://xl.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.huixinmuqiang.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ao.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ta.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qm.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qg.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vb.bookmarksfly.cn

================================================================================
来源：http://iw.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://io.gzmigu.cn

================================================================================
来源：http://vq.asd995.cn

[M01] 读取命令行参数
来源：http://us.521024.cn

Py:   sys.argv[1:]
来源：http://ot.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://xu.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://pf.szsharing.cn

TS:   process.argv.slice(2)
来源：http://bc.bjjhwx.cn

Java: args 数组（main 方法参数）
来源：http://wh.9csxet.cn

Go:   os.Args[1:]
来源：http://sa.yuexingan06.cn

Ruby: ARGV
来源：http://md.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://iu.hahajie.cn

[M02] 读取环境变量
来源：http://py.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ek.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dc.521024.cn

JS:   process.env.HOME
来源：http://hk.shxzukj.cn

TS:   process.env.HOME
来源：http://bp.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://se.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://am.newstarts.cn

Ruby: ENV["HOME"]
来源：http://xx.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dz.newstarts.cn

[M03] 执行外部命令
来源：http://de.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vn.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qr.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cn.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xf.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fo.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ft.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pl.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://ts.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://is.jctech888.com.cn

Py:   os.getcwd()
来源：http://zt.huanxung.cn

PHP:  getcwd();
来源：http://sp.521024.cn

JS:   process.cwd()
来源：http://zk.yuntaijiaju.cn

TS:   process.cwd()
来源：http://uz.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://mb.szsharing.cn

Go:   os.Getwd()
来源：http://eg.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://gd.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lx.asd995.cn

[M05] 设置退出码
来源：http://nt.gzmigu.cn

Py:   sys.exit(1)
来源：http://xj.yuntaijiaju.cn

PHP:  exit(1);
来源：http://ly.bookmarksfly.cn

JS:   process.exit(1)
来源：http://aj.shtwfgs.cn

TS:   process.exit(1)
来源：http://at.9csxet.cn

Java: System.exit(1)
来源：http://zk.nicolike.cn

Go:   os.Exit(1)
来源：http://rq.yuntaijiaju.cn

Ruby: exit 1
来源：http://xf.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bc.jctech888.com.cn

[M06] 向标准错误输出
来源：http://bb.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ok.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jx.bookmarksfly.cn

JS:   console.error("err")
来源：http://kw.bjjhwx.cn

TS:   console.error("err")
来源：http://vo.asd995.cn

Java: System.err.println("err")
来源：http://er.hnjuh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iw.newstarts.cn

Ruby: warn "err"
来源：http://em.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://fm.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://ek.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://un.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qf.shxzukj.cn

JS:   require.main === module
来源：http://mw.haigaiapp.cn

TS:   require.main === module
来源：http://dc.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://ca.asd995.cn

Go:   func main()
来源：http://js.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://na.hnjuh.cn

C#:   static void Main(string[] args)
来源：http://en.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://hg.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://fn.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://jz.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://xh.colortex.cn

TS:   process.platform;  process.version
来源：http://jw.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://be.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xt.huanxung.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fl.bookmarksfly.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rg.yuntaijiaju.cn

================================================================================
来源：http://kf.9csxet.cn

N. 数据结构与算法
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://kz.asd995.cn

[N01] 二分查找（有序数组）
来源：http://ud.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ty.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://au.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gj.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qr.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mk.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://ng.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fv.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vz.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://wv.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://in.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nv.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mu.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vb.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://en.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://fv.hnjuh.cn

Ruby: arr.sort
来源：http://bn.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gc.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://br.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zu.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://vs.nszjky.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sr.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eg.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dy.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xm.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sg.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nd.yuexingan06.cn

[N04] 斐波那契数列
来源：http://cm.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fn.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ws.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://it.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jm.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qk.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cu.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eb.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wr.panjiajie.cn

[N05] 最大公约数
来源：http://uh.521024.cn

Py:   math.gcd(a, b)
来源：http://ra.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dn.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kn.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ns.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jd.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pc.9csxet.cn

Ruby: a.gcd(b)
来源：http://aa.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bl.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://cm.521024.cn

Py:   s == s[::-1]
来源：http://se.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://kj.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://ks.521024.cn

TS:   s === [...s].reverse().join("")
来源：http://ri.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lk.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://pl.lnxyls.cn

Ruby: s == s.reverse
来源：http://rs.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ww.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://sl.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iq.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ap.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dd.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://qs.nicolike.cn

Java: // 手写 HashMap
来源：http://rf.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://ma.lnxyls.cn

Ruby: // 手写 Hash
来源：http://ne.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gt.huanxung.cn

[N08] 生成全排列
来源：http://sd.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://pd.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://sg.lnxyls.cn

JS:   // 手写回溯递归
来源：http://bg.huanxung.cn

TS:   // 手写回溯递归
来源：http://fi.hnjuh.cn

Java: // 手写回溯递归
来源：http://ds.panjiajie.cn

Go:   // 手写回溯递归
来源：http://wc.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://ny.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://zu.bookmarksfly.cn


<!-- 参考信息 -->