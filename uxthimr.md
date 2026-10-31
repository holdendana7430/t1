代发 wailian999

TS:   JSON.parse(s)
来源：http://vp.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://os.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://rk.9csxet.cn

Ruby: JSON.parse(s)
来源：http://xt.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ch.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nw.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rc.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://om.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bw.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ue.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wg.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ix.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zf.nicolike.cn

[K04] 读取 JSON 文件
来源：http://dw.nicolike.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://me.shxzukj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://my.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kw.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://no.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://by.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tq.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vv.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zh.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://ru.yuexingan06.cn

Py:   copy.deepcopy(obj)
来源：http://la.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://kt.newstarts.cn

JS:   structuredClone(obj)
来源：http://fy.newstarts.cn

TS:   structuredClone(obj)
来源：http://yp.shxzukj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://in.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oy.gzmigu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://my.muxihuayi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fk.panjiajie.cn

[K06] 解析 URL 查询串
来源：http://an.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ub.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tg.szxytkj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ki.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tt.hnjuh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ge.hahajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oq.chemitech.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hx.hnjuh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xx.shxzukj.cn

[K07] 进制转换
来源：http://mh.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jh.newstarts.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rm.asd995.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tu.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ut.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bw.521024.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ny.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zd.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sz.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://hj.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://iv.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hh.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://nl.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://rw.yuexingan06.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xv.huixinmuqiang.cn

Go:   encoding/gob
来源：http://nn.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://au.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gd.bookmarksfly.cn

================================================================================
来源：http://ek.yuntaijiaju.cn

L. 网络请求
来源：http://er.chemitech.net.cn

================================================================================
来源：http://mg.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://mx.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vs.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fk.hahajie.cn

JS:   await fetch(url)
来源：http://hz.muxihuayi.cn

TS:   await fetch(url)
来源：http://iu.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ub.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://oy.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ph.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ez.huanxung.cn

[L02] 发送 POST JSON
来源：http://tj.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hj.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mc.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hu.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rn.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hq.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vm.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hd.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://ih.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uv.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cg.szxytkj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kq.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://di.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fc.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rv.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ef.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fj.bjjhwx.cn

[L04] 设置超时
来源：http://cp.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://hi.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hb.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zs.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kx.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xq.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pq.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ge.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wo.szsharing.cn

[L05] 上传文件（multipart）
来源：http://kk.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://im.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yh.yuntaijiaju.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ix.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gp.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zq.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fv.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qa.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wj.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://ai.shxzskj.cn

Py:   resp.json()
来源：http://dd.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://sx.wgjwhj.cn

JS:   await resp.json()
来源：http://qz.asd995.cn

TS:   await resp.json()
来源：http://xt.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hn.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wf.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://of.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jp.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://st.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pe.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jq.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://nn.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://iq.colortex.cn

Java: resp.statusCode()
来源：http://qa.nicolike.cn

Go:   resp.StatusCode
来源：http://bb.nicolike.cn

Ruby: resp.code.to_i
来源：http://bo.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://uw.asd995.cn

[L08] 并发请求多个地址
来源：http://ll.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ln.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://wh.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ab.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ui.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wf.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wl.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yx.huixinmuqiang.cn

================================================================================
来源：http://br.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://oy.9csxet.cn

================================================================================
来源：http://we.huanxung.cn

[M01] 读取命令行参数
来源：http://jv.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://ry.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://ks.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://zt.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://un.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://bu.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://vt.jianghongdianzi.cn

Ruby: ARGV
来源：http://jv.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://iq.yuexingan06.cn

[M02] 读取环境变量
来源：http://vg.szsharing.cn

Py:   os.environ.get("HOME")
来源：http://ok.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rs.haigaiapp.cn

JS:   process.env.HOME
来源：http://bi.gzmigu.cn

TS:   process.env.HOME
来源：http://ya.9csxet.cn

Java: System.getenv("HOME")
来源：http://qt.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ay.asd995.cn

Ruby: ENV["HOME"]
来源：http://yr.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://px.shxzskj.cn

[M03] 执行外部命令
来源：http://le.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jr.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gy.muxihuayi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iz.colortex.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://id.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://le.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kd.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ks.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://bo.hnjuh.cn

