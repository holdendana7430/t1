代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yn.yuexingan06.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xb.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tl.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pc.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://df.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oi.shxzukj.cn

[K05] 深拷贝对象
来源：http://xg.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://oo.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://rn.huanxung.cn

JS:   structuredClone(obj)
来源：http://ml.hnjuh.cn

TS:   structuredClone(obj)
来源：http://nq.chemitech.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rb.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gt.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ks.gzmigu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://op.jctech888.com.cn

[K06] 解析 URL 查询串
来源：http://lw.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ki.yuexingan06.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xl.colortex.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rj.nszjky.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uc.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cb.521024.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sx.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hf.huixiangedu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nj.szxytkj.cn

[K07] 进制转换
来源：http://wl.9csxet.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hx.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://te.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bi.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://li.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ya.huixiangedu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hp.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ys.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://do.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://za.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://cw.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oh.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://cm.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://fu.shtwfgs.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iy.huixinmuqiang.cn

Go:   encoding/gob
来源：http://cl.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://qq.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uk.shxzskj.cn

================================================================================
来源：http://zd.gzmigu.cn

L. 网络请求
来源：http://aa.bookmarksfly.cn

================================================================================
来源：http://zr.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://ta.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://js.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://am.bjjhwx.cn

JS:   await fetch(url)
来源：http://cw.muxihuayi.cn

TS:   await fetch(url)
来源：http://az.yuntaijiaju.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ia.szsharing.cn

Go:   resp, err := http.Get(url)
来源：http://bt.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ak.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ku.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://di.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hi.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hr.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jw.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fg.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gk.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kp.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://un.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://me.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://uh.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ai.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ze.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dg.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ge.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gb.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://no.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ez.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tf.asd995.cn

[L04] 设置超时
来源：http://jg.521024.cn

Py:   requests.get(url, timeout=5)
来源：http://zz.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ay.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jp.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ge.shtwfgs.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hp.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ce.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zg.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://do.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://dy.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ag.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ce.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bs.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fd.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://no.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zv.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hq.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ye.nszjky.cn

[L06] 解析响应为 JSON
来源：http://mj.jianghongdianzi.cn

Py:   resp.json()
来源：http://dr.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://dq.bjjhwx.cn

JS:   await resp.json()
来源：http://bp.huixiangedu.cn

TS:   await resp.json()
来源：http://jm.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xx.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sc.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://jf.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nk.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://gn.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qb.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kw.asd995.cn

JS:   resp.ok;  resp.status
来源：http://tg.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://ha.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://zy.jctech888.com.cn

Go:   resp.StatusCode
来源：http://co.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://ya.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://sg.colortex.cn

[L08] 并发请求多个地址
来源：http://rw.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hi.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://hn.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://na.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iu.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mh.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vy.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zc.nicolike.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wq.colortex.cn

================================================================================
来源：http://uq.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://dy.huixiangedu.cn

================================================================================
来源：http://zv.yuexingan06.cn

[M01] 读取命令行参数
来源：http://oq.huanxung.cn

Py:   sys.argv[1:]
来源：http://oc.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://xq.nszjky.cn

JS:   process.argv.slice(2)
来源：http://mk.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://it.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://aq.shtwfgs.cn

Go:   os.Args[1:]
来源：http://nu.9csxet.cn

Ruby: ARGV
来源：http://we.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://up.wgjwhj.cn

[M02] 读取环境变量
来源：http://pt.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://zk.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pa.shtwfgs.cn

JS:   process.env.HOME
来源：http://gc.nicolike.cn

TS:   process.env.HOME
来源：http://is.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://zm.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://so.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://xc.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kr.szsharing.cn

[M03] 执行外部命令
来源：http://wx.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zp.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nn.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rm.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dh.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://os.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ku.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ww.shxzskj.cn

C#:   Process.Start("ls", "-l");
来源：http://dq.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://xu.lnxyls.cn

Py:   os.getcwd()
来源：http://zl.521024.cn

PHP:  getcwd();
来源：http://ds.haigaiapp.cn

JS:   process.cwd()
来源：http://he.gzmigu.cn

TS:   process.cwd()
来源：http://wp.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://kz.panjiajie.cn

Go:   os.Getwd()
来源：http://zf.chemitech.net.cn

Ruby: Dir.pwd
来源：http://pg.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rz.muxihuayi.cn

