代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://rn.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://io.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sl.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nw.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dy.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://md.wgjwhj.cn

[K04] 读取 JSON 文件
来源：http://ha.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jo.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wc.nszjky.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cn.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xj.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yo.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kh.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qg.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hl.chemitech.net.cn

[K05] 深拷贝对象
来源：http://bw.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://in.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://lj.asd995.cn

JS:   structuredClone(obj)
来源：http://uq.colortex.cn

TS:   structuredClone(obj)
来源：http://vc.yuexingan06.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xt.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yq.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bb.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xu.muxihuayi.cn

[K06] 解析 URL 查询串
来源：http://cz.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yx.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fu.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ic.shtwfgs.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zt.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yw.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rk.nicolike.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://us.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ln.lnxyls.cn

[K07] 进制转换
来源：http://nh.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ej.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mn.9csxet.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eh.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mz.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kp.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nj.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yl.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rs.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://yd.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://vj.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sm.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://le.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://ra.chemitech.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://on.shxzskj.cn

Go:   encoding/gob
来源：http://ly.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://ps.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kl.huixinmuqiang.cn

================================================================================
来源：http://nb.bjjhwx.cn

L. 网络请求
来源：http://jg.jctech888.com.cn

================================================================================
来源：http://jc.nszjky.cn

[L01] 发送 GET 请求
来源：http://jn.colortex.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://io.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ob.muxihuayi.cn

JS:   await fetch(url)
来源：http://lw.szxytkj.cn

TS:   await fetch(url)
来源：http://xf.chemitech.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tq.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://mw.hnjuh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hu.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cc.szxytkj.cn

[L02] 发送 POST JSON
来源：http://ge.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://re.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mz.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kn.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tg.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wo.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://np.wgjwhj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xy.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://do.nszjky.cn

[L03] 设置自定义请求头
来源：http://sq.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qi.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pg.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ot.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qi.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eg.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rj.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vh.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bg.gzmigu.cn

[L04] 设置超时
来源：http://sd.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://rd.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://an.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yb.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ra.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zz.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ix.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aj.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tl.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://oj.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ri.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xi.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lg.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hi.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fu.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rn.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ls.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mu.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://wu.haigaiapp.cn

Py:   resp.json()
来源：http://pw.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://bu.shtwfgs.cn

JS:   await resp.json()
来源：http://im.yuntaijiaju.cn

TS:   await resp.json()
来源：http://wj.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wu.haigaiapp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ww.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://fu.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jj.nszjky.cn

[L07] 处理 HTTP 状态码
来源：http://tx.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xh.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nr.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://qw.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://vi.huixiangedu.cn

Java: resp.statusCode()
来源：http://jk.muxihuayi.cn

Go:   resp.StatusCode
来源：http://bf.asd995.cn

Ruby: resp.code.to_i
来源：http://cf.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://fl.szxytkj.cn

[L08] 并发请求多个地址
来源：http://ms.lnxyls.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rz.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://kh.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fo.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vu.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vs.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fd.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://af.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dz.haigaiapp.cn

================================================================================
来源：http://ns.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://mc.521024.cn

================================================================================
来源：http://dl.nicolike.cn

[M01] 读取命令行参数
来源：http://tb.shxzskj.cn

Py:   sys.argv[1:]
来源：http://wm.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://br.nszjky.cn

JS:   process.argv.slice(2)
来源：http://tk.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://xt.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://ln.muxihuayi.cn

Go:   os.Args[1:]
来源：http://nc.lnxyls.cn

Ruby: ARGV
来源：http://ds.panjiajie.cn

C#:   args 数组（Main 方法参数）
来源：http://xq.muxihuayi.cn

[M02] 读取环境变量
来源：http://cx.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://bp.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jg.szxytkj.cn

JS:   process.env.HOME
来源：http://ek.asd995.cn

TS:   process.env.HOME
来源：http://sn.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://bm.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gp.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://zj.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pi.muxihuayi.cn

[M03] 执行外部命令
来源：http://lp.haigaiapp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hr.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rx.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xg.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ia.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jt.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lz.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ss.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://md.szsharing.cn

[M04] 获取当前工作目录
来源：http://hk.hahajie.cn

Py:   os.getcwd()
来源：http://hg.nicolike.cn

PHP:  getcwd();
来源：http://sw.shxzukj.cn

JS:   process.cwd()
来源：http://mn.lnxyls.cn

