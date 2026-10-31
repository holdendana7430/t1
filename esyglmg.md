代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://gp.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hf.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://oj.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bq.szsharing.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ix.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lk.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dx.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wk.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zt.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ce.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rd.lnxyls.cn

[K05] 深拷贝对象
来源：http://ny.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://wh.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://yh.panjiajie.cn

JS:   structuredClone(obj)
来源：http://cn.hnjuh.cn

TS:   structuredClone(obj)
来源：http://so.panjiajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://od.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pi.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zd.huixinmuqiang.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rb.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://gm.asd995.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gy.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://su.nszjky.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yz.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yx.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ng.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ej.jianghongdianzi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qk.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qa.hahajie.cn

[K07] 进制转换
来源：http://lu.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rz.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gs.shxzukj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qx.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mh.chemitech.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kw.szxytkj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oz.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dl.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://co.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ww.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://js.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yu.lnxyls.cn

JS:   v8.serialize(obj)        // Node
来源：http://in.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://lv.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cy.jctech888.com.cn

Go:   encoding/gob
来源：http://vl.hnjuh.cn

Ruby: Marshal.dump(obj)
来源：http://pr.hahajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oo.asd995.cn

================================================================================
来源：http://fu.bjjhwx.cn

L. 网络请求
来源：http://oh.jctech888.com.cn

================================================================================
来源：http://nm.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://ev.nicolike.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bg.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wf.asd995.cn

JS:   await fetch(url)
来源：http://bh.nszjky.cn

TS:   await fetch(url)
来源：http://dm.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uu.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://lp.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://es.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xo.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://tt.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lp.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ie.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://az.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sh.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lj.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ym.gzmigu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sy.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tc.colortex.cn

[L03] 设置自定义请求头
来源：http://tf.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xi.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gv.huanxung.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eq.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bz.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rv.gzmigu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tm.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ta.huixinmuqiang.cn

[L04] 设置超时
来源：http://bb.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://ab.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xa.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uu.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://py.newstarts.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qq.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pt.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ti.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pt.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ka.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zl.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://su.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pk.yuntaijiaju.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wr.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sw.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rv.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xn.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vv.shxzskj.cn

[L06] 解析响应为 JSON
来源：http://mv.bookmarksfly.cn

Py:   resp.json()
来源：http://gx.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://wg.521024.cn

JS:   await resp.json()
来源：http://gm.nicolike.cn

TS:   await resp.json()
来源：http://ed.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://za.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ed.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://oc.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ze.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://zp.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ro.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ms.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://ah.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://zo.jctech888.com.cn

Java: resp.statusCode()
来源：http://ih.jctech888.com.cn

Go:   resp.StatusCode
来源：http://ng.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://xm.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://pz.shxzukj.cn

[L08] 并发请求多个地址
来源：http://hq.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ha.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://ns.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://je.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lu.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://az.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://si.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aa.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rv.haigaiapp.cn

================================================================================
来源：http://vg.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://se.hnjuh.cn

================================================================================
来源：http://ft.yuexingan06.cn

[M01] 读取命令行参数
来源：http://zi.huanxung.cn

Py:   sys.argv[1:]
来源：http://of.hahajie.cn

PHP:  $argv;  $argc;
来源：http://ku.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://eq.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://rw.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://rf.bookmarksfly.cn

Go:   os.Args[1:]
来源：http://cc.hnjuh.cn

Ruby: ARGV
来源：http://wy.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://xn.yuexingan06.cn

[M02] 读取环境变量
来源：http://xb.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://kc.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qt.shxzskj.cn

JS:   process.env.HOME
来源：http://lc.wgjwhj.cn

TS:   process.env.HOME
来源：http://xa.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ug.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jw.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ot.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ux.bjjhwx.cn

[M03] 执行外部命令
来源：http://tb.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ba.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tj.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wp.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nu.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fr.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oj.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mv.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://sv.szsharing.cn

[M04] 获取当前工作目录
来源：http://nw.hnjuh.cn

Py:   os.getcwd()
来源：http://pm.huanxung.cn

PHP:  getcwd();
来源：http://ih.colortex.cn

JS:   process.cwd()
来源：http://mg.chemitech.net.cn

TS:   process.cwd()
来源：http://wq.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://sr.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://il.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://qu.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ll.muxihuayi.cn

