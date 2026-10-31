代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://ua.huixiangedu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://re.yuexingan06.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ko.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zc.asd995.cn

[K06] 解析 URL 查询串
来源：http://uc.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ml.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hw.haigaiapp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bv.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://on.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kn.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rp.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://le.colortex.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mv.521024.cn

[K07] 进制转换
来源：http://ry.huanxung.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wv.shxzukj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jb.nicolike.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gp.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bh.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zh.szsharing.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pf.muxihuayi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oc.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wd.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://xo.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://vn.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mu.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://gm.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://yx.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tf.szxytkj.cn

Go:   encoding/gob
来源：http://hv.szxytkj.cn

Ruby: Marshal.dump(obj)
来源：http://tt.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ec.huanxung.cn

================================================================================
来源：http://rn.szxytkj.cn

L. 网络请求
来源：http://ne.shxzskj.cn

================================================================================
来源：http://wh.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://dd.haigaiapp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xx.bjjhwx.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bm.asd995.cn

JS:   await fetch(url)
来源：http://cd.nszjky.cn

TS:   await fetch(url)
来源：http://oi.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pp.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://tc.huixiangedu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zc.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wt.nicolike.cn

[L02] 发送 POST JSON
来源：http://df.yuntaijiaju.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zo.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kt.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ds.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tg.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xk.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://na.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ho.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nu.nszjky.cn

[L03] 设置自定义请求头
来源：http://wf.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://az.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xr.chemitech.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fm.szxytkj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wl.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vq.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ww.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://px.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ov.gzmigu.cn

[L04] 设置超时
来源：http://gb.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://li.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iz.haigaiapp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jn.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bg.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eh.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hy.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ma.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oq.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://hs.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kn.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ji.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yo.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hp.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://se.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rn.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ww.9csxet.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://el.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://un.yuntaijiaju.cn

Py:   resp.json()
来源：http://wd.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://kv.yuexingan06.cn

JS:   await resp.json()
来源：http://cj.nicolike.cn

TS:   await resp.json()
来源：http://qg.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gr.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ux.newstarts.cn

Ruby: JSON.parse(resp.body)
来源：http://ma.9csxet.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qk.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://mh.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dn.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ne.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://ic.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://wb.colortex.cn

Java: resp.statusCode()
来源：http://vz.bjjhwx.cn

Go:   resp.StatusCode
来源：http://xl.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://co.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://kh.nicolike.cn

[L08] 并发请求多个地址
来源：http://nw.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://or.asd995.cn

PHP:  curl_multi_init() 系列
来源：http://nw.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xw.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://le.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jx.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://td.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://en.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://za.bookmarksfly.cn

================================================================================
来源：http://gf.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://ei.szxytkj.cn

================================================================================
来源：http://md.hahajie.cn

[M01] 读取命令行参数
来源：http://uk.nszjky.cn

Py:   sys.argv[1:]
来源：http://eg.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://nc.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://bn.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://mc.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://dy.9csxet.cn

Go:   os.Args[1:]
来源：http://wf.shxzukj.cn

Ruby: ARGV
来源：http://hi.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://wb.asd995.cn

[M02] 读取环境变量
来源：http://zp.colortex.cn

Py:   os.environ.get("HOME")
来源：http://ca.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ja.chemitech.net.cn

JS:   process.env.HOME
来源：http://pn.lnxyls.cn

TS:   process.env.HOME
来源：http://yp.hahajie.cn

Java: System.getenv("HOME")
来源：http://ah.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ks.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://bk.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ld.9csxet.cn

[M03] 执行外部命令
来源：http://xm.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yo.huixinmuqiang.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ff.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ti.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kq.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wv.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://th.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fg.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ik.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://fs.bookmarksfly.cn

Py:   os.getcwd()
来源：http://os.nszjky.cn

PHP:  getcwd();
来源：http://oi.shtwfgs.cn

JS:   process.cwd()
来源：http://ns.asd995.cn

TS:   process.cwd()
来源：http://xh.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://es.shxzskj.cn

Go:   os.Getwd()
来源：http://jz.asd995.cn

Ruby: Dir.pwd
来源：http://nl.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ul.hahajie.cn

[M05] 设置退出码
来源：http://ue.shxzskj.cn

Py:   sys.exit(1)
来源：http://ki.521024.cn

PHP:  exit(1);
来源：http://iw.jctech888.com.cn

JS:   process.exit(1)
来源：http://qm.shtwfgs.cn

TS:   process.exit(1)
来源：http://fk.lnxyls.cn

