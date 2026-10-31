代发 wailian999

[K06] 解析 URL 查询串
来源：http://xx.nicolike.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nl.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sy.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xf.jctech888.com.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bw.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fs.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vx.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cw.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jh.bjjhwx.cn

[K07] 进制转换
来源：http://zn.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ry.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://py.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zz.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fk.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qd.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kt.yuntaijiaju.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eg.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ex.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://cr.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://pq.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cd.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ct.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://kj.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lh.nszjky.cn

Go:   encoding/gob
来源：http://xr.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://hr.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ax.shxzukj.cn

================================================================================
来源：http://bs.newstarts.cn

L. 网络请求
来源：http://iq.szsharing.cn

================================================================================
来源：http://hp.shxzukj.cn

[L01] 发送 GET 请求
来源：http://ck.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bu.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://en.huixiangedu.cn

JS:   await fetch(url)
来源：http://fa.9csxet.cn

TS:   await fetch(url)
来源：http://ts.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ab.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://ex.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ex.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lr.nicolike.cn

[L02] 发送 POST JSON
来源：http://tm.huanxung.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xb.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qt.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iz.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xz.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ld.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kn.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bz.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zs.panjiajie.cn

[L03] 设置自定义请求头
来源：http://qv.bjjhwx.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kg.521024.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tv.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hr.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://js.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mu.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ec.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ga.521024.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zo.shxzskj.cn

[L04] 设置超时
来源：http://ne.shxzukj.cn

Py:   requests.get(url, timeout=5)
来源：http://nc.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hn.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vo.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nl.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mh.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qp.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vz.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ys.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://pj.muxihuayi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ni.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bj.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hq.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qh.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nb.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iq.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rg.haigaiapp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fw.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://sq.gzmigu.cn

Py:   resp.json()
来源：http://fn.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ng.colortex.cn

JS:   await resp.json()
来源：http://oe.muxihuayi.cn

TS:   await resp.json()
来源：http://ap.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://do.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dw.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://ou.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eq.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://lk.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hq.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lx.asd995.cn

JS:   resp.ok;  resp.status
来源：http://aa.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://be.muxihuayi.cn

Java: resp.statusCode()
来源：http://xo.huixiangedu.cn

Go:   resp.StatusCode
来源：http://iw.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://ju.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://rc.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://sf.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cj.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://yj.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zv.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ga.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ig.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ca.shxzskj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sa.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rf.521024.cn

================================================================================
来源：http://dp.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://nn.szsharing.cn

================================================================================
来源：http://bb.gzmigu.cn

[M01] 读取命令行参数
来源：http://kr.panjiajie.cn

Py:   sys.argv[1:]
来源：http://ky.hahajie.cn

PHP:  $argv;  $argc;
来源：http://hq.nicolike.cn

JS:   process.argv.slice(2)
来源：http://qm.szsharing.cn

TS:   process.argv.slice(2)
来源：http://bs.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://sk.bjjhwx.cn

Go:   os.Args[1:]
来源：http://km.szxytkj.cn

Ruby: ARGV
来源：http://dv.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://te.nicolike.cn

[M02] 读取环境变量
来源：http://ld.huixiangedu.cn

Py:   os.environ.get("HOME")
来源：http://wr.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pd.bookmarksfly.cn

JS:   process.env.HOME
来源：http://zw.szsharing.cn

TS:   process.env.HOME
来源：http://vh.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://is.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kg.shxzukj.cn

Ruby: ENV["HOME"]
来源：http://vr.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://up.hnjuh.cn

[M03] 执行外部命令
来源：http://ya.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://il.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ks.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://me.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://st.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bb.yuexingan06.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aj.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yp.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://dq.nszjky.cn

[M04] 获取当前工作目录
来源：http://ae.asd995.cn

Py:   os.getcwd()
来源：http://kw.haigaiapp.cn

PHP:  getcwd();
来源：http://eo.muxihuayi.cn

JS:   process.cwd()
来源：http://eu.muxihuayi.cn

TS:   process.cwd()
来源：http://zd.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://rx.hnjuh.cn

Go:   os.Getwd()
来源：http://es.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://if.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ty.panjiajie.cn

[M05] 设置退出码
来源：http://nd.bjjhwx.cn

Py:   sys.exit(1)
来源：http://wg.huixinmuqiang.cn

PHP:  exit(1);
来源：http://bj.szsharing.cn

JS:   process.exit(1)
来源：http://qx.haigaiapp.cn

TS:   process.exit(1)
来源：http://mo.haigaiapp.cn

Java: System.exit(1)
来源：http://vu.hnjuh.cn

