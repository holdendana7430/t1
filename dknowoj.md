代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cs.hahajie.cn

Go:   json.Marshal(obj)
来源：http://jw.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://io.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ne.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://lo.hnjuh.cn

Py:   json.loads(s)
来源：http://lv.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mj.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://lt.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://wp.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hv.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://dn.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://jz.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cc.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://nj.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wb.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zr.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wk.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yo.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://we.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gw.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hg.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nr.bjjhwx.cn

[K04] 读取 JSON 文件
来源：http://dy.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zc.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sr.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ak.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xe.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yr.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yb.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qu.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ve.huanxung.cn

[K05] 深拷贝对象
来源：http://vt.521024.cn

Py:   copy.deepcopy(obj)
来源：http://lm.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://ts.wgjwhj.cn

JS:   structuredClone(obj)
来源：http://ls.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://cv.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uj.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qx.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ml.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wm.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://wu.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zq.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zm.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mn.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zp.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://az.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yd.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sx.nicolike.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qd.chemitech.net.cn

[K07] 进制转换
来源：http://km.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mw.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yg.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ed.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ws.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ii.shxzukj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qe.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fx.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ju.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qk.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://of.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bz.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://qi.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://vo.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vy.shtwfgs.cn

Go:   encoding/gob
来源：http://kc.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://pu.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ry.521024.cn

================================================================================
来源：http://jq.jianghongdianzi.cn

L. 网络请求
来源：http://ly.huixinmuqiang.cn

================================================================================
来源：http://sk.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://lv.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ui.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nicolike.cn

JS:   await fetch(url)
来源：http://um.lnxyls.cn

TS:   await fetch(url)
来源：http://wb.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cq.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://ca.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hy.nicolike.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vr.gzmigu.cn

[L02] 发送 POST JSON
来源：http://fe.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uc.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ez.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wl.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jm.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://db.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rm.jianghongdianzi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oz.nszjky.cn

[L03] 设置自定义请求头
来源：http://sm.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://em.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pn.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://us.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kr.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mt.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sc.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dl.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tk.newstarts.cn

[L04] 设置超时
来源：http://po.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://sb.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://by.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lj.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dd.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hv.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fb.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ub.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zs.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://it.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ii.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eu.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ly.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gi.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zi.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kq.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ie.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nf.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://od.huixiangedu.cn

Py:   resp.json()
来源：http://tk.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://gw.jianghongdianzi.cn

JS:   await resp.json()
来源：http://dz.shtwfgs.cn

TS:   await resp.json()
来源：http://ul.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vq.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dp.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://gq.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xo.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://vx.yuexingan06.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://se.yuntaijiaju.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ow.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://jy.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://ae.9csxet.cn

Java: resp.statusCode()
来源：http://hf.chemitech.net.cn

Go:   resp.StatusCode
来源：http://nm.hahajie.cn

Ruby: resp.code.to_i
来源：http://gl.asd995.cn

C#:   (int)resp.StatusCode
来源：http://ph.hnjuh.cn

[L08] 并发请求多个地址
来源：http://gz.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ip.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://ui.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bi.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mz.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uu.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ui.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jr.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sq.bjjhwx.cn

================================================================================
来源：http://xp.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://nr.huixiangedu.cn

================================================================================
来源：http://wi.shxzskj.cn

[M01] 读取命令行参数
来源：http://aj.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://oe.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://gv.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://gp.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://kd.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://uz.panjiajie.cn

Go:   os.Args[1:]
来源：http://mu.nicolike.cn

Ruby: ARGV
来源：http://ms.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://pp.hahajie.cn

[M02] 读取环境变量
来源：http://zo.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://cc.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wj.nicolike.cn

JS:   process.env.HOME
来源：http://ye.huixiangedu.cn

TS:   process.env.HOME
来源：http://rb.asd995.cn

Java: System.getenv("HOME")
来源：http://mm.hnjuh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hm.nicolike.cn

Ruby: ENV["HOME"]
来源：http://nl.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hb.szxytkj.cn

[M03] 执行外部命令
来源：http://lm.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ql.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ry.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gk.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gm.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ld.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gb.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sd.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://iv.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://nd.9csxet.cn

Py:   os.getcwd()
来源：http://rc.nicolike.cn

PHP:  getcwd();
来源：http://qm.shtwfgs.cn