TS:   process.cwd()
来源：http://aw.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://hm.lnxyls.cn

Go:   os.Getwd()
来源：http://pg.shxzskj.cn

Ruby: Dir.pwd
来源：http://yn.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ii.huixiangedu.cn

[M05] 设置退出码
来源：http://ac.huixiangedu.cn

Py:   sys.exit(1)
来源：http://zu.huixiangedu.cn

PHP:  exit(1);
来源：http://gm.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://cp.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://sp.panjiajie.cn

Java: System.exit(1)
来源：http://ap.szxytkj.cn

Go:   os.Exit(1)
来源：http://tt.nicolike.cn

Ruby: exit 1
来源：http://ir.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ss.9csxet.cn

[M06] 向标准错误输出
来源：http://se.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://oc.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rz.panjiajie.cn

JS:   console.error("err")
来源：http://vz.yuntaijiaju.cn

TS:   console.error("err")
来源：http://qy.szsharing.cn

Java: System.err.println("err")
来源：http://uz.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gn.huanxung.cn

Ruby: warn "err"
来源：http://qf.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ge.9csxet.cn

[M07] 判断是否为主入口
来源：http://mi.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://wj.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ej.colortex.cn

JS:   require.main === module
来源：http://jh.huixiangedu.cn

TS:   require.main === module
来源：http://kc.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://ea.bjjhwx.cn

Go:   func main()
来源：http://rx.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uu.huanxung.cn

C#:   static void Main(string[] args)
来源：http://gd.wgjwhj.cn

[M08] 获取系统与运行时信息
来源：http://fe.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://gf.huanxung.cn

PHP:  PHP_OS;  phpversion();
来源：http://ew.szxytkj.cn

JS:   process.platform;  process.version
来源：http://kg.nicolike.cn

TS:   process.platform;  process.version
来源：http://xz.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rl.newstarts.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jk.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lv.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vs.bookmarksfly.cn

================================================================================
来源：http://er.nicolike.cn

N. 数据结构与算法
来源：http://my.muxihuayi.cn

================================================================================
来源：http://gf.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://ek.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gt.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xx.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bf.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tl.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://is.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://sb.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xy.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oj.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://tm.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jq.wgjwhj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pg.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ha.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xi.asd995.cn

Go:   slices.Sort(arr)
来源：http://au.9csxet.cn

Ruby: arr.sort
来源：http://rm.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oi.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://dp.wgjwhj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yl.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://vl.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rh.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://az.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://so.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://as.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ic.muxihuayi.cn

[N04] 斐波那契数列
来源：http://qu.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ge.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qd.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sq.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rg.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://su.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vn.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rb.szxytkj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sx.huixinmuqiang.cn

[N05] 最大公约数
来源：http://tk.colortex.cn

Py:   math.gcd(a, b)
来源：http://kq.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uy.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sp.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pz.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ty.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kz.nicolike.cn

Ruby: a.gcd(b)
来源：http://ja.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hy.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://ec.nicolike.cn

Py:   s == s[::-1]
来源：http://td.9csxet.cn

PHP:  $s === strrev($s);
来源：http://vb.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://vk.asd995.cn

TS:   s === [...s].reverse().join("")
来源：http://it.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qk.nicolike.cn

Go:   // 双指针从两端比较
来源：http://qd.wgjwhj.cn

Ruby: s == s.reverse
来源：http://xm.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vt.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://yo.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://my.szxytkj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://po.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://er.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://nb.colortex.cn

Java: // 手写 HashMap
来源：http://mt.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://bh.asd995.cn

Ruby: // 手写 Hash
来源：http://ts.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pj.chemitech.net.cn

[N08] 生成全排列
来源：http://tp.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://xe.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ni.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://hh.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://gf.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://om.huanxung.cn

Go:   // 手写回溯递归
来源：http://cg.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://ff.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://jf.szsharing.cn

[N09] 栈与队列
来源：http://os.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uo.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://le.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ko.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lc.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bj.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vl.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://du.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rr.gzmigu.cn

[N10] 链表节点定义
来源：http://zw.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ta.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bz.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dt.hnjuh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bh.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://eq.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hi.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://it.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sa.huanxung.cn

[N11] 二叉树中序遍历
来源：http://gm.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cd.9csxet.cn

PHP:  // 手写递归函数
来源：http://pd.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lz.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fh.huixinmuqiang.cn

Java: // 手写递归
来源：http://xa.nicolike.cn


<!-- 参考信息 -->