[M05] 设置退出码
来源：http://lk.lnxyls.cn

Py:   sys.exit(1)
来源：http://ru.hnjuh.cn

PHP:  exit(1);
来源：http://sa.panjiajie.cn

JS:   process.exit(1)
来源：http://fb.bjjhwx.cn

TS:   process.exit(1)
来源：http://fv.colortex.cn

Java: System.exit(1)
来源：http://cs.wgjwhj.cn

Go:   os.Exit(1)
来源：http://uf.nszjky.cn

Ruby: exit 1
来源：http://ds.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mn.colortex.cn

[M06] 向标准错误输出
来源：http://yv.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://kv.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qv.asd995.cn

JS:   console.error("err")
来源：http://tf.yuexingan06.cn

TS:   console.error("err")
来源：http://hk.hahajie.cn

Java: System.err.println("err")
来源：http://fz.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gf.yuexingan06.cn

Ruby: warn "err"
来源：http://oa.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://qo.colortex.cn

[M07] 判断是否为主入口
来源：http://cb.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://fp.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ue.szsharing.cn

JS:   require.main === module
来源：http://dy.shxzukj.cn

TS:   require.main === module
来源：http://yr.521024.cn

Java: public static void main(String[] args)
来源：http://iv.yuexingan06.cn

Go:   func main()
来源：http://ci.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jg.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://lf.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://nz.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://tg.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ec.shxzskj.cn

JS:   process.platform;  process.version
来源：http://ve.panjiajie.cn

TS:   process.platform;  process.version
来源：http://la.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yw.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xj.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uc.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eg.jctech888.com.cn

================================================================================
来源：http://ws.bookmarksfly.cn

N. 数据结构与算法
来源：http://ll.panjiajie.cn

================================================================================
来源：http://cg.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://if.shtwfgs.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zy.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://if.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jm.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dj.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oa.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://uk.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bz.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nz.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ai.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://if.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qh.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wm.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fg.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ae.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://sp.muxihuayi.cn

Ruby: arr.sort
来源：http://zv.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wy.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://wi.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fo.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://cl.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ip.newstarts.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ei.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rz.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ij.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wr.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://du.bjjhwx.cn

[N04] 斐波那契数列
来源：http://zd.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ws.shxzukj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sl.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://av.haigaiapp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://df.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jf.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xe.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oj.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aw.jctech888.com.cn

[N05] 最大公约数
来源：http://fw.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://yn.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://je.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zs.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vh.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wl.nicolike.cn

Ruby: a.gcd(b)
来源：http://hd.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bp.szsharing.cn

[N06] 判断回文字符串
来源：http://pf.bjjhwx.cn

Py:   s == s[::-1]
来源：http://ot.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://jf.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://rl.nszjky.cn

TS:   s === [...s].reverse().join("")
来源：http://qd.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dj.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://pc.shxzukj.cn

Ruby: s == s.reverse
来源：http://oy.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gv.hnjuh.cn

[N07] 两数之和（返回下标）
来源：http://az.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yq.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wn.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dp.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ig.gzmigu.cn

Java: // 手写 HashMap
来源：http://qy.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ms.huanxung.cn

Ruby: // 手写 Hash
来源：http://vl.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gn.haigaiapp.cn

[N08] 生成全排列
来源：http://zn.nszjky.cn

Py:   itertools.permutations(arr)
来源：http://ws.colortex.cn

PHP:  // 手写递归交换
来源：http://ii.521024.cn

JS:   // 手写回溯递归
来源：http://nq.hnjuh.cn

TS:   // 手写回溯递归
来源：http://pp.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://lt.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://na.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://yq.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://yl.gzmigu.cn

[N09] 栈与队列
来源：http://dq.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cp.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ca.szsharing.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jm.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rs.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fh.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hf.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://do.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mi.hahajie.cn

[N10] 链表节点定义
来源：http://kv.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lp.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qy.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uh.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ol.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://yt.wgjwhj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ya.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://by.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oj.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://na.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qx.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://mh.nicolike.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dl.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ez.szsharing.cn

Java: // 手写递归
来源：http://bl.bookmarksfly.cn

Go:   // 手写递归
来源：http://mh.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rm.szxytkj.cn

C#:   // 手写递归
来源：http://sf.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nu.chemitech.net.cn


<!-- 参考信息 -->