代发 wailian999

TS:   JSON.parse(s)
来源：http://xm.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ry.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://yg.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://gi.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ag.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://aq.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pi.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gm.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cc.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://er.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fz.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pf.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ii.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nk.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://dj.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hb.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mx.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dp.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nn.hnjuh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nj.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ri.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://is.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kf.shtwfgs.cn

[K05] 深拷贝对象
来源：http://ty.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://uq.yuexingan06.cn

PHP:  unserialize(serialize($obj));
来源：http://ro.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://gu.szxytkj.cn

TS:   structuredClone(obj)
来源：http://ey.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mm.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sm.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://is.szxytkj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xt.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://rx.jianghongdianzi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oe.newstarts.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://be.yuexingan06.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dr.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yz.bjjhwx.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xy.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hm.colortex.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://du.lnxyls.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lp.colortex.cn

[K07] 进制转换
来源：http://pg.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zy.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rd.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qd.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://we.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ra.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://be.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ok.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kc.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://jk.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://dt.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iv.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://vv.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://tw.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nh.521024.cn

Go:   encoding/gob
来源：http://zm.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://qi.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://og.colortex.cn

================================================================================
来源：http://vp.yuntaijiaju.cn

L. 网络请求
来源：http://dm.nszjky.cn

================================================================================
来源：http://qf.newstarts.cn

[L01] 发送 GET 请求
来源：http://sq.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gb.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zr.huixiangedu.cn

JS:   await fetch(url)
来源：http://tx.jctech888.com.cn

TS:   await fetch(url)
来源：http://ah.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sx.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://vs.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tp.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ne.szsharing.cn

[L02] 发送 POST JSON
来源：http://tu.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ok.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vy.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pt.jctech888.com.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ok.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jj.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nm.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://py.colortex.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ne.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://cv.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wj.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vc.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lk.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fq.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ov.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bu.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ws.yuntaijiaju.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ri.wgjwhj.cn

[L04] 设置超时
来源：http://ni.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://yr.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nw.nicolike.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sp.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://re.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://od.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://or.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rf.hahajie.cn

[L05] 上传文件（multipart）
来源：http://pa.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zv.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gj.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ar.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ho.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cg.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sm.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kg.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eg.hahajie.cn

[L06] 解析响应为 JSON
来源：http://ho.yuexingan06.cn

Py:   resp.json()
来源：http://ua.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://zk.muxihuayi.cn

JS:   await resp.json()
来源：http://ln.szsharing.cn

TS:   await resp.json()
来源：http://jt.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gr.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mu.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://je.shtwfgs.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tf.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://jn.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fs.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eu.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://ya.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://vf.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://ej.lnxyls.cn

Go:   resp.StatusCode
来源：http://jw.shxzskj.cn

Ruby: resp.code.to_i
来源：http://fi.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://qp.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://xc.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wo.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://rd.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zw.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://md.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ff.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://df.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vh.shxzukj.cn

================================================================================
来源：http://pq.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://fb.yuntaijiaju.cn

================================================================================
来源：http://zd.shtwfgs.cn

[M01] 读取命令行参数
来源：http://da.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://fd.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://vn.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ab.9csxet.cn

TS:   process.argv.slice(2)
来源：http://jv.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ti.newstarts.cn

Go:   os.Args[1:]
来源：http://au.huixiangedu.cn

Ruby: ARGV
来源：http://ss.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://fa.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://jr.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://ht.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bu.chemitech.net.cn

JS:   process.env.HOME
来源：http://jl.9csxet.cn

TS:   process.env.HOME
来源：http://xu.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://jy.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ls.asd995.cn

Ruby: ENV["HOME"]
来源：http://fy.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ef.szxytkj.cn

[M03] 执行外部命令
来源：http://wu.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fs.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mn.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yf.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mx.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hv.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ez.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ik.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://ic.szsharing.cn

[M04] 获取当前工作目录
来源：http://wc.huanxung.cn

Py:   os.getcwd()
来源：http://rb.bookmarksfly.cn

PHP:  getcwd();
来源：http://wp.521024.cn

JS:   process.cwd()
来源：http://xg.bookmarksfly.cn

TS:   process.cwd()
来源：http://qz.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://lx.newstarts.cn

Go:   os.Getwd()
来源：http://mg.521024.cn

Ruby: Dir.pwd
来源：http://mm.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ws.szxytkj.cn

[M05] 设置退出码
来源：http://pm.shxzukj.cn

Py:   sys.exit(1)
来源：http://tr.yuexingan06.cn

PHP:  exit(1);
来源：http://mh.newstarts.cn

JS:   process.exit(1)
来源：http://dk.gzmigu.cn

TS:   process.exit(1)
来源：http://wd.bjjhwx.cn

Java: System.exit(1)
来源：http://do.chemitech.net.cn

Go:   os.Exit(1)
来源：http://xa.gzmigu.cn

Ruby: exit 1
来源：http://el.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nc.nszjky.cn

[M06] 向标准错误输出
来源：http://xy.9csxet.cn

Py:   print("err", file=sys.stderr)
来源：http://ej.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tp.asd995.cn

JS:   console.error("err")
来源：http://li.shxzukj.cn

TS:   console.error("err")
来源：http://ey.shxzukj.cn

Java: System.err.println("err")
来源：http://de.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://al.muxihuayi.cn

Ruby: warn "err"
来源：http://co.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://hq.nicolike.cn

[M07] 判断是否为主入口
来源：http://gv.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://wu.jianghongdianzi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nf.521024.cn

JS:   require.main === module
来源：http://ls.nicolike.cn

TS:   require.main === module
来源：http://vx.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ci.newstarts.cn

Go:   func main()
来源：http://px.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tm.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://em.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://pu.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://be.huixiangedu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ff.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://fd.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://bm.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://om.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hf.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ea.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cb.chemitech.net.cn

================================================================================
来源：http://uw.huanxung.cn

N. 数据结构与算法
来源：http://tb.huanxung.cn

================================================================================
来源：http://mz.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://wx.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zq.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aa.asd995.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oy.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fg.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ls.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ag.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://st.lnxyls.cn

[N02] 排序（工程实践用内置实现）
来源：http://lq.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://za.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lh.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ze.szsharing.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://my.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://oe.521024.cn

Ruby: arr.sort
来源：http://cp.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uj.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://tl.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oy.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://pp.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sb.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bg.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yp.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wl.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cb.chemitech.net.cn

[N04] 斐波那契数列
来源：http://fj.bookmarksfly.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ju.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://th.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mf.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xk.jianghongdianzi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jz.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://de.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gg.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jj.chemitech.net.cn

[N05] 最大公约数
来源：http://tp.521024.cn

Py:   math.gcd(a, b)
来源：http://jv.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cy.bookmarksfly.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ei.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ql.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yl.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uj.521024.cn

Ruby: a.gcd(b)
来源：http://mh.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ig.shxzskj.cn

[N06] 判断回文字符串
来源：http://zs.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ob.521024.cn

PHP:  $s === strrev($s);
来源：http://uz.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://fj.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://bk.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rt.nszjky.cn

Go:   // 双指针从两端比较
来源：http://aa.hahajie.cn

Ruby: s == s.reverse
来源：http://uu.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nb.nicolike.cn

[N07] 两数之和（返回下标）
来源：http://lw.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tq.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dl.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ka.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://zd.chemitech.net.cn

Java: // 手写 HashMap
来源：http://gc.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://ul.hnjuh.cn

Ruby: // 手写 Hash
来源：http://rs.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vl.bjjhwx.cn

[N08] 生成全排列
来源：http://ud.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://xk.szsharing.cn

PHP:  // 手写递归交换
来源：http://qo.szsharing.cn

JS:   // 手写回溯递归
来源：http://iv.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://xq.shxzukj.cn

Java: // 手写回溯递归
来源：http://sm.colortex.cn

Go:   // 手写回溯递归
来源：http://pd.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://vu.hahajie.cn

C#:   // 手写回溯递归
来源：http://mp.521024.cn

[N09] 栈与队列
来源：http://an.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lu.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uy.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://io.nicolike.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://of.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ma.szsharing.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bm.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ql.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://te.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://vt.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vx.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dn.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ab.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jd.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://kr.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ox.szsharing.cn


<!-- 参考信息 -->