JS:   process.cwd()
来源：http://ey.shxzukj.cn

TS:   process.cwd()
来源：http://le.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://uu.szxytkj.cn

Go:   os.Getwd()
来源：http://jv.jctech888.com.cn

Ruby: Dir.pwd
来源：http://lc.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ie.wgjwhj.cn

[M05] 设置退出码
来源：http://wt.9csxet.cn

Py:   sys.exit(1)
来源：http://oo.huixinmuqiang.cn

PHP:  exit(1);
来源：http://eo.hahajie.cn

JS:   process.exit(1)
来源：http://da.panjiajie.cn

TS:   process.exit(1)
来源：http://lo.jctech888.com.cn

Java: System.exit(1)
来源：http://tz.huanxung.cn

Go:   os.Exit(1)
来源：http://hd.panjiajie.cn

Ruby: exit 1
来源：http://bd.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ae.huanxung.cn

[M06] 向标准错误输出
来源：http://um.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://zp.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ba.chemitech.net.cn

JS:   console.error("err")
来源：http://ld.hnjuh.cn

TS:   console.error("err")
来源：http://ha.nszjky.cn

Java: System.err.println("err")
来源：http://ed.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ol.jctech888.com.cn

Ruby: warn "err"
来源：http://lj.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://dr.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://og.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://tn.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mk.jctech888.com.cn

JS:   require.main === module
来源：http://jt.hnjuh.cn

TS:   require.main === module
来源：http://ei.lnxyls.cn

Java: public static void main(String[] args)
来源：http://vr.szsharing.cn

Go:   func main()
来源：http://pl.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zz.nszjky.cn

C#:   static void Main(string[] args)
来源：http://jc.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://qs.hahajie.cn

Py:   platform.system();  platform.python_version()
来源：http://bt.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mt.nicolike.cn

JS:   process.platform;  process.version
来源：http://xs.shxzukj.cn

TS:   process.platform;  process.version
来源：http://fk.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ce.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dl.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tn.lnxyls.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fy.bjjhwx.cn

================================================================================
来源：http://ja.wgjwhj.cn

N. 数据结构与算法
来源：http://zn.jianghongdianzi.cn

================================================================================
来源：http://nd.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://dc.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mb.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wh.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://db.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dl.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aw.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://mh.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yi.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oj.asd995.cn

[N02] 排序（工程实践用内置实现）
来源：http://ue.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://yg.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ha.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wv.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kx.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lf.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://dn.jianghongdianzi.cn

Ruby: arr.sort
来源：http://kj.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qs.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://jm.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://br.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://qq.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oj.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ve.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fr.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zw.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mt.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://di.jctech888.com.cn

[N04] 斐波那契数列
来源：http://zf.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dg.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jj.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ri.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yd.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ha.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ib.hnjuh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zg.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rp.hahajie.cn

[N05] 最大公约数
来源：http://jp.huanxung.cn

Py:   math.gcd(a, b)
来源：http://jw.hahajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://me.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fe.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rw.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aw.shxzukj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sj.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://tp.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wu.wgjwhj.cn

[N06] 判断回文字符串
来源：http://ih.hnjuh.cn

Py:   s == s[::-1]
来源：http://kc.nszjky.cn

PHP:  $s === strrev($s);
来源：http://nq.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://tx.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://wj.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://li.colortex.cn

Go:   // 双指针从两端比较
来源：http://uv.shxzskj.cn

Ruby: s == s.reverse
来源：http://ve.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vp.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://gp.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://go.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://df.nszjky.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gs.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://wc.asd995.cn

Java: // 手写 HashMap
来源：http://ks.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://bz.panjiajie.cn

Ruby: // 手写 Hash
来源：http://ew.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mm.newstarts.cn

[N08] 生成全排列
来源：http://gu.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://bq.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://ho.shxzskj.cn

JS:   // 手写回溯递归
来源：http://zz.nszjky.cn

TS:   // 手写回溯递归
来源：http://sf.huixiangedu.cn

Java: // 手写回溯递归
来源：http://ot.lnxyls.cn

Go:   // 手写回溯递归
来源：http://rn.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://uz.szsharing.cn

C#:   // 手写回溯递归
来源：http://io.panjiajie.cn

[N09] 栈与队列
来源：http://fx.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://df.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cr.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://op.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pb.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ma.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xa.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ms.asd995.cn


<!-- 参考信息 -->