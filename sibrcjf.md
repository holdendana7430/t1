代发 wailian999

TS:   JSON.parse(s)
来源：http://xv.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ef.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://xm.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://cs.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ka.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://zd.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pi.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zb.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gc.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wp.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://km.jctech888.com.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oh.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bw.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jw.colortex.cn

[K04] 读取 JSON 文件
来源：http://gh.chemitech.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wb.haigaiapp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://de.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xv.bjjhwx.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xn.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nl.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dt.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cu.nicolike.cn

[K05] 深拷贝对象
来源：http://va.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://wp.hahajie.cn

PHP:  unserialize(serialize($obj));
来源：http://az.newstarts.cn

JS:   structuredClone(obj)
来源：http://by.szxytkj.cn

TS:   structuredClone(obj)
来源：http://xi.huixinmuqiang.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oh.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tc.chemitech.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ai.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nn.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://mt.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hi.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yd.nicolike.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zh.521024.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aa.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lu.bjjhwx.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dv.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pq.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cb.yuntaijiaju.cn

[K07] 进制转换
来源：http://zr.panjiajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://km.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nj.bjjhwx.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dz.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ql.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://do.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jz.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://id.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pj.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://rh.nicolike.cn

Py:   pickle.dumps(obj)
来源：http://fd.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vz.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://af.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://me.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jg.colortex.cn

Go:   encoding/gob
来源：http://ce.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://kq.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hx.gzmigu.cn

================================================================================
来源：http://af.hahajie.cn

L. 网络请求
来源：http://ol.9csxet.cn

================================================================================
来源：http://op.asd995.cn

[L01] 发送 GET 请求
来源：http://ue.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gj.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pj.muxihuayi.cn

JS:   await fetch(url)
来源：http://ou.chemitech.net.cn

TS:   await fetch(url)
来源：http://ay.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bo.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://zj.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rk.chemitech.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://me.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://df.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rv.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mz.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://en.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dm.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xp.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bx.shxzskj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lh.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cu.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://qx.szsharing.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ig.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ul.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dh.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tb.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ir.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pp.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sl.shtwfgs.cn

[L04] 设置超时
来源：http://bi.huixiangedu.cn

Py:   requests.get(url, timeout=5)
来源：http://cy.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yl.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zr.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zn.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ov.haigaiapp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ww.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dt.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gi.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://sw.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://at.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xj.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dh.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kb.gzmigu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kd.lnxyls.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wg.yuexingan06.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://um.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bj.521024.cn

[L06] 解析响应为 JSON
来源：http://dn.bjjhwx.cn

Py:   resp.json()
来源：http://xd.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://ae.shxzskj.cn

JS:   await resp.json()
来源：http://uh.nicolike.cn

TS:   await resp.json()
来源：http://ig.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://za.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pi.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ns.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ft.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ul.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jp.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gv.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://nn.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://hs.jctech888.com.cn

Java: resp.statusCode()
来源：http://ab.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://wx.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://td.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://gr.nicolike.cn

[L08] 并发请求多个地址
来源：http://dr.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ng.jctech888.com.cn

PHP:  curl_multi_init() 系列
来源：http://kd.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.521024.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zj.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jc.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wm.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fq.hahajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gc.bjjhwx.cn

================================================================================
来源：http://xz.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://xg.yuntaijiaju.cn

================================================================================
来源：http://bx.nszjky.cn

[M01] 读取命令行参数
来源：http://vh.szsharing.cn

Py:   sys.argv[1:]
来源：http://ib.521024.cn

PHP:  $argv;  $argc;
来源：http://qw.shtwfgs.cn

JS:   process.argv.slice(2)
来源：http://in.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://qa.asd995.cn

Java: args 数组（main 方法参数）
来源：http://hj.jctech888.com.cn

Go:   os.Args[1:]
来源：http://ky.lnxyls.cn

Ruby: ARGV
来源：http://vc.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://ng.shxzskj.cn

[M02] 读取环境变量
来源：http://ma.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://xb.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uk.colortex.cn

JS:   process.env.HOME
来源：http://hm.wgjwhj.cn

TS:   process.env.HOME
来源：http://hl.szsharing.cn

Java: System.getenv("HOME")
来源：http://nk.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://la.yuexingan06.cn

Ruby: ENV["HOME"]
来源：http://wk.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ke.nicolike.cn

[M03] 执行外部命令
来源：http://yb.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qm.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bi.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://am.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ts.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ft.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zu.newstarts.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ma.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://wc.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://se.lnxyls.cn

Py:   os.getcwd()
来源：http://ue.shxzukj.cn

PHP:  getcwd();
来源：http://hr.jianghongdianzi.cn

JS:   process.cwd()
来源：http://zp.haigaiapp.cn

TS:   process.cwd()
来源：http://rn.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://sz.shtwfgs.cn

Go:   os.Getwd()
来源：http://md.muxihuayi.cn

Ruby: Dir.pwd
来源：http://mh.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iv.lnxyls.cn

[M05] 设置退出码
来源：http://iq.panjiajie.cn

Py:   sys.exit(1)
来源：http://xr.jctech888.com.cn

PHP:  exit(1);
来源：http://fe.hnjuh.cn

JS:   process.exit(1)
来源：http://mq.hnjuh.cn

TS:   process.exit(1)
来源：http://nr.newstarts.cn

Java: System.exit(1)
来源：http://nh.muxihuayi.cn

Go:   os.Exit(1)
来源：http://il.lnxyls.cn

Ruby: exit 1
来源：http://xu.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sj.huixiangedu.cn

[M06] 向标准错误输出
来源：http://ap.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://cd.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ki.lnxyls.cn

JS:   console.error("err")
来源：http://by.colortex.cn

TS:   console.error("err")
来源：http://nc.lnxyls.cn

Java: System.err.println("err")
来源：http://ky.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dp.lnxyls.cn

Ruby: warn "err"
来源：http://xw.panjiajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://hy.lnxyls.cn

[M07] 判断是否为主入口
来源：http://tn.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://ij.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wp.asd995.cn

JS:   require.main === module
来源：http://zk.bjjhwx.cn

TS:   require.main === module
来源：http://rv.chemitech.net.cn

Java: public static void main(String[] args)
来源：http://jj.jianghongdianzi.cn

Go:   func main()
来源：http://am.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qq.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://vi.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://kb.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://xa.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://zv.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://hw.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://ai.hahajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cb.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zk.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nv.9csxet.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bo.hnjuh.cn

================================================================================
来源：http://gp.wgjwhj.cn

N. 数据结构与算法
来源：http://cg.hahajie.cn

================================================================================
来源：http://lj.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://ld.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kr.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://he.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nn.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ot.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ht.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://rx.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xu.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ed.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://cb.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ub.yuntaijiaju.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://le.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://br.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ge.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uf.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://ba.panjiajie.cn

Ruby: arr.sort
来源：http://nb.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ya.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://gt.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dn.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://dy.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zo.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ov.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ar.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ph.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tf.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iv.chemitech.net.cn

[N04] 斐波那契数列
来源：http://za.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gy.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ab.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lo.chemitech.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zl.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gz.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://li.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ir.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tf.yuntaijiaju.cn

[N05] 最大公约数
来源：http://dl.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://ni.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yn.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mv.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ng.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dw.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gu.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://sq.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lx.shtwfgs.cn

[N06] 判断回文字符串
来源：http://ay.asd995.cn

Py:   s == s[::-1]
来源：http://sv.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://uy.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://ps.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://hd.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fx.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://ph.szsharing.cn

Ruby: s == s.reverse
来源：http://yr.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lr.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://gx.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pa.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://up.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bd.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://xo.bjjhwx.cn

Java: // 手写 HashMap
来源：http://je.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://jt.nicolike.cn

Ruby: // 手写 Hash
来源：http://bt.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gf.huixinmuqiang.cn

[N08] 生成全排列
来源：http://gw.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://fc.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://nn.newstarts.cn

JS:   // 手写回溯递归
来源：http://oh.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://ju.muxihuayi.cn

Java: // 手写回溯递归
来源：http://re.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://gv.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ax.hnjuh.cn

C#:   // 手写回溯递归
来源：http://mz.yuexingan06.cn

[N09] 栈与队列
来源：http://rw.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nm.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fk.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mt.szxytkj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fk.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sg.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ep.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yd.muxihuayi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uz.newstarts.cn

[N10] 链表节点定义
来源：http://vq.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tp.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oo.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nm.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kg.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://tu.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tj.huanxung.cn


<!-- 参考信息 -->