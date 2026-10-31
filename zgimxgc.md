代发 wailian999

[K06] 解析 URL 查询串
来源：http://ln.newstarts.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rr.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ks.hahajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yt.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pk.newstarts.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rk.szsharing.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qk.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uj.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mu.asd995.cn

[K07] 进制转换
来源：http://le.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gf.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zt.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://io.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oz.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bq.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vg.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ss.nicolike.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://it.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://br.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://kr.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mz.szsharing.cn

JS:   v8.serialize(obj)        // Node
来源：http://lk.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://ua.9csxet.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hy.gzmigu.cn

Go:   encoding/gob
来源：http://kc.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://ro.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://td.nicolike.cn

================================================================================
来源：http://bx.shxzukj.cn

L. 网络请求
来源：http://sx.bookmarksfly.cn

================================================================================
来源：http://jb.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://dc.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qw.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cp.yuexingan06.cn

JS:   await fetch(url)
来源：http://br.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://bk.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://el.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://bl.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zk.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hx.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://oo.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wq.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ue.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://px.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sp.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vl.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sp.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mr.bookmarksfly.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ru.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://lo.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sm.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ya.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gf.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zs.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zv.szxytkj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bs.huixiangedu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hg.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dd.bookmarksfly.cn

[L04] 设置超时
来源：http://ru.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://pq.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yh.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ny.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://na.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gv.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ur.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://io.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wi.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://hh.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ca.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eg.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ff.haigaiapp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cq.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sz.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dz.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tp.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ap.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://sn.huixinmuqiang.cn

Py:   resp.json()
来源：http://vl.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://tx.yuntaijiaju.cn

JS:   await resp.json()
来源：http://tu.nszjky.cn

TS:   await resp.json()
来源：http://ur.nszjky.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jd.bookmarksfly.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fi.521024.cn

Ruby: JSON.parse(resp.body)
来源：http://iq.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ya.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://ax.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kz.yuexingan06.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zk.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://an.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://tg.hnjuh.cn

Java: resp.statusCode()
来源：http://go.shtwfgs.cn

Go:   resp.StatusCode
来源：http://rn.nicolike.cn

Ruby: resp.code.to_i
来源：http://gl.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://bx.shxzskj.cn

[L08] 并发请求多个地址
来源：http://qz.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zk.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://dq.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wi.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kj.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cc.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bi.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gz.nszjky.cn

================================================================================
来源：http://el.521024.cn

M. 命令行 / 进程 / 环境
来源：http://xq.chemitech.net.cn

================================================================================
来源：http://uw.521024.cn

[M01] 读取命令行参数
来源：http://cf.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://bb.asd995.cn

PHP:  $argv;  $argc;
来源：http://ay.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://kd.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://xq.521024.cn

Java: args 数组（main 方法参数）
来源：http://ke.newstarts.cn

Go:   os.Args[1:]
来源：http://ca.huixiangedu.cn

Ruby: ARGV
来源：http://jp.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://bq.chemitech.net.cn

[M02] 读取环境变量
来源：http://cc.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://nc.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sc.asd995.cn

JS:   process.env.HOME
来源：http://me.shxzukj.cn

TS:   process.env.HOME
来源：http://oz.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://ul.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kd.hahajie.cn

Ruby: ENV["HOME"]
来源：http://hi.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yo.shtwfgs.cn

[M03] 执行外部命令
来源：http://jr.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://co.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ok.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kc.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yj.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lr.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sl.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jk.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://oz.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://xu.yuexingan06.cn

Py:   os.getcwd()
来源：http://zb.shtwfgs.cn

PHP:  getcwd();
来源：http://nf.chemitech.net.cn

JS:   process.cwd()
来源：http://ig.asd995.cn

TS:   process.cwd()
来源：http://db.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://aa.jctech888.com.cn

Go:   os.Getwd()
来源：http://ff.bjjhwx.cn

Ruby: Dir.pwd
来源：http://uu.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zm.huixinmuqiang.cn

[M05] 设置退出码
来源：http://bf.panjiajie.cn

Py:   sys.exit(1)
来源：http://pq.shxzukj.cn

PHP:  exit(1);
来源：http://zk.shxzskj.cn

JS:   process.exit(1)
来源：http://hr.nszjky.cn

TS:   process.exit(1)
来源：http://qi.bookmarksfly.cn

Java: System.exit(1)
来源：http://ll.shxzukj.cn

Go:   os.Exit(1)
来源：http://jb.shxzskj.cn

Ruby: exit 1
来源：http://fp.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jd.hnjuh.cn

[M06] 向标准错误输出
来源：http://er.szxytkj.cn

