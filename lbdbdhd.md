代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://go.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ei.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://tk.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://le.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zd.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eu.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mp.bjjhwx.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hn.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dy.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lf.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tj.chemitech.net.cn

[K05] 深拷贝对象
来源：http://qj.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://lz.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ih.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://to.asd995.cn

TS:   structuredClone(obj)
来源：http://mn.shtwfgs.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kr.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wu.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kx.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dk.yuntaijiaju.cn

[K06] 解析 URL 查询串
来源：http://za.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://al.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zv.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://om.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nr.9csxet.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ip.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://et.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ce.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yd.hnjuh.cn

[K07] 进制转换
来源：http://wn.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kp.bjjhwx.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jj.panjiajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fa.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xk.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qw.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ea.wgjwhj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bc.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vh.szxytkj.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://vh.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yk.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://rx.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://xz.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hs.colortex.cn

Go:   encoding/gob
来源：http://ow.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://va.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jx.haigaiapp.cn

================================================================================
来源：http://et.szsharing.cn

L. 网络请求
来源：http://hz.wgjwhj.cn

================================================================================
来源：http://gm.newstarts.cn

[L01] 发送 GET 请求
来源：http://rw.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oz.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xr.yuexingan06.cn

JS:   await fetch(url)
来源：http://oi.szsharing.cn

TS:   await fetch(url)
来源：http://uv.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sb.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://ks.szxytkj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vv.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://me.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://mz.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qh.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://il.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ex.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bw.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ei.nszjky.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ed.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gg.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://au.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://zb.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cq.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yk.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://il.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bg.bookmarksfly.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rp.haigaiapp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gi.yuexingan06.cn

[L04] 设置超时
来源：http://rb.lnxyls.cn

Py:   requests.get(url, timeout=5)
来源：http://uh.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tv.jianghongdianzi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kc.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://be.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sd.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ro.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ax.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mj.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://ef.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ru.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ci.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kq.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oj.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ti.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fi.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jb.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://am.521024.cn

[L06] 解析响应为 JSON
来源：http://xf.szxytkj.cn

Py:   resp.json()
来源：http://pf.nszjky.cn

PHP:  json_decode($body, true);
来源：http://qu.yuntaijiaju.cn

JS:   await resp.json()
来源：http://xa.shtwfgs.cn

TS:   await resp.json()
来源：http://cl.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gw.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mb.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://ax.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xf.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://by.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.panjiajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sp.colortex.cn

JS:   resp.ok;  resp.status
来源：http://td.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://xm.huanxung.cn

Java: resp.statusCode()
来源：http://kt.bjjhwx.cn

Go:   resp.StatusCode
来源：http://yk.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://to.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://si.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://fv.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tj.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://rl.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tq.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qx.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nd.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vk.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jj.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dy.colortex.cn

================================================================================
来源：http://qk.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://dz.szsharing.cn

================================================================================
来源：http://ja.haigaiapp.cn

[M01] 读取命令行参数
来源：http://wn.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://pq.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://rj.asd995.cn

JS:   process.argv.slice(2)
来源：http://mn.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ph.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://lt.szxytkj.cn

Go:   os.Args[1:]
来源：http://zs.szxytkj.cn

Ruby: ARGV
来源：http://ky.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://yk.nicolike.cn

[M02] 读取环境变量
来源：http://ik.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://zk.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zz.asd995.cn

JS:   process.env.HOME
来源：http://ka.huixinmuqiang.cn

TS:   process.env.HOME
来源：http://yn.nszjky.cn

Java: System.getenv("HOME")
来源：http://ab.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lp.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://kd.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kw.shxzskj.cn

[M03] 执行外部命令
来源：http://vc.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mi.jianghongdianzi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kg.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ut.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mq.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hn.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kv.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ko.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://oe.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://qt.jctech888.com.cn

Py:   os.getcwd()
来源：http://wq.panjiajie.cn

PHP:  getcwd();
来源：http://ty.521024.cn

JS:   process.cwd()
来源：http://or.hahajie.cn

TS:   process.cwd()
来源：http://bs.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://ik.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ub.9csxet.cn

Ruby: Dir.pwd
来源：http://gf.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://us.chemitech.net.cn