Go:   os.Exit(1)
来源：http://uq.jctech888.com.cn

Ruby: exit 1
来源：http://af.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ds.jctech888.com.cn

[M06] 向标准错误输出
来源：http://sz.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://oz.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wgjwhj.cn

JS:   console.error("err")
来源：http://jr.hnjuh.cn

TS:   console.error("err")
来源：http://mu.asd995.cn

Java: System.err.println("err")
来源：http://bv.asd995.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://em.huanxung.cn

Ruby: warn "err"
来源：http://dn.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://np.hnjuh.cn

[M07] 判断是否为主入口
来源：http://qv.asd995.cn

Py:   if __name__ == "__main__":
来源：http://fd.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hj.shxzskj.cn

JS:   require.main === module
来源：http://jt.nszjky.cn

TS:   require.main === module
来源：http://fp.asd995.cn

Java: public static void main(String[] args)
来源：http://jb.huixinmuqiang.cn

Go:   func main()
来源：http://qg.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bp.nszjky.cn

C#:   static void Main(string[] args)
来源：http://on.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://ro.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://lc.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://lh.huanxung.cn

JS:   process.platform;  process.version
来源：http://va.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://pq.huixinmuqiang.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ga.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pw.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://by.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bw.muxihuayi.cn

================================================================================
来源：http://tc.yuntaijiaju.cn

N. 数据结构与算法
来源：http://je.gzmigu.cn

================================================================================
来源：http://bi.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://nh.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kd.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nh.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vl.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gd.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://av.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://mz.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dt.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ge.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://ym.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://aa.huixinmuqiang.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rl.chemitech.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xz.shxzukj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qo.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://er.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://rx.9csxet.cn

Ruby: arr.sort
来源：http://lx.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bp.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://qj.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zg.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://yq.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cf.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vr.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ml.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qj.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lm.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kd.9csxet.cn

[N04] 斐波那契数列
来源：http://tb.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dl.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vp.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://of.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uf.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kt.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qb.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ta.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qs.szxytkj.cn

[N05] 最大公约数
来源：http://im.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://tp.panjiajie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fk.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zy.huixinmuqiang.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bs.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ir.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ed.asd995.cn

Ruby: a.gcd(b)
来源：http://lp.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ys.chemitech.net.cn

[N06] 判断回文字符串
来源：http://mf.szxytkj.cn

Py:   s == s[::-1]
来源：http://lo.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://di.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://rj.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://kh.bookmarksfly.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pz.521024.cn

Go:   // 双指针从两端比较
来源：http://xd.lnxyls.cn

Ruby: s == s.reverse
来源：http://ro.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rk.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://wb.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bu.huixiangedu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aa.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oo.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://ry.huanxung.cn

Java: // 手写 HashMap
来源：http://ct.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://xq.lnxyls.cn

Ruby: // 手写 Hash
来源：http://bs.gzmigu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fj.lnxyls.cn

[N08] 生成全排列
来源：http://kj.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://hz.shxzskj.cn

PHP:  // 手写递归交换
来源：http://ht.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://vo.shxzskj.cn

TS:   // 手写回溯递归
来源：http://ta.panjiajie.cn

Java: // 手写回溯递归
来源：http://dl.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://es.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://wy.lnxyls.cn

C#:   // 手写回溯递归
来源：http://ik.lnxyls.cn

[N09] 栈与队列
来源：http://ai.jctech888.com.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yp.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wf.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cl.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cx.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wy.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qz.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mm.521024.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ut.huixiangedu.cn

[N10] 链表节点定义
来源：http://lm.yuntaijiaju.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tl.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bo.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://of.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hn.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://mv.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kd.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://by.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hn.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://il.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ko.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://po.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tv.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qn.yuntaijiaju.cn

Java: // 手写递归
来源：http://vk.jianghongdianzi.cn

Go:   // 手写递归
来源：http://er.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wj.huanxung.cn

C#:   // 手写递归
来源：http://uc.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lp.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zf.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://td.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bf.muxihuayi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hu.jctech888.com.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nt.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cb.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vn.huixinmuqiang.cn

================================================================================
来源：http://ab.szxytkj.cn

O. 并发与异步
来源：http://zi.haigaiapp.cn

================================================================================
来源：http://il.shxzukj.cn

[O01] 启动一个线程
来源：http://xv.9csxet.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ib.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lc.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tp.huixinmuqiang.cn

TS:   // 同 JS
来源：http://sn.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://jo.haigaiapp.cn

Go:   go f()
来源：http://gt.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://hf.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://nd.colortex.cn


<!-- 参考信息 -->