[M05] 设置退出码
来源：http://rh.szxytkj.cn

Py:   sys.exit(1)
来源：http://ri.shtwfgs.cn

PHP:  exit(1);
来源：http://wi.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://im.huanxung.cn

TS:   process.exit(1)
来源：http://oc.nicolike.cn

Java: System.exit(1)
来源：http://bj.shxzskj.cn

Go:   os.Exit(1)
来源：http://ta.yuexingan06.cn

Ruby: exit 1
来源：http://ip.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jf.bjjhwx.cn

[M06] 向标准错误输出
来源：http://el.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://uj.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cy.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ll.lnxyls.cn

TS:   console.error("err")
来源：http://yj.bjjhwx.cn

Java: System.err.println("err")
来源：http://hp.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wu.shxzukj.cn

Ruby: warn "err"
来源：http://zd.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://pi.newstarts.cn

[M07] 判断是否为主入口
来源：http://sh.asd995.cn

Py:   if __name__ == "__main__":
来源：http://hw.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vn.bookmarksfly.cn

JS:   require.main === module
来源：http://or.muxihuayi.cn

TS:   require.main === module
来源：http://yg.hnjuh.cn

Java: public static void main(String[] args)
来源：http://zi.shtwfgs.cn

Go:   func main()
来源：http://iu.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cd.nszjky.cn

C#:   static void Main(string[] args)
来源：http://sd.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://bx.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://nb.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://az.9csxet.cn

JS:   process.platform;  process.version
来源：http://xz.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://on.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lt.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ov.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bb.panjiajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yo.hahajie.cn

================================================================================
来源：http://rc.colortex.cn

N. 数据结构与算法
来源：http://zo.nszjky.cn

================================================================================
来源：http://en.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://to.huixinmuqiang.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sw.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sm.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fg.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hy.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://et.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://ax.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://la.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sh.jctech888.com.cn

[N02] 排序（工程实践用内置实现）
来源：http://pv.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://yg.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dt.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aq.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zr.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zn.newstarts.cn

Go:   slices.Sort(arr)
来源：http://dz.bookmarksfly.cn

Ruby: arr.sort
来源：http://xa.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://om.huanxung.cn

[N03] 快速排序（分治示例）
来源：http://qd.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tu.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://op.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oy.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://en.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iy.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gb.bookmarksfly.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dt.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://di.panjiajie.cn

[N04] 斐波那契数列
来源：http://jn.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gw.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gd.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yp.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jp.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xi.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rs.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kz.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nm.hnjuh.cn

[N05] 最大公约数
来源：http://dd.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://tj.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bg.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ff.muxihuayi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vo.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ha.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://il.newstarts.cn

Ruby: a.gcd(b)
来源：http://kn.shxzskj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uy.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://lv.shtwfgs.cn

Py:   s == s[::-1]
来源：http://gd.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://tb.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://wl.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://qj.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nt.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://gr.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://sn.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kj.colortex.cn

[N07] 两数之和（返回下标）
来源：http://it.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kf.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rt.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ak.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://mo.panjiajie.cn

Java: // 手写 HashMap
来源：http://zn.colortex.cn

Go:   // 手写 map[int]int
来源：http://ox.nszjky.cn

Ruby: // 手写 Hash
来源：http://fl.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://si.shxzskj.cn

[N08] 生成全排列
来源：http://pt.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://fe.shxzukj.cn

PHP:  // 手写递归交换
来源：http://en.nszjky.cn

JS:   // 手写回溯递归
来源：http://tz.huanxung.cn

TS:   // 手写回溯递归
来源：http://oe.muxihuayi.cn

Java: // 手写回溯递归
来源：http://lq.hnjuh.cn

Go:   // 手写回溯递归
来源：http://dm.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://fg.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://ma.yuexingan06.cn

[N09] 栈与队列
来源：http://ss.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pv.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pq.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aj.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mw.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ul.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pu.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uz.huixiangedu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kt.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://pk.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jz.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://he.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ho.huanxung.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yw.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://ph.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bz.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wu.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ya.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://hx.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://za.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://fz.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bp.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wl.jctech888.com.cn

Java: // 手写递归
来源：http://bi.szxytkj.cn

Go:   // 手写递归
来源：http://be.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sy.521024.cn

C#:   // 手写递归
来源：http://nn.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qx.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vl.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dl.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xs.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://va.hahajie.cn


<!-- 参考信息 -->