[M05] 设置退出码
来源：http://eh.nicolike.cn

Py:   sys.exit(1)
来源：http://vj.panjiajie.cn

PHP:  exit(1);
来源：http://uv.shtwfgs.cn

JS:   process.exit(1)
来源：http://jo.9csxet.cn

TS:   process.exit(1)
来源：http://mf.huanxung.cn

Java: System.exit(1)
来源：http://nz.nicolike.cn

Go:   os.Exit(1)
来源：http://db.521024.cn

Ruby: exit 1
来源：http://ok.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hi.gzmigu.cn

[M06] 向标准错误输出
来源：http://ld.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://ub.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zv.jianghongdianzi.cn

JS:   console.error("err")
来源：http://yp.shxzukj.cn

TS:   console.error("err")
来源：http://vy.shxzskj.cn

Java: System.err.println("err")
来源：http://jk.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://od.yuntaijiaju.cn

Ruby: warn "err"
来源：http://og.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://ux.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://xu.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://nx.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qv.hahajie.cn

JS:   require.main === module
来源：http://vs.hnjuh.cn

TS:   require.main === module
来源：http://ij.nszjky.cn

Java: public static void main(String[] args)
来源：http://bs.szxytkj.cn

Go:   func main()
来源：http://ye.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://va.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://my.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://jr.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://un.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://gz.shxzukj.cn

JS:   process.platform;  process.version
来源：http://np.huanxung.cn

TS:   process.platform;  process.version
来源：http://rw.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xn.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://at.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://an.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jv.lnxyls.cn

================================================================================
来源：http://io.bookmarksfly.cn

N. 数据结构与算法
来源：http://zw.asd995.cn

================================================================================
来源：http://gs.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://hr.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qd.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://op.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uq.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://of.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bg.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://re.asd995.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jd.521024.cn

C#:   Array.BinarySearch(arr, x)
来源：http://np.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://zc.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://we.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ie.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://do.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uy.521024.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ry.9csxet.cn

Go:   slices.Sort(arr)
来源：http://ax.yuntaijiaju.cn

Ruby: arr.sort
来源：http://se.nicolike.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ga.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://wp.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rl.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://be.haigaiapp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://st.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wf.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gb.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bx.newstarts.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tg.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hs.shxzskj.cn

[N04] 斐波那契数列
来源：http://iy.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ww.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tz.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vj.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fc.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kq.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tz.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wt.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ao.szxytkj.cn

[N05] 最大公约数
来源：http://ey.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://ab.colortex.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gw.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rl.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iu.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lj.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nu.nszjky.cn

Ruby: a.gcd(b)
来源：http://ih.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hw.shxzskj.cn

[N06] 判断回文字符串
来源：http://yx.wgjwhj.cn

Py:   s == s[::-1]
来源：http://ms.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://am.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://dq.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://ue.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gk.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ki.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://vd.bjjhwx.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zb.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://pa.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uk.muxihuayi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bz.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zh.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://oz.521024.cn

Java: // 手写 HashMap
来源：http://gz.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://we.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://gi.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ym.shxzskj.cn

[N08] 生成全排列
来源：http://yf.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://so.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://gn.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://lo.shxzukj.cn

TS:   // 手写回溯递归
来源：http://mn.huixiangedu.cn

Java: // 手写回溯递归
来源：http://ht.huanxung.cn

Go:   // 手写回溯递归
来源：http://od.jianghongdianzi.cn

Ruby: arr.permutation.to_a
来源：http://zz.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://pz.521024.cn

[N09] 栈与队列
来源：http://pw.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fs.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lm.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bp.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uw.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zk.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hn.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ve.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jb.9csxet.cn

[N10] 链表节点定义
来源：http://ue.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ay.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fo.jianghongdianzi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://st.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://el.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://tp.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wo.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oa.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xv.huanxung.cn

[N11] 二叉树中序遍历
来源：http://sg.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kb.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://vv.colortex.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rf.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.yuexingan06.cn

Java: // 手写递归
来源：http://du.huixinmuqiang.cn

Go:   // 手写递归
来源：http://eu.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zu.panjiajie.cn

C#:   // 手写递归
来源：http://jb.9csxet.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hk.huixinmuqiang.cn


<!-- 参考信息 -->