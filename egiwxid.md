代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cc.haigaiapp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xl.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mr.jctech888.com.cn

[K05] 深拷贝对象
来源：http://gx.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://kj.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://ci.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://vd.asd995.cn

TS:   structuredClone(obj)
来源：http://xk.huixiangedu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fa.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oi.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://px.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xw.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://bv.yuntaijiaju.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pi.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://po.bjjhwx.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ee.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qd.muxihuayi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://be.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kp.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ao.shxzukj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnjuh.cn

[K07] 进制转换
来源：http://ie.szsharing.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://az.wgjwhj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rq.szxytkj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qs.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://km.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lp.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fo.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ta.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ux.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://fs.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://ik.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://op.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://zi.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://it.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cf.jianghongdianzi.cn

Go:   encoding/gob
来源：http://uu.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://hx.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pj.nszjky.cn

================================================================================
来源：http://uz.huanxung.cn

L. 网络请求
来源：http://cv.521024.cn

================================================================================
来源：http://fg.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://jd.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rb.muxihuayi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xx.jianghongdianzi.cn

JS:   await fetch(url)
来源：http://mn.wgjwhj.cn

TS:   await fetch(url)
来源：http://gq.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hl.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://dt.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sz.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ek.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://ny.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qz.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xx.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cd.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wr.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ck.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nz.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rf.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uv.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ir.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xy.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://li.shxzukj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ta.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lv.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ta.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gr.haigaiapp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kv.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zp.hnjuh.cn

[L04] 设置超时
来源：http://gj.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://zq.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cc.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sj.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vc.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vr.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zo.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sp.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gl.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://rd.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ab.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fv.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pl.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ns.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lq.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://np.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uu.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xv.newstarts.cn

[L06] 解析响应为 JSON
来源：http://fr.panjiajie.cn

Py:   resp.json()
来源：http://rv.huanxung.cn

PHP:  json_decode($body, true);
来源：http://cu.shxzskj.cn

JS:   await resp.json()
来源：http://fl.szxytkj.cn

TS:   await resp.json()
来源：http://ra.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rr.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rh.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://sk.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qz.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://jc.huixiangedu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rf.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://mn.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://lz.panjiajie.cn

Java: resp.statusCode()
来源：http://ar.jctech888.com.cn

Go:   resp.StatusCode
来源：http://ws.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://xp.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://pi.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://tz.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://do.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://cn.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ve.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oh.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oy.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ju.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yx.jianghongdianzi.cn

================================================================================
来源：http://tl.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://cz.shxzukj.cn

================================================================================
来源：http://zw.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://tf.hnjuh.cn

Py:   sys.argv[1:]
来源：http://mf.yuexingan06.cn

PHP:  $argv;  $argc;
来源：http://pt.colortex.cn

JS:   process.argv.slice(2)
来源：http://br.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://ht.asd995.cn

Java: args 数组（main 方法参数）
来源：http://wt.9csxet.cn

Go:   os.Args[1:]
来源：http://wb.521024.cn

Ruby: ARGV
来源：http://nn.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://dp.521024.cn

[M02] 读取环境变量
来源：http://as.szxytkj.cn

Py:   os.environ.get("HOME")
来源：http://cb.shxzskj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jm.panjiajie.cn

JS:   process.env.HOME
来源：http://ix.panjiajie.cn

TS:   process.env.HOME
来源：http://xl.521024.cn

Java: System.getenv("HOME")
来源：http://ja.chemitech.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sa.9csxet.cn

Ruby: ENV["HOME"]
来源：http://wu.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ey.wgjwhj.cn

[M03] 执行外部命令
来源：http://po.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mn.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qb.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lx.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kw.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ri.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lz.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tg.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://dw.huanxung.cn

[M04] 获取当前工作目录
来源：http://qc.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://hb.hahajie.cn

PHP:  getcwd();
来源：http://bl.newstarts.cn

JS:   process.cwd()
来源：http://qe.colortex.cn

TS:   process.cwd()
来源：http://jw.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://vi.shxzukj.cn

Go:   os.Getwd()
来源：http://vh.muxihuayi.cn

Ruby: Dir.pwd
来源：http://xt.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qs.nszjky.cn

[M05] 设置退出码
来源：http://ut.panjiajie.cn

Py:   sys.exit(1)
来源：http://lp.bookmarksfly.cn

