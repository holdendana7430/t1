代发 wailian999

[K06] 解析 URL 查询串
来源：http://xi.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zw.hahajie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://go.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ke.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gs.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nz.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yo.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ul.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bg.haigaiapp.cn

[K07] 进制转换
来源：http://er.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wc.colortex.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://se.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wv.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://io.wgjwhj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qa.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ge.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fr.hahajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sj.bookmarksfly.cn

[K08] 二进制序列化（非 JSON）
来源：http://qh.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://yx.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tp.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://cp.gzmigu.cn

TS:   v8.serialize(obj)        // Node
来源：http://iz.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zj.wgjwhj.cn

Go:   encoding/gob
来源：http://uz.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://pr.nszjky.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jc.hahajie.cn

================================================================================
来源：http://kj.yuntaijiaju.cn

L. 网络请求
来源：http://jc.bookmarksfly.cn

================================================================================
来源：http://ck.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://yi.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mw.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qj.521024.cn

JS:   await fetch(url)
来源：http://eb.panjiajie.cn

TS:   await fetch(url)
来源：http://uc.haigaiapp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pl.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://hl.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tj.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ru.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ol.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://py.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qb.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wu.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xa.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ng.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nv.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ku.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vn.nszjky.cn

[L03] 设置自定义请求头
来源：http://tz.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fg.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dv.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bn.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kd.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ug.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rv.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aa.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dd.chemitech.net.cn

[L04] 设置超时
来源：http://rp.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://vb.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uo.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ss.jianghongdianzi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ef.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bs.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lr.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jk.panjiajie.cn

[L05] 上传文件（multipart）
来源：http://yv.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zp.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xk.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bw.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ot.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vr.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ey.bookmarksfly.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rh.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://op.521024.cn

[L06] 解析响应为 JSON
来源：http://ks.huixinmuqiang.cn

Py:   resp.json()
来源：http://kh.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://ra.huixiangedu.cn

JS:   await resp.json()
来源：http://om.panjiajie.cn

TS:   await resp.json()
来源：http://gx.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mg.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ti.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://eh.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qb.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ei.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://je.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sl.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://nt.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://jm.muxihuayi.cn

Java: resp.statusCode()
来源：http://pj.shtwfgs.cn

Go:   resp.StatusCode
来源：http://ym.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://gs.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://np.newstarts.cn

[L08] 并发请求多个地址
来源：http://ym.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iv.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://sm.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xt.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ej.gzmigu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qy.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wc.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jn.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ws.hahajie.cn

================================================================================
来源：http://dc.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://ol.9csxet.cn

================================================================================
来源：http://jq.jctech888.com.cn

[M01] 读取命令行参数
来源：http://ew.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://sj.hahajie.cn

PHP:  $argv;  $argc;
来源：http://cy.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://oq.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://am.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://qz.521024.cn

Go:   os.Args[1:]
来源：http://pw.huanxung.cn

Ruby: ARGV
来源：http://mx.jctech888.com.cn

C#:   args 数组（Main 方法参数）
来源：http://fz.shxzskj.cn

[M02] 读取环境变量
来源：http://vc.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://uf.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bk.asd995.cn

JS:   process.env.HOME
来源：http://bc.asd995.cn

TS:   process.env.HOME
来源：http://eg.lnxyls.cn

Java: System.getenv("HOME")
来源：http://av.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xy.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://ms.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ca.wgjwhj.cn

[M03] 执行外部命令
来源：http://za.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gz.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iu.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zd.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uf.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dj.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vf.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uh.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://jh.panjiajie.cn

[M04] 获取当前工作目录
来源：http://rc.9csxet.cn

Py:   os.getcwd()
来源：http://dl.chemitech.net.cn

PHP:  getcwd();
来源：http://hk.wgjwhj.cn

JS:   process.cwd()
来源：http://wp.521024.cn

TS:   process.cwd()
来源：http://gn.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pg.chemitech.net.cn

Go:   os.Getwd()
来源：http://qp.jctech888.com.cn

Ruby: Dir.pwd
来源：http://mh.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ia.jianghongdianzi.cn

[M05] 设置退出码
来源：http://ya.huanxung.cn

Py:   sys.exit(1)
来源：http://gm.9csxet.cn

PHP:  exit(1);
来源：http://ms.huanxung.cn

JS:   process.exit(1)
来源：http://xc.hnjuh.cn

TS:   process.exit(1)
来源：http://bs.hahajie.cn

Java: System.exit(1)
来源：http://ex.panjiajie.cn

Go:   os.Exit(1)
来源：http://fv.bjjhwx.cn

Ruby: exit 1
来源：http://gs.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pq.huanxung.cn

[M06] 向标准错误输出
来源：http://kv.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://wv.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tu.hahajie.cn

JS:   console.error("err")
来源：http://tc.huixinmuqiang.cn

TS:   console.error("err")
来源：http://vm.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ph.yuexingan06.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mo.newstarts.cn

Ruby: warn "err"
来源：http://vt.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://gs.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ko.nicolike.cn

Py:   if __name__ == "__main__":
来源：http://qq.lnxyls.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://to.shtwfgs.cn

JS:   require.main === module
来源：http://fa.9csxet.cn

TS:   require.main === module
来源：http://im.nszjky.cn

Java: public static void main(String[] args)
来源：http://qm.newstarts.cn

Go:   func main()
来源：http://og.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uq.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://fr.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://zc.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://ns.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ou.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://cr.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://rt.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://is.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vz.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cz.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qu.shtwfgs.cn

================================================================================
来源：http://en.szxytkj.cn

N. 数据结构与算法
来源：http://vw.hahajie.cn

================================================================================
来源：http://sg.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://fh.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ah.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://et.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://us.huixiangedu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ul.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nh.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://zj.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dv.huanxung.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bw.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://ye.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ll.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wf.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cm.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hh.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jg.hahajie.cn

Go:   slices.Sort(arr)
来源：http://dl.newstarts.cn

Ruby: arr.sort
来源：http://vv.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cp.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://fx.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ob.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://wn.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tc.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ba.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lx.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uf.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cd.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hr.shxzukj.cn

[N04] 斐波那契数列
来源：http://tv.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fi.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ts.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.jctech888.com.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://un.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zn.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wb.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cz.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dg.nicolike.cn

[N05] 最大公约数
来源：http://kw.521024.cn

Py:   math.gcd(a, b)
来源：http://jt.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xz.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aw.jctech888.com.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gg.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sx.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wz.huixiangedu.cn

Ruby: a.gcd(b)
来源：http://de.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://il.nicolike.cn

[N06] 判断回文字符串
来源：http://bu.muxihuayi.cn

Py:   s == s[::-1]
来源：http://xl.hahajie.cn

PHP:  $s === strrev($s);
来源：http://rv.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://in.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://bj.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rh.asd995.cn

Go:   // 双指针从两端比较
来源：http://hd.huixinmuqiang.cn

Ruby: s == s.reverse
来源：http://ro.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cd.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://lm.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rx.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bh.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yf.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://er.szxytkj.cn

Java: // 手写 HashMap
来源：http://bf.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://ml.nicolike.cn

Ruby: // 手写 Hash
来源：http://ez.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ys.huixinmuqiang.cn

[N08] 生成全排列
来源：http://md.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://fw.hnjuh.cn

PHP:  // 手写递归交换
来源：http://ff.nszjky.cn

JS:   // 手写回溯递归
来源：http://ff.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://fx.wgjwhj.cn

Java: // 手写回溯递归
来源：http://rk.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://vz.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://yx.jianghongdianzi.cn

C#:   // 手写回溯递归
来源：http://md.hnjuh.cn

[N09] 栈与队列
来源：http://uo.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://my.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iz.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wb.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pk.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yb.muxihuayi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jl.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bz.bookmarksfly.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pa.muxihuayi.cn

[N10] 链表节点定义
来源：http://lu.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jx.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zv.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ed.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dv.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://wh.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://re.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xj.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rj.lnxyls.cn

[N11] 二叉树中序遍历
来源：http://sd.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ql.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://ip.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cv.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ig.szsharing.cn

Java: // 手写递归
来源：http://vl.asd995.cn

Go:   // 手写递归
来源：http://gd.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eb.panjiajie.cn

C#:   // 手写递归
来源：http://iz.gzmigu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rd.huixiangedu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ih.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ra.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cl.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sp.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vp.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dn.huixiangedu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cq.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rs.muxihuayi.cn

================================================================================
来源：http://ot.muxihuayi.cn

O. 并发与异步
来源：http://um.lnxyls.cn

================================================================================
来源：http://kb.lnxyls.cn

[O01] 启动一个线程
来源：http://jt.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nd.521024.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cv.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mb.muxihuayi.cn

TS:   // 同 JS
来源：http://vw.bookmarksfly.cn

Java: new Thread(() -> f()).start()
来源：http://yx.panjiajie.cn

Go:   go f()
来源：http://zl.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://eh.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://rz.panjiajie.cn


<!-- 参考信息 -->