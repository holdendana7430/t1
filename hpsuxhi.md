代发 wailian999

[K06] 解析 URL 查询串
来源：http://gp.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hi.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cm.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ts.huanxung.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bt.shtwfgs.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tc.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ug.huixiangedu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nz.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ix.newstarts.cn

[K07] 进制转换
来源：http://eg.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wa.lnxyls.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yp.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ma.huixinmuqiang.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fm.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ry.jctech888.com.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fq.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fr.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ij.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://fb.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://hs.huixiangedu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pi.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yw.9csxet.cn

TS:   v8.serialize(obj)        // Node
来源：http://as.yuntaijiaju.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wg.wgjwhj.cn

Go:   encoding/gob
来源：http://nx.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://so.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zo.bookmarksfly.cn

================================================================================
来源：http://bo.asd995.cn

L. 网络请求
来源：http://ad.jianghongdianzi.cn

================================================================================
来源：http://ve.szxytkj.cn

[L01] 发送 GET 请求
来源：http://mg.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ll.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lq.lnxyls.cn

JS:   await fetch(url)
来源：http://sc.wgjwhj.cn

TS:   await fetch(url)
来源：http://jq.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ae.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://wz.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://id.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gb.newstarts.cn

[L02] 发送 POST JSON
来源：http://gz.hahajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ek.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nb.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://op.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ou.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zn.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oq.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rx.panjiajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vv.asd995.cn

[L03] 设置自定义请求头
来源：http://cw.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bg.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://an.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hm.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ud.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ov.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yc.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qz.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cm.szsharing.cn

[L04] 设置超时
来源：http://kp.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://bk.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://af.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kk.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pq.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://us.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cl.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wn.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://zb.gzmigu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zr.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ia.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rq.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qy.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pm.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://io.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ah.huixiangedu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uc.huanxung.cn

[L06] 解析响应为 JSON
来源：http://xr.shxzskj.cn

Py:   resp.json()
来源：http://ik.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://jr.huixiangedu.cn

JS:   await resp.json()
来源：http://fw.yuntaijiaju.cn

TS:   await resp.json()
来源：http://sp.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wl.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wn.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://dc.yuntaijiaju.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ar.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://pk.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lg.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lc.asd995.cn

JS:   resp.ok;  resp.status
来源：http://la.asd995.cn

TS:   resp.ok;  resp.status
来源：http://qr.shtwfgs.cn

Java: resp.statusCode()
来源：http://oe.asd995.cn

Go:   resp.StatusCode
来源：http://ra.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://cy.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://et.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://fw.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ox.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://ad.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://du.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ll.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jd.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://el.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ip.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mt.shxzukj.cn

================================================================================
来源：http://ie.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://qb.newstarts.cn

================================================================================
来源：http://lb.newstarts.cn

[M01] 读取命令行参数
来源：http://md.lnxyls.cn

Py:   sys.argv[1:]
来源：http://yn.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://bj.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://nc.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://ts.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://me.nicolike.cn

Go:   os.Args[1:]
来源：http://ze.colortex.cn

Ruby: ARGV
来源：http://or.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://px.muxihuayi.cn

[M02] 读取环境变量
来源：http://nk.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://xf.bjjhwx.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bg.asd995.cn

JS:   process.env.HOME
来源：http://zw.521024.cn

TS:   process.env.HOME
来源：http://sz.521024.cn

Java: System.getenv("HOME")
来源：http://ld.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wa.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://jk.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hk.chemitech.net.cn

[M03] 执行外部命令
来源：http://hm.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rd.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ep.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rp.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mo.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ob.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qj.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hz.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://nk.shxzskj.cn

[M04] 获取当前工作目录
来源：http://bl.chemitech.net.cn

Py:   os.getcwd()
来源：http://cu.yuntaijiaju.cn

PHP:  getcwd();
来源：http://pj.521024.cn

JS:   process.cwd()
来源：http://zq.nicolike.cn

TS:   process.cwd()
来源：http://sn.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://yp.shxzskj.cn

Go:   os.Getwd()
来源：http://wg.hahajie.cn

Ruby: Dir.pwd
来源：http://yf.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mr.szsharing.cn

[M05] 设置退出码
来源：http://ql.9csxet.cn

Py:   sys.exit(1)
来源：http://vq.muxihuayi.cn

PHP:  exit(1);
来源：http://ma.panjiajie.cn

JS:   process.exit(1)
来源：http://yr.shxzukj.cn

TS:   process.exit(1)
来源：http://zm.shtwfgs.cn