Java: System.exit(1)
来源：http://bs.szxytkj.cn

Go:   os.Exit(1)
来源：http://jk.9csxet.cn

Ruby: exit 1
来源：http://eg.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rq.yuexingan06.cn

[M06] 向标准错误输出
来源：http://nz.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://qc.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sq.jctech888.com.cn

JS:   console.error("err")
来源：http://lu.9csxet.cn

TS:   console.error("err")
来源：http://ms.szsharing.cn

Java: System.err.println("err")
来源：http://tk.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://px.chemitech.net.cn

Ruby: warn "err"
来源：http://nb.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://te.asd995.cn

[M07] 判断是否为主入口
来源：http://wc.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://jr.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qq.lnxyls.cn

JS:   require.main === module
来源：http://rc.panjiajie.cn

TS:   require.main === module
来源：http://jr.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://eu.yuntaijiaju.cn

Go:   func main()
来源：http://qn.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qq.521024.cn

C#:   static void Main(string[] args)
来源：http://gr.521024.cn

[M08] 获取系统与运行时信息
来源：http://iu.nszjky.cn

Py:   platform.system();  platform.python_version()
来源：http://ht.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://wh.shxzukj.cn

JS:   process.platform;  process.version
来源：http://fl.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://pu.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dg.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ue.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ok.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oe.521024.cn

================================================================================
来源：http://il.szsharing.cn

N. 数据结构与算法
来源：http://lt.jianghongdianzi.cn

================================================================================
来源：http://sp.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://vo.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://um.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ba.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://li.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lh.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://re.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://vc.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ii.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ee.jianghongdianzi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ii.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://lw.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pk.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://be.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pz.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ba.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://dx.jctech888.com.cn

Ruby: arr.sort
来源：http://zr.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rl.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://yn.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hr.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://iw.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qy.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qu.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://se.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://in.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jt.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hp.panjiajie.cn

[N04] 斐波那契数列
来源：http://du.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://do.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yf.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mm.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tu.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hn.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fe.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xr.haigaiapp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kc.muxihuayi.cn

[N05] 最大公约数
来源：http://np.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ta.newstarts.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yb.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pl.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ex.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nn.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yu.shxzskj.cn

Ruby: a.gcd(b)
来源：http://xv.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mo.panjiajie.cn

[N06] 判断回文字符串
来源：http://ya.shxzukj.cn

Py:   s == s[::-1]
来源：http://cg.nszjky.cn

PHP:  $s === strrev($s);
来源：http://dq.chemitech.net.cn

JS:   s === [...s].reverse().join("")
来源：http://jd.bjjhwx.cn

TS:   s === [...s].reverse().join("")
来源：http://xt.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zg.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://eo.gzmigu.cn

Ruby: s == s.reverse
来源：http://gr.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dz.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://yk.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fr.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ld.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dr.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://bo.nicolike.cn

Java: // 手写 HashMap
来源：http://nw.huixinmuqiang.cn

Go:   // 手写 map[int]int
来源：http://bi.nicolike.cn

Ruby: // 手写 Hash
来源：http://rz.muxihuayi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ig.wgjwhj.cn

[N08] 生成全排列
来源：http://vj.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://av.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://kt.nszjky.cn

JS:   // 手写回溯递归
来源：http://os.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://bt.haigaiapp.cn

Java: // 手写回溯递归
来源：http://rz.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://xa.colortex.cn

Ruby: arr.permutation.to_a
来源：http://is.huanxung.cn

C#:   // 手写回溯递归
来源：http://xm.huixiangedu.cn

[N09] 栈与队列
来源：http://vj.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ye.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ly.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://el.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ys.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vd.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qv.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://po.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bg.jctech888.com.cn

[N10] 链表节点定义
来源：http://nj.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sz.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wc.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fu.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gv.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://ty.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fa.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rb.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pt.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://za.huixiangedu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cy.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://qa.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xt.shxzukj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://la.chemitech.net.cn

Java: // 手写递归
来源：http://ja.huixiangedu.cn

Go:   // 手写递归
来源：http://jq.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lt.jianghongdianzi.cn

C#:   // 手写递归
来源：http://cz.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uc.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ls.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://za.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xm.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ui.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vw.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ts.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pd.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ym.hnjuh.cn

================================================================================
来源：http://mj.shxzukj.cn

O. 并发与异步
来源：http://cf.muxihuayi.cn

================================================================================
来源：http://vo.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://vj.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zn.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zt.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ez.jianghongdianzi.cn

TS:   // 同 JS
来源：http://eq.huixiangedu.cn


<!-- 参考信息 -->