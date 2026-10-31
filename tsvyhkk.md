代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tg.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vo.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://oz.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://fb.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bd.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://ix.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.nicolike.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kd.yuntaijiaju.cn

[K02] JSON 字符串转对象
来源：http://wy.shxzukj.cn

Py:   json.loads(s)
来源：http://jf.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ye.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://bf.521024.cn

TS:   JSON.parse(s)
来源：http://iv.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ud.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://eh.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://mv.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mw.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://uj.shtwfgs.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qx.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://my.bjjhwx.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ng.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zr.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sg.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ku.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lk.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ae.hahajie.cn

[K04] 读取 JSON 文件
来源：http://hx.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tt.muxihuayi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://st.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sx.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cc.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ki.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jo.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dz.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aa.lnxyls.cn

[K05] 深拷贝对象
来源：http://do.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://ax.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://sh.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ng.szsharing.cn

TS:   structuredClone(obj)
来源：http://ag.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rp.huanxung.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://do.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vu.haigaiapp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://it.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://yj.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://st.asd995.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kr.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xo.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zs.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wb.shxzskj.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xf.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xa.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://en.huanxung.cn

[K07] 进制转换
来源：http://gh.huixiangedu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hi.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ww.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gm.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ve.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yt.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cy.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rk.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gx.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ep.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ux.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://lh.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://bo.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vd.panjiajie.cn

Go:   encoding/gob
来源：http://lp.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://xm.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://se.shxzskj.cn

================================================================================
来源：http://yc.bookmarksfly.cn

L. 网络请求
来源：http://tg.szxytkj.cn

================================================================================
来源：http://gg.9csxet.cn

[L01] 发送 GET 请求
来源：http://jp.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aq.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://do.shxzskj.cn

JS:   await fetch(url)
来源：http://ka.bookmarksfly.cn

TS:   await fetch(url)
来源：http://sb.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ka.shxzskj.cn

Go:   resp, err := http.Get(url)
来源：http://ae.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pj.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xg.nszjky.cn

[L02] 发送 POST JSON
来源：http://zi.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ci.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ws.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yd.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ls.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://td.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bx.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jf.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nm.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ar.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wg.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://id.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xs.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kw.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ga.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pa.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hl.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zf.szxytkj.cn

[L04] 设置超时
来源：http://pv.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://sm.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://py.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://te.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://an.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yc.yuexingan06.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fx.yuntaijiaju.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ik.nszjky.cn

[L05] 上传文件（multipart）
来源：http://vr.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pv.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://or.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ve.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://py.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gf.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ok.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ek.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pl.colortex.cn

[L06] 解析响应为 JSON
来源：http://ro.huixiangedu.cn

Py:   resp.json()
来源：http://es.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://lk.chemitech.net.cn

JS:   await resp.json()
来源：http://te.nszjky.cn

TS:   await resp.json()
来源：http://mg.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ic.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ih.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ln.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gt.521024.cn

[L07] 处理 HTTP 状态码
来源：http://yz.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xf.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ug.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://lt.asd995.cn

TS:   resp.ok;  resp.status
来源：http://oi.asd995.cn

Java: resp.statusCode()
来源：http://mm.shxzskj.cn

Go:   resp.StatusCode
来源：http://bt.newstarts.cn

Ruby: resp.code.to_i
来源：http://gl.asd995.cn

C#:   (int)resp.StatusCode
来源：http://pb.szsharing.cn

[L08] 并发请求多个地址
来源：http://pg.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mq.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://kb.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sm.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nq.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mw.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ki.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xf.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qn.hnjuh.cn

================================================================================
来源：http://ij.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://ew.huixiangedu.cn

================================================================================
来源：http://on.huanxung.cn

[M01] 读取命令行参数
来源：http://ie.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://uj.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://no.521024.cn

JS:   process.argv.slice(2)
来源：http://gb.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://pn.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://bo.chemitech.net.cn

Go:   os.Args[1:]
来源：http://la.521024.cn

Ruby: ARGV
来源：http://xl.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://ft.hnjuh.cn

[M02] 读取环境变量
来源：http://kk.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://md.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fx.jctech888.com.cn

JS:   process.env.HOME
来源：http://eq.bookmarksfly.cn

TS:   process.env.HOME
来源：http://xx.hahajie.cn

Java: System.getenv("HOME")
来源：http://xy.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ha.colortex.cn

Ruby: ENV["HOME"]
来源：http://cp.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://em.jctech888.com.cn