Java: System.exit(1)
来源：http://tv.bjjhwx.cn

Go:   os.Exit(1)
来源：http://jb.lnxyls.cn

Ruby: exit 1
来源：http://tb.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bv.szxytkj.cn

[M06] 向标准错误输出
来源：http://jq.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://af.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://je.bjjhwx.cn

JS:   console.error("err")
来源：http://hv.nicolike.cn

TS:   console.error("err")
来源：http://us.huixiangedu.cn

Java: System.err.println("err")
来源：http://uq.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sz.jianghongdianzi.cn

Ruby: warn "err"
来源：http://pk.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://tg.szsharing.cn

[M07] 判断是否为主入口
来源：http://ao.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://cv.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mr.nicolike.cn

JS:   require.main === module
来源：http://oh.521024.cn

TS:   require.main === module
来源：http://ew.asd995.cn

Java: public static void main(String[] args)
来源：http://qc.shtwfgs.cn

Go:   func main()
来源：http://gm.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wu.9csxet.cn

C#:   static void Main(string[] args)
来源：http://rn.9csxet.cn

[M08] 获取系统与运行时信息
来源：http://si.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://pn.hnjuh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ls.szsharing.cn

JS:   process.platform;  process.version
来源：http://ia.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://mz.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xp.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hw.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://su.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tb.gzmigu.cn

================================================================================
来源：http://qs.szsharing.cn

N. 数据结构与算法
来源：http://dy.bookmarksfly.cn

================================================================================
来源：http://jg.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://wv.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xv.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kg.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zb.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ek.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nb.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://xw.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cj.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ve.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bh.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://vc.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lc.jianghongdianzi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ji.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gm.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ix.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://zc.bjjhwx.cn

Ruby: arr.sort
来源：http://tf.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tb.asd995.cn

[N03] 快速排序（分治示例）
来源：http://gf.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nx.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://ru.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://me.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eu.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fp.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cm.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pt.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dy.nszjky.cn

[N04] 斐波那契数列
来源：http://qt.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jc.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sd.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zv.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sr.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aa.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gr.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ua.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ez.shtwfgs.cn

[N05] 最大公约数
来源：http://me.521024.cn

Py:   math.gcd(a, b)
来源：http://ew.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vy.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sw.huanxung.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ww.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://py.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://ny.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://li.9csxet.cn

[N06] 判断回文字符串
来源：http://hf.hnjuh.cn

Py:   s == s[::-1]
来源：http://bq.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://yd.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://xf.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://jo.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tn.huanxung.cn

Go:   // 双指针从两端比较
来源：http://ea.yuexingan06.cn

Ruby: s == s.reverse
来源：http://ta.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gs.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://nv.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ae.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wd.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gf.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://un.panjiajie.cn

Java: // 手写 HashMap
来源：http://rg.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://nx.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://an.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wt.nicolike.cn

[N08] 生成全排列
来源：http://jb.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://bg.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://zt.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://ln.jianghongdianzi.cn

TS:   // 手写回溯递归
来源：http://qa.bookmarksfly.cn

Java: // 手写回溯递归
来源：http://yz.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://yy.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://fu.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://cc.wgjwhj.cn

[N09] 栈与队列
来源：http://ei.szxytkj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nx.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ls.shtwfgs.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kd.huixiangedu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://df.lnxyls.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://in.shxzskj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rs.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dv.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hq.jctech888.com.cn

[N10] 链表节点定义
来源：http://pg.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hv.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yn.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mv.shtwfgs.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nm.szsharing.cn

Java: class Node { int v; Node next; }
来源：http://pw.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tx.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qj.colortex.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nv.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://if.lnxyls.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lm.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://lr.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vu.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ca.yuexingan06.cn

Java: // 手写递归
来源：http://oa.muxihuayi.cn

Go:   // 手写递归
来源：http://zi.bjjhwx.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ss.szxytkj.cn

C#:   // 手写递归
来源：http://lg.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://su.bjjhwx.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yo.wgjwhj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://of.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://if.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ku.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zu.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://md.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ru.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mb.shxzskj.cn

================================================================================
来源：http://fr.lnxyls.cn

O. 并发与异步
来源：http://qo.bjjhwx.cn

================================================================================
来源：http://vj.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://eu.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vp.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vu.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ge.hahajie.cn

TS:   // 同 JS
来源：http://bu.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://xm.wgjwhj.cn

Go:   go f()
来源：http://nm.hnjuh.cn

Ruby: Thread.new { f }
来源：http://kf.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://lt.yuntaijiaju.cn


<!-- 参考信息 -->