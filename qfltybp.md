代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lr.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://yc.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zh.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gl.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tv.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qz.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vr.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://he.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dr.521024.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bb.huixiangedu.cn

[K04] 读取 JSON 文件
来源：http://my.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dg.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wp.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://of.9csxet.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hb.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ec.lnxyls.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fj.asd995.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hn.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yb.muxihuayi.cn

[K05] 深拷贝对象
来源：http://pb.huixiangedu.cn

Py:   copy.deepcopy(obj)
来源：http://rn.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://zw.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://im.nicolike.cn

TS:   structuredClone(obj)
来源：http://vu.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tm.gzmigu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mw.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ep.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wi.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://hy.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sz.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yt.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gg.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://af.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ft.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://om.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xf.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qt.gzmigu.cn

[K07] 进制转换
来源：http://qc.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ao.bookmarksfly.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pi.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gk.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rr.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ak.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rg.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hy.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ii.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://fg.chemitech.net.cn

Py:   pickle.dumps(obj)
来源：http://fd.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mj.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://tp.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ka.jctech888.com.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bb.yuntaijiaju.cn

Go:   encoding/gob
来源：http://aw.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://ph.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oj.newstarts.cn

================================================================================
来源：http://zn.9csxet.cn

L. 网络请求
来源：http://lc.chemitech.net.cn

================================================================================
来源：http://fq.szxytkj.cn

[L01] 发送 GET 请求
来源：http://nd.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ha.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uk.9csxet.cn

JS:   await fetch(url)
来源：http://ch.panjiajie.cn

TS:   await fetch(url)
来源：http://kt.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dc.huixiangedu.cn

Go:   resp, err := http.Get(url)
来源：http://ma.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oq.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ej.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://xv.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kb.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hx.lnxyls.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kl.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bb.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vy.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hl.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vu.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mf.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://tg.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ku.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ds.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jo.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qt.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kc.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ew.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vp.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xv.chemitech.net.cn

[L04] 设置超时
来源：http://xv.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://ue.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fv.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aw.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mv.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bb.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jj.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yf.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://bn.yuntaijiaju.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eu.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zh.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gj.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lp.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tu.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rv.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nx.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yk.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://oi.lnxyls.cn

Py:   resp.json()
来源：http://kz.bookmarksfly.cn

PHP:  json_decode($body, true);
来源：http://mg.chemitech.net.cn

JS:   await resp.json()
来源：http://mo.yuexingan06.cn

TS:   await resp.json()
来源：http://ep.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vh.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qw.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://sm.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lx.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://up.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ph.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bf.wgjwhj.cn

JS:   resp.ok;  resp.status
来源：http://pn.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://mm.jctech888.com.cn

Java: resp.statusCode()
来源：http://ei.colortex.cn

Go:   resp.StatusCode
来源：http://eo.gzmigu.cn

Ruby: resp.code.to_i
来源：http://mg.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ek.szxytkj.cn

[L08] 并发请求多个地址
来源：http://iw.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gb.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://mt.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tw.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ox.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vs.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qv.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jz.yuntaijiaju.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lc.colortex.cn

================================================================================
来源：http://ql.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://hm.muxihuayi.cn

================================================================================
来源：http://de.hnjuh.cn

[M01] 读取命令行参数
来源：http://od.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://qy.nszjky.cn

PHP:  $argv;  $argc;
来源：http://gs.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://oc.szsharing.cn

TS:   process.argv.slice(2)
来源：http://rd.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://et.hnjuh.cn

Go:   os.Args[1:]
来源：http://od.bookmarksfly.cn

Ruby: ARGV
来源：http://ht.jianghongdianzi.cn

C#:   args 数组（Main 方法参数）
来源：http://wf.shxzskj.cn

[M02] 读取环境变量
来源：http://cl.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://jz.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gy.jctech888.com.cn

JS:   process.env.HOME
来源：http://rc.bookmarksfly.cn

TS:   process.env.HOME
来源：http://hd.521024.cn

Java: System.getenv("HOME")
来源：http://qs.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bb.asd995.cn

Ruby: ENV["HOME"]
来源：http://gn.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zv.yuexingan06.cn

[M03] 执行外部命令
来源：http://nh.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://el.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gy.jctech888.com.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ue.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vy.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://av.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://go.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://md.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://hb.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://od.panjiajie.cn

