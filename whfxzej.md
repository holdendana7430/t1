代发 wailian999

[K02] JSON 字符串转对象
来源：http://le.colortex.cn

Py:   json.loads(s)
来源：http://dz.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nu.panjiajie.cn

JS:   JSON.parse(s)
来源：http://no.shxzukj.cn

TS:   JSON.parse(s)
来源：http://et.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ga.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://no.hahajie.cn

Ruby: JSON.parse(s)
来源：http://zb.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hi.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ej.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cj.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cy.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ui.chemitech.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wr.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ia.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vb.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zl.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wx.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://fh.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ja.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pr.hnjuh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pd.nszjky.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tj.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sz.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ht.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ex.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gq.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://kc.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://yf.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://mi.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://id.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://my.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gz.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://go.colortex.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://el.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ay.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://lq.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pw.nicolike.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dp.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gc.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sx.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ku.nicolike.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tg.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fs.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ak.szxytkj.cn

[K07] 进制转换
来源：http://lz.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://og.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yh.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://io.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://de.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wf.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://us.huixinmuqiang.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pq.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xz.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://kp.gzmigu.cn

Py:   pickle.dumps(obj)
来源：http://ki.yuexingan06.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://su.shxzskj.cn

JS:   v8.serialize(obj)        // Node
来源：http://dc.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://se.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ih.nszjky.cn

Go:   encoding/gob
来源：http://eh.521024.cn

Ruby: Marshal.dump(obj)
来源：http://bt.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uh.nicolike.cn

================================================================================
来源：http://cy.huixiangedu.cn

L. 网络请求
来源：http://qn.yuexingan06.cn

================================================================================
来源：http://th.nszjky.cn

[L01] 发送 GET 请求
来源：http://dv.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sb.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uq.huixiangedu.cn

JS:   await fetch(url)
来源：http://sp.newstarts.cn

TS:   await fetch(url)
来源：http://yg.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bo.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://sh.asd995.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wm.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pw.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://fe.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pw.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qw.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ie.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tb.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nn.jianghongdianzi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://it.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lt.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://on.521024.cn

[L03] 设置自定义请求头
来源：http://rs.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ud.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qv.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vh.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wx.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xj.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eu.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://si.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fd.bookmarksfly.cn

[L04] 设置超时
来源：http://ve.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://jw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vp.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wq.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zf.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fs.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://co.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ba.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hj.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://ju.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bm.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://op.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ck.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://by.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ab.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://db.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://id.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gj.9csxet.cn

[L06] 解析响应为 JSON
来源：http://bj.newstarts.cn

Py:   resp.json()
来源：http://wd.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://yr.huixinmuqiang.cn

JS:   await resp.json()
来源：http://uw.9csxet.cn

TS:   await resp.json()
来源：http://vn.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zw.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eo.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://uf.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ft.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://gu.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vs.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xa.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://td.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://cx.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://cw.nicolike.cn

Go:   resp.StatusCode
来源：http://kq.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://ba.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://mq.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://pl.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pg.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://xv.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ov.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ta.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ih.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hg.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kq.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://li.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://cx.szsharing.cn

[M01] 读取命令行参数
来源：http://bq.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ac.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://uq.panjiajie.cn

JS:   process.argv.slice(2)
来源：http://yt.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://re.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://nz.wgjwhj.cn

Go:   os.Args[1:]
来源：http://qf.huanxung.cn

Ruby: ARGV
来源：http://tl.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://xc.colortex.cn

[M02] 读取环境变量
来源：http://aq.521024.cn

Py:   os.environ.get("HOME")
来源：http://ch.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xl.lnxyls.cn

JS:   process.env.HOME
来源：http://ft.nicolike.cn

TS:   process.env.HOME
来源：http://tj.asd995.cn

Java: System.getenv("HOME")
来源：http://xa.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://df.colortex.cn

Ruby: ENV["HOME"]
来源：http://lb.huanxung.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sn.nszjky.cn

[M03] 执行外部命令
来源：http://bx.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mt.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ar.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qc.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dm.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nc.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rf.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fd.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://xz.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://oa.shtwfgs.cn

Py:   os.getcwd()
来源：http://ba.gzmigu.cn

PHP:  getcwd();
来源：http://mc.shxzskj.cn

JS:   process.cwd()
来源：http://py.521024.cn

TS:   process.cwd()
来源：http://gn.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://xt.nicolike.cn

Go:   os.Getwd()
来源：http://eq.hahajie.cn

Ruby: Dir.pwd
来源：http://mi.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sc.521024.cn

[M05] 设置退出码
来源：http://xd.szxytkj.cn

Py:   sys.exit(1)
来源：http://db.yuntaijiaju.cn

PHP:  exit(1);
来源：http://dc.521024.cn

JS:   process.exit(1)
来源：http://zs.szsharing.cn

TS:   process.exit(1)
来源：http://op.shtwfgs.cn

Java: System.exit(1)
来源：http://eu.asd995.cn

Go:   os.Exit(1)
来源：http://xk.haigaiapp.cn

Ruby: exit 1
来源：http://pg.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://as.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ik.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://eo.haigaiapp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ct.lnxyls.cn

JS:   console.error("err")
来源：http://nb.bjjhwx.cn

TS:   console.error("err")
来源：http://rg.shtwfgs.cn

Java: System.err.println("err")
来源：http://tv.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sa.bjjhwx.cn

Ruby: warn "err"
来源：http://xc.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ix.szsharing.cn

[M07] 判断是否为主入口
来源：http://dn.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://ef.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fc.jianghongdianzi.cn

JS:   require.main === module
来源：http://eo.shxzukj.cn

TS:   require.main === module
来源：http://ah.9csxet.cn

Java: public static void main(String[] args)
来源：http://na.bookmarksfly.cn

Go:   func main()
来源：http://mc.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ou.9csxet.cn

C#:   static void Main(string[] args)
来源：http://rm.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ci.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://il.huixinmuqiang.cn

PHP:  PHP_OS;  phpversion();
来源：http://jj.huanxung.cn

JS:   process.platform;  process.version
来源：http://gl.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://go.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://it.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dr.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://la.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dh.muxihuayi.cn

================================================================================
来源：http://xe.jctech888.com.cn

N. 数据结构与算法
来源：http://by.9csxet.cn

================================================================================
来源：http://di.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://sd.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zl.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ob.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lw.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ot.szxytkj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oq.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://ff.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zs.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ln.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://ur.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://td.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gf.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hw.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dd.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://pg.jianghongdianzi.cn

Ruby: arr.sort
来源：http://bk.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://en.521024.cn

[N03] 快速排序（分治示例）
来源：http://gy.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ll.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://qs.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xz.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iy.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://er.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pu.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hn.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tv.shtwfgs.cn

[N04] 斐波那契数列
来源：http://uz.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yb.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://to.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sa.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ii.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vb.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jr.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fr.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qg.bjjhwx.cn

[N05] 最大公约数
来源：http://hp.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://cf.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://te.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eg.shtwfgs.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ga.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jz.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mb.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ih.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nv.nszjky.cn

[N06] 判断回文字符串
来源：http://tt.panjiajie.cn

Py:   s == s[::-1]
来源：http://oo.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://cn.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://tq.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://ob.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ga.haigaiapp.cn

Go:   // 双指针从两端比较
来源：http://vs.panjiajie.cn

Ruby: s == s.reverse
来源：http://da.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wx.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://dq.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ga.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ip.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hx.521024.cn

TS:   // 手写 Map<string, number>
来源：http://no.shxzukj.cn

Java: // 手写 HashMap
来源：http://jz.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://ax.hnjuh.cn

Ruby: // 手写 Hash
来源：http://pz.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pg.bjjhwx.cn

[N08] 生成全排列
来源：http://ib.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://tw.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://vz.9csxet.cn

JS:   // 手写回溯递归
来源：http://tx.gzmigu.cn

TS:   // 手写回溯递归
来源：http://tk.nicolike.cn

Java: // 手写回溯递归
来源：http://jo.colortex.cn

Go:   // 手写回溯递归
来源：http://ap.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://ga.wgjwhj.cn

C#:   // 手写回溯递归
来源：http://sz.jianghongdianzi.cn

[N09] 栈与队列
来源：http://si.yuntaijiaju.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ux.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://em.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zn.wgjwhj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kr.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dr.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cb.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zz.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ja.shtwfgs.cn

[N10] 链表节点定义
来源：http://ln.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fb.jianghongdianzi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sf.jctech888.com.cn


<!-- 参考信息 -->