[M04] 获取当前工作目录
来源：http://qs.9csxet.cn

Py:   os.getcwd()
来源：http://by.9csxet.cn

PHP:  getcwd();
来源：http://vk.gzmigu.cn

JS:   process.cwd()
来源：http://bt.jianghongdianzi.cn

TS:   process.cwd()
来源：http://wk.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://gm.nicolike.cn

Go:   os.Getwd()
来源：http://tf.chemitech.net.cn

Ruby: Dir.pwd
来源：http://lk.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xx.huixiangedu.cn

[M05] 设置退出码
来源：http://lr.shxzskj.cn

Py:   sys.exit(1)
来源：http://cd.shxzskj.cn

PHP:  exit(1);
来源：http://ko.muxihuayi.cn

JS:   process.exit(1)
来源：http://vf.nszjky.cn

TS:   process.exit(1)
来源：http://ts.chemitech.net.cn

Java: System.exit(1)
来源：http://iq.szsharing.cn

Go:   os.Exit(1)
来源：http://tl.wgjwhj.cn

Ruby: exit 1
来源：http://ny.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vx.gzmigu.cn

[M06] 向标准错误输出
来源：http://le.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://lr.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mu.521024.cn

JS:   console.error("err")
来源：http://vp.wgjwhj.cn

TS:   console.error("err")
来源：http://dt.521024.cn

Java: System.err.println("err")
来源：http://wo.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haigaiapp.cn

Ruby: warn "err"
来源：http://jr.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://zi.521024.cn

[M07] 判断是否为主入口
来源：http://me.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://re.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dx.wgjwhj.cn

JS:   require.main === module
来源：http://ro.colortex.cn

TS:   require.main === module
来源：http://xw.9csxet.cn

Java: public static void main(String[] args)
来源：http://ps.lnxyls.cn

Go:   func main()
来源：http://tg.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rw.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://sh.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://hs.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://ef.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://pa.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://uw.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://dk.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pg.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sz.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gh.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ci.szxytkj.cn

================================================================================
来源：http://td.shxzukj.cn

N. 数据结构与算法
来源：http://sb.yuexingan06.cn

================================================================================
来源：http://qa.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://wx.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ev.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://db.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xo.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xh.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://gz.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yp.newstarts.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bs.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://jw.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://lj.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ey.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pn.huixiangedu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ym.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hh.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://oy.jianghongdianzi.cn

Ruby: arr.sort
来源：http://fb.hahajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fe.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://vg.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jk.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://fr.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sb.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gi.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ml.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sb.huanxung.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pb.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pj.521024.cn

[N04] 斐波那契数列
来源：http://vr.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zl.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zb.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ma.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qj.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://we.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hd.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://my.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sd.shxzukj.cn

[N05] 最大公约数
来源：http://ol.nszjky.cn

Py:   math.gcd(a, b)
来源：http://up.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rr.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bk.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://it.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qn.bookmarksfly.cn

Ruby: a.gcd(b)
来源：http://ii.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ps.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://om.colortex.cn

Py:   s == s[::-1]
来源：http://ww.9csxet.cn

PHP:  $s === strrev($s);
来源：http://ek.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://sa.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://ka.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://id.newstarts.cn

Go:   // 双指针从两端比较
来源：http://wb.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ko.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yt.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://gx.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zv.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qm.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sz.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://ht.huanxung.cn

Java: // 手写 HashMap
来源：http://iv.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://lj.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://fb.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pk.lnxyls.cn

[N08] 生成全排列
来源：http://eq.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://ot.colortex.cn

PHP:  // 手写递归交换
来源：http://xh.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://ao.newstarts.cn

TS:   // 手写回溯递归
来源：http://ws.shtwfgs.cn

Java: // 手写回溯递归
来源：http://wh.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://st.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://of.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://gh.szsharing.cn

[N09] 栈与队列
来源：http://ic.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rb.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ob.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://td.jianghongdianzi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rk.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ia.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cd.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qk.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jz.huixiangedu.cn

[N10] 链表节点定义
来源：http://hm.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bh.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fp.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ra.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tj.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://ln.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oq.panjiajie.cn


<!-- 参考信息 -->