PHP:  exit(1);
来源：http://ea.szsharing.cn

JS:   process.exit(1)
来源：http://cc.jctech888.com.cn

TS:   process.exit(1)
来源：http://jq.newstarts.cn

Java: System.exit(1)
来源：http://bf.9csxet.cn

Go:   os.Exit(1)
来源：http://eu.chemitech.net.cn

Ruby: exit 1
来源：http://dk.huixinmuqiang.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gd.jctech888.com.cn

[M06] 向标准错误输出
来源：http://vo.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ib.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uq.huanxung.cn

JS:   console.error("err")
来源：http://wz.yuexingan06.cn

TS:   console.error("err")
来源：http://cl.lnxyls.cn

Java: System.err.println("err")
来源：http://cg.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uk.asd995.cn

Ruby: warn "err"
来源：http://xe.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://os.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://yh.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://cv.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vb.colortex.cn

JS:   require.main === module
来源：http://qx.9csxet.cn

TS:   require.main === module
来源：http://rc.szsharing.cn

Java: public static void main(String[] args)
来源：http://vm.yuexingan06.cn

Go:   func main()
来源：http://jz.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ic.szsharing.cn

C#:   static void Main(string[] args)
来源：http://cg.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://ze.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ag.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://ur.szsharing.cn

JS:   process.platform;  process.version
来源：http://qo.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://wt.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dw.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xp.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qw.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qp.bookmarksfly.cn

================================================================================
来源：http://mc.jianghongdianzi.cn

N. 数据结构与算法
来源：http://zs.szxytkj.cn

================================================================================
来源：http://ey.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://kk.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uu.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qe.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://um.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ox.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qq.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://dl.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hg.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nr.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://yu.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://no.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hj.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vy.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tw.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kh.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://rm.wgjwhj.cn

Ruby: arr.sort
来源：http://ra.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rw.colortex.cn

[N03] 快速排序（分治示例）
来源：http://jt.huixinmuqiang.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://of.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://cd.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xh.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vf.jctech888.com.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mm.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yn.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ol.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bl.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://uk.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pj.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rb.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://do.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gu.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vb.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vm.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ym.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zq.jianghongdianzi.cn

[N05] 最大公约数
来源：http://lx.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://bt.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ds.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nn.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dx.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ee.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jt.colortex.cn

Ruby: a.gcd(b)
来源：http://wf.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hi.huixiangedu.cn

[N06] 判断回文字符串
来源：http://um.newstarts.cn

Py:   s == s[::-1]
来源：http://pa.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://ty.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://od.hnjuh.cn

TS:   s === [...s].reverse().join("")
来源：http://xv.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sy.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://jm.asd995.cn

Ruby: s == s.reverse
来源：http://vt.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xr.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://do.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wg.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nh.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://od.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://fg.nszjky.cn

Java: // 手写 HashMap
来源：http://wo.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://ow.wgjwhj.cn

Ruby: // 手写 Hash
来源：http://vk.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xl.muxihuayi.cn

[N08] 生成全排列
来源：http://jg.521024.cn

Py:   itertools.permutations(arr)
来源：http://yb.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://zx.hnjuh.cn

JS:   // 手写回溯递归
来源：http://vn.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://ax.haigaiapp.cn

Java: // 手写回溯递归
来源：http://zk.shxzskj.cn

Go:   // 手写回溯递归
来源：http://gq.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://jy.szxytkj.cn

C#:   // 手写回溯递归
来源：http://kx.nicolike.cn

[N09] 栈与队列
来源：http://jq.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iy.newstarts.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xh.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yb.huanxung.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vu.haigaiapp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ws.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zf.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qf.panjiajie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ky.shxzukj.cn

[N10] 链表节点定义
来源：http://hi.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tg.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mb.huixinmuqiang.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dm.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hg.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://pg.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wv.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xr.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bc.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://ho.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ex.asd995.cn

PHP:  // 手写递归函数
来源：http://rh.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pu.521024.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sq.gzmigu.cn

Java: // 手写递归
来源：http://mh.panjiajie.cn

Go:   // 手写递归
来源：http://mc.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fl.shxzskj.cn

C#:   // 手写递归
来源：http://zh.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tc.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ju.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vv.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tf.chemitech.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xy.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zm.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hi.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dw.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dw.yuexingan06.cn


<!-- 参考信息 -->