[M03] 执行外部命令
来源：http://qj.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eu.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ci.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vg.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gx.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qq.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xu.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mq.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://yp.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://pz.hnjuh.cn

Py:   os.getcwd()
来源：http://ae.muxihuayi.cn

PHP:  getcwd();
来源：http://bc.jctech888.com.cn

JS:   process.cwd()
来源：http://jx.9csxet.cn

TS:   process.cwd()
来源：http://jy.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://ok.huixiangedu.cn

Go:   os.Getwd()
来源：http://yk.muxihuayi.cn

Ruby: Dir.pwd
来源：http://wh.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yb.huixinmuqiang.cn

[M05] 设置退出码
来源：http://lq.hahajie.cn

Py:   sys.exit(1)
来源：http://lp.jctech888.com.cn

PHP:  exit(1);
来源：http://gn.panjiajie.cn

JS:   process.exit(1)
来源：http://gi.nicolike.cn

TS:   process.exit(1)
来源：http://bq.521024.cn

Java: System.exit(1)
来源：http://pe.haigaiapp.cn

Go:   os.Exit(1)
来源：http://hf.chemitech.net.cn

Ruby: exit 1
来源：http://zn.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qk.chemitech.net.cn

[M06] 向标准错误输出
来源：http://qp.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://op.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xx.colortex.cn

JS:   console.error("err")
来源：http://yx.asd995.cn

TS:   console.error("err")
来源：http://ox.bookmarksfly.cn

Java: System.err.println("err")
来源：http://mx.nicolike.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://px.bjjhwx.cn

Ruby: warn "err"
来源：http://vq.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://ed.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://fa.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://sh.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tr.chemitech.net.cn

JS:   require.main === module
来源：http://xe.wgjwhj.cn

TS:   require.main === module
来源：http://ka.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://zp.lnxyls.cn

Go:   func main()
来源：http://ak.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ja.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://sq.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://yl.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://fr.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://jx.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://kf.hahajie.cn

TS:   process.platform;  process.version
来源：http://mf.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qg.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ou.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pj.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yc.hahajie.cn

================================================================================
来源：http://lt.shtwfgs.cn

N. 数据结构与算法
来源：http://oh.huixinmuqiang.cn

================================================================================
来源：http://yz.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://qr.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ri.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hu.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tc.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://av.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kz.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://zi.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oo.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dk.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://mf.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://bz.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sz.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nh.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mm.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qe.hahajie.cn

Go:   slices.Sort(arr)
来源：http://on.szsharing.cn

Ruby: arr.sort
来源：http://me.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://py.jianghongdianzi.cn

[N03] 快速排序（分治示例）
来源：http://oe.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mh.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://rl.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yj.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nj.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wu.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rf.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://et.asd995.cn

[N04] 斐波那契数列
来源：http://qv.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wf.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hd.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xw.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dp.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jf.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wh.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qy.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hq.nszjky.cn

[N05] 最大公约数
来源：http://xl.colortex.cn

Py:   math.gcd(a, b)
来源：http://kh.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xs.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hl.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dy.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://do.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mu.newstarts.cn

Ruby: a.gcd(b)
来源：http://cl.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wt.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://cn.chemitech.net.cn

Py:   s == s[::-1]
来源：http://mz.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://nx.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://tx.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://ta.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ki.huanxung.cn

Go:   // 双指针从两端比较
来源：http://pt.nszjky.cn

Ruby: s == s.reverse
来源：http://zx.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ji.colortex.cn

[N07] 两数之和（返回下标）
来源：http://in.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fi.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nr.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ui.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://an.gzmigu.cn

Java: // 手写 HashMap
来源：http://pe.nicolike.cn

Go:   // 手写 map[int]int
来源：http://gm.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://wd.wgjwhj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://em.muxihuayi.cn

[N08] 生成全排列
来源：http://te.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://by.huanxung.cn

PHP:  // 手写递归交换
来源：http://vk.asd995.cn

JS:   // 手写回溯递归
来源：http://lr.nszjky.cn

TS:   // 手写回溯递归
来源：http://nu.hnjuh.cn

Java: // 手写回溯递归
来源：http://mq.newstarts.cn

Go:   // 手写回溯递归
来源：http://xh.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://kh.newstarts.cn

C#:   // 手写回溯递归
来源：http://vc.gzmigu.cn

[N09] 栈与队列
来源：http://yw.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ig.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pi.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cl.bjjhwx.cn


<!-- 参考信息 -->