代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qb.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ia.szxytkj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://so.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ve.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qy.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wl.huanxung.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tr.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ho.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lq.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mq.9csxet.cn

[K04] 读取 JSON 文件
来源：http://ud.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://by.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cp.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xd.jctech888.com.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mx.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xd.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mt.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ql.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uj.szxytkj.cn

[K05] 深拷贝对象
来源：http://zp.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://bx.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://uh.yuexingan06.cn

JS:   structuredClone(obj)
来源：http://jn.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://aj.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gv.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ql.bookmarksfly.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fd.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pg.jianghongdianzi.cn

[K06] 解析 URL 查询串
来源：http://ys.jctech888.com.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://df.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hd.wgjwhj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xs.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://de.asd995.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rj.huixinmuqiang.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dw.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sq.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ge.haigaiapp.cn

[K07] 进制转换
来源：http://ci.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fr.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bv.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gv.panjiajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jf.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lm.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wx.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://el.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ml.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sp.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://ny.lnxyls.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yr.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://du.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://mp.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ko.gzmigu.cn

Go:   encoding/gob
来源：http://bj.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://qe.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vm.muxihuayi.cn

================================================================================
来源：http://wn.521024.cn

L. 网络请求
来源：http://md.nszjky.cn

================================================================================
来源：http://re.hahajie.cn

[L01] 发送 GET 请求
来源：http://wh.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oo.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wz.szsharing.cn

JS:   await fetch(url)
来源：http://gd.gzmigu.cn

TS:   await fetch(url)
来源：http://mg.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nz.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://em.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fm.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ai.hahajie.cn

[L02] 发送 POST JSON
来源：http://mb.szsharing.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pr.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sh.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cs.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ps.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pd.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ed.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ti.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://az.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://bx.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oh.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fs.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://su.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ch.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fs.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nv.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wj.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kd.9csxet.cn

[L04] 设置超时
来源：http://nj.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://us.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tz.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xd.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jz.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lx.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zc.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://af.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mo.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://xk.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qc.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://in.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gw.gzmigu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hd.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yp.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oi.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yc.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xn.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://vv.huanxung.cn

Py:   resp.json()
来源：http://gm.colortex.cn

PHP:  json_decode($body, true);
来源：http://wv.huixiangedu.cn

JS:   await resp.json()
来源：http://zl.lnxyls.cn

TS:   await resp.json()
来源：http://qt.szxytkj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ix.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bs.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://mo.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fg.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://yz.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ft.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pv.colortex.cn

JS:   resp.ok;  resp.status
来源：http://ey.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://is.szsharing.cn

Java: resp.statusCode()
来源：http://ry.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://oe.colortex.cn

Ruby: resp.code.to_i
来源：http://lx.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://nz.szsharing.cn

[L08] 并发请求多个地址
来源：http://tx.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ab.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://bv.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uv.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oz.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ay.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hq.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ja.lnxyls.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cq.gzmigu.cn

================================================================================
来源：http://ao.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://vq.bjjhwx.cn

================================================================================
来源：http://mi.yuexingan06.cn

[M01] 读取命令行参数
来源：http://hf.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://zu.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://qp.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://ls.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://ja.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://zv.colortex.cn

Go:   os.Args[1:]
来源：http://sc.bookmarksfly.cn

Ruby: ARGV
来源：http://wt.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://hp.bjjhwx.cn

[M02] 读取环境变量
来源：http://ah.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://rl.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hk.panjiajie.cn

JS:   process.env.HOME
来源：http://kk.shxzukj.cn

TS:   process.env.HOME
来源：http://ma.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://lh.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wz.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://go.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jw.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://sk.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fu.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://of.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nx.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fd.wgjwhj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bw.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wo.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lj.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://fj.shxzukj.cn

[M04] 获取当前工作目录
来源：http://jp.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://rn.jianghongdianzi.cn

PHP:  getcwd();
来源：http://wm.huixinmuqiang.cn

JS:   process.cwd()
来源：http://kl.huixiangedu.cn

TS:   process.cwd()
来源：http://lg.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ax.wgjwhj.cn

Go:   os.Getwd()
来源：http://fd.shtwfgs.cn

Ruby: Dir.pwd
来源：http://sg.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ij.huixiangedu.cn

[M05] 设置退出码
来源：http://uz.nicolike.cn

Py:   sys.exit(1)
来源：http://cq.muxihuayi.cn

PHP:  exit(1);
来源：http://tv.huanxung.cn

JS:   process.exit(1)
来源：http://xc.asd995.cn

TS:   process.exit(1)
来源：http://ya.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ld.hnjuh.cn

Go:   os.Exit(1)
来源：http://jf.newstarts.cn

Ruby: exit 1
来源：http://fc.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tw.gzmigu.cn

[M06] 向标准错误输出
来源：http://sy.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://tg.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dk.shtwfgs.cn

JS:   console.error("err")
来源：http://nx.huanxung.cn

TS:   console.error("err")
来源：http://lk.nszjky.cn

Java: System.err.println("err")
来源：http://ux.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tk.asd995.cn

Ruby: warn "err"
来源：http://iz.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://fc.asd995.cn

[M07] 判断是否为主入口
来源：http://qn.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://lx.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vs.hahajie.cn

JS:   require.main === module
来源：http://gy.huixiangedu.cn

TS:   require.main === module
来源：http://vz.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://bi.huixinmuqiang.cn

Go:   func main()
来源：http://mw.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://do.colortex.cn

C#:   static void Main(string[] args)
来源：http://dx.colortex.cn

[M08] 获取系统与运行时信息
来源：http://lv.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://un.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://ps.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://hl.9csxet.cn

TS:   process.platform;  process.version
来源：http://hj.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pq.muxihuayi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qa.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qb.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xl.nicolike.cn

================================================================================
来源：http://kh.bookmarksfly.cn

N. 数据结构与算法
来源：http://rd.shxzukj.cn

================================================================================
来源：http://tb.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://fo.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tl.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lq.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fh.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ze.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ux.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://bb.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nz.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ov.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://br.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://tr.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ff.colortex.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ql.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oe.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cz.shxzskj.cn

Go:   slices.Sort(arr)
来源：http://uo.huanxung.cn

Ruby: arr.sort
来源：http://gk.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lk.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://mr.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qq.huixinmuqiang.cn

PHP:  // 递归实现，或用 usort
来源：http://jg.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wp.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sz.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://na.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ay.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sn.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qu.shtwfgs.cn

[N04] 斐波那契数列
来源：http://kj.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://me.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cb.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rx.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ib.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pm.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bu.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aj.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zh.jctech888.com.cn

[N05] 最大公约数
来源：http://ay.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ay.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://je.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hv.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gx.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wb.huanxung.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wc.gzmigu.cn

Ruby: a.gcd(b)
来源：http://kk.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rt.shtwfgs.cn

[N06] 判断回文字符串
来源：http://wt.colortex.cn

Py:   s == s[::-1]
来源：http://jr.szsharing.cn

PHP:  $s === strrev($s);
来源：http://xi.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://vu.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://oc.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ua.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://nd.asd995.cn

Ruby: s == s.reverse
来源：http://xw.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wx.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://mx.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jb.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ie.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jw.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://ps.chemitech.net.cn

Java: // 手写 HashMap
来源：http://ff.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://la.szxytkj.cn

Ruby: // 手写 Hash
来源：http://hw.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wl.szxytkj.cn

[N08] 生成全排列
来源：http://yg.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ku.huanxung.cn

PHP:  // 手写递归交换
来源：http://pt.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://fc.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://rj.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://pc.asd995.cn

Go:   // 手写回溯递归
来源：http://sc.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://vm.shxzukj.cn

C#:   // 手写回溯递归
来源：http://au.szxytkj.cn

[N09] 栈与队列
来源：http://vp.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mt.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://me.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zq.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ub.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fc.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ek.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zf.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ee.shxzukj.cn

[N10] 链表节点定义
来源：http://yo.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://di.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rh.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jw.colortex.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cx.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://pr.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kh.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ia.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ar.nszjky.cn

[N11] 二叉树中序遍历
来源：http://en.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yq.521024.cn


<!-- 参考信息 -->