Py:   print("err", file=sys.stderr)
来源：http://bj.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dm.gzmigu.cn

JS:   console.error("err")
来源：http://os.jctech888.com.cn

TS:   console.error("err")
来源：http://aj.9csxet.cn

Java: System.err.println("err")
来源：http://sf.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ho.asd995.cn

Ruby: warn "err"
来源：http://ta.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://kt.newstarts.cn

[M07] 判断是否为主入口
来源：http://ls.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://wn.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rg.yuexingan06.cn

JS:   require.main === module
来源：http://rn.huixiangedu.cn

TS:   require.main === module
来源：http://fw.shxzskj.cn

Java: public static void main(String[] args)
来源：http://rj.chemitech.net.cn

Go:   func main()
来源：http://tt.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bd.521024.cn

C#:   static void Main(string[] args)
来源：http://cf.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://bx.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://pd.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://hs.asd995.cn

JS:   process.platform;  process.version
来源：http://ml.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://ti.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rr.gzmigu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yv.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vr.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fd.hahajie.cn

================================================================================
来源：http://jy.panjiajie.cn

N. 数据结构与算法
来源：http://ln.521024.cn

================================================================================
来源：http://bx.colortex.cn

[N01] 二分查找（有序数组）
来源：http://vl.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hd.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sg.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ox.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pq.gzmigu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jq.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://wu.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gm.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://fu.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://lg.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fn.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ha.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://el.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mj.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://kc.nszjky.cn

Ruby: arr.sort
来源：http://uy.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pc.nicolike.cn

[N03] 快速排序（分治示例）
来源：http://sp.bookmarksfly.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dd.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://fv.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cw.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kd.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xc.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ng.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pn.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ek.chemitech.net.cn

[N04] 斐波那契数列
来源：http://eh.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yj.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rn.jianghongdianzi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yn.newstarts.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://za.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pz.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rp.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cx.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qd.huixiangedu.cn

[N05] 最大公约数
来源：http://zd.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://ml.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pj.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wp.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gi.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yx.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pq.nicolike.cn

Ruby: a.gcd(b)
来源：http://im.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uj.shxzukj.cn

[N06] 判断回文字符串
来源：http://kr.nszjky.cn

Py:   s == s[::-1]
来源：http://vv.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://uh.shtwfgs.cn

JS:   s === [...s].reverse().join("")
来源：http://jz.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://kf.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dv.szsharing.cn

Go:   // 双指针从两端比较
来源：http://by.jctech888.com.cn

Ruby: s == s.reverse
来源：http://lr.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yz.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://fi.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yx.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jm.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qj.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://gw.muxihuayi.cn

Java: // 手写 HashMap
来源：http://os.newstarts.cn

Go:   // 手写 map[int]int
来源：http://jk.gzmigu.cn

Ruby: // 手写 Hash
来源：http://vq.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://il.jctech888.com.cn

[N08] 生成全排列
来源：http://oh.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://fm.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://cd.hahajie.cn

JS:   // 手写回溯递归
来源：http://cv.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://ye.nszjky.cn

Java: // 手写回溯递归
来源：http://gq.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://zw.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://wl.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://mq.521024.cn

[N09] 栈与队列
来源：http://tz.9csxet.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ng.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pz.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eh.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ip.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ao.colortex.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://il.nicolike.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ub.haigaiapp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rv.huanxung.cn

[N10] 链表节点定义
来源：http://wn.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jr.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://us.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hr.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wj.colortex.cn

Java: class Node { int v; Node next; }
来源：http://uw.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pz.gzmigu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qd.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eh.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://yq.asd995.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nn.newstarts.cn

PHP:  // 手写递归函数
来源：http://ri.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pe.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ku.szsharing.cn

Java: // 手写递归
来源：http://mc.szsharing.cn

Go:   // 手写递归
来源：http://ne.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wf.jctech888.com.cn

C#:   // 手写递归
来源：http://sa.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sr.szxytkj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jv.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lc.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ew.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oz.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ix.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ys.gzmigu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pt.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ux.huixinmuqiang.cn

================================================================================
来源：http://qf.huixiangedu.cn

O. 并发与异步
来源：http://ey.shxzskj.cn

================================================================================
来源：http://hy.haigaiapp.cn

[O01] 启动一个线程
来源：http://gi.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zb.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ud.newstarts.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ta.gzmigu.cn

TS:   // 同 JS
来源：http://lx.szxytkj.cn

Java: new Thread(() -> f()).start()
来源：http://bu.colortex.cn

Go:   go f()
来源：http://xk.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://ft.shtwfgs.cn

C#:   Task.Run(() => F());
来源：http://nj.shxzskj.cn


<!-- 参考信息 -->