Py:   os.getcwd()
来源：http://rg.chemitech.net.cn

PHP:  getcwd();
来源：http://hs.huixiangedu.cn

JS:   process.cwd()
来源：http://us.panjiajie.cn

TS:   process.cwd()
来源：http://su.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ya.wgjwhj.cn

Go:   os.Getwd()
来源：http://bm.hahajie.cn

Ruby: Dir.pwd
来源：http://ef.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ql.shtwfgs.cn

[M05] 设置退出码
来源：http://pt.huanxung.cn

Py:   sys.exit(1)
来源：http://ig.lnxyls.cn

PHP:  exit(1);
来源：http://hm.jctech888.com.cn

JS:   process.exit(1)
来源：http://tq.shtwfgs.cn

TS:   process.exit(1)
来源：http://vq.asd995.cn

Java: System.exit(1)
来源：http://zb.hahajie.cn

Go:   os.Exit(1)
来源：http://ab.hahajie.cn

Ruby: exit 1
来源：http://eu.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xr.panjiajie.cn

[M06] 向标准错误输出
来源：http://gn.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://tg.chemitech.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dm.bjjhwx.cn

JS:   console.error("err")
来源：http://sb.jctech888.com.cn

TS:   console.error("err")
来源：http://rr.wgjwhj.cn

Java: System.err.println("err")
来源：http://ft.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vd.yuntaijiaju.cn

Ruby: warn "err"
来源：http://rb.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://pp.muxihuayi.cn

[M07] 判断是否为主入口
来源：http://aq.colortex.cn

Py:   if __name__ == "__main__":
来源：http://vj.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uf.nszjky.cn

JS:   require.main === module
来源：http://cc.bjjhwx.cn

TS:   require.main === module
来源：http://zv.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://gt.jctech888.com.cn

Go:   func main()
来源：http://ma.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://su.bookmarksfly.cn

C#:   static void Main(string[] args)
来源：http://ok.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://va.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://ms.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://aa.panjiajie.cn

JS:   process.platform;  process.version
来源：http://ot.asd995.cn

TS:   process.platform;  process.version
来源：http://vu.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kh.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://se.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kj.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ql.huixinmuqiang.cn

================================================================================
来源：http://wz.wgjwhj.cn

N. 数据结构与算法
来源：http://hz.colortex.cn

================================================================================
来源：http://oj.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://fl.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ir.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vq.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wk.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wo.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fx.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://gf.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xf.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iq.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://tw.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vt.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iy.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://in.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ba.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://on.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://ll.yuexingan06.cn

Ruby: arr.sort
来源：http://eo.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cn.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://un.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ou.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://jw.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xb.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gw.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ma.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ql.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nn.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mn.shtwfgs.cn

[N04] 斐波那契数列
来源：http://cy.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://na.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yi.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mh.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jx.lnxyls.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vs.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yd.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kv.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hs.wgjwhj.cn

[N05] 最大公约数
来源：http://uv.nicolike.cn

Py:   math.gcd(a, b)
来源：http://ux.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tx.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ku.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hw.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kr.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wk.gzmigu.cn

Ruby: a.gcd(b)
来源：http://jy.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mb.chemitech.net.cn

[N06] 判断回文字符串
来源：http://vr.hnjuh.cn

Py:   s == s[::-1]
来源：http://sk.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://nk.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://ho.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://ld.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hv.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://vm.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ox.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rn.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ge.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pf.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ka.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yb.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://cv.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://bi.nszjky.cn

Go:   // 手写 map[int]int
来源：http://gb.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://ww.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://es.colortex.cn

[N08] 生成全排列
来源：http://ab.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://lu.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://gc.nicolike.cn

JS:   // 手写回溯递归
来源：http://cm.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://ct.gzmigu.cn

Java: // 手写回溯递归
来源：http://dp.newstarts.cn

Go:   // 手写回溯递归
来源：http://bc.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://kr.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://om.shxzskj.cn

[N09] 栈与队列
来源：http://vh.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xq.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mv.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ax.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ji.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xm.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vq.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ae.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jf.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://fe.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zf.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nu.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gd.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sn.9csxet.cn

Java: class Node { int v; Node next; }
来源：http://ve.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ua.haigaiapp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qz.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qv.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://ul.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sg.chemitech.net.cn


<!-- 参考信息 -->