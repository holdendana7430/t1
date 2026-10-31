代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://bt.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://sj.haigaiapp.cn

JS:   structuredClone(obj)
来源：http://nl.huixinmuqiang.cn

TS:   structuredClone(obj)
来源：http://oa.bookmarksfly.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eu.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hi.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cr.nszjky.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nc.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://bb.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qd.wgjwhj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pu.9csxet.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zb.huixiangedu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://on.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ia.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cx.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mn.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gk.bookmarksfly.cn

[K07] 进制转换
来源：http://hv.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qf.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sy.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cc.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://np.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yi.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fp.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cg.huixinmuqiang.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ik.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ji.521024.cn

Py:   pickle.dumps(obj)
来源：http://xo.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uq.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://cx.szxytkj.cn

TS:   v8.serialize(obj)        // Node
来源：http://yi.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ki.huixiangedu.cn

Go:   encoding/gob
来源：http://rt.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://yh.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mf.hahajie.cn

================================================================================
来源：http://ti.hahajie.cn

L. 网络请求
来源：http://bt.9csxet.cn

================================================================================
来源：http://jt.bjjhwx.cn

[L01] 发送 GET 请求
来源：http://to.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ha.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://np.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://kw.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://wd.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ij.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://tf.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ck.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tl.newstarts.cn

[L02] 发送 POST JSON
来源：http://up.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mk.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gz.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ih.muxihuayi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://md.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rd.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qj.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sv.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://up.gzmigu.cn

[L03] 设置自定义请求头
来源：http://uq.shtwfgs.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hv.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wl.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://il.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iy.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ix.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://je.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yu.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xl.lnxyls.cn

[L04] 设置超时
来源：http://nj.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://ly.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cl.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gf.bjjhwx.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zv.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tk.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ph.hnjuh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://az.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vw.nszjky.cn

[L05] 上传文件（multipart）
来源：http://sa.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bv.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hj.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zq.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ux.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fl.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yc.szxytkj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wd.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sq.9csxet.cn

[L06] 解析响应为 JSON
来源：http://tl.bjjhwx.cn

Py:   resp.json()
来源：http://yi.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://wo.haigaiapp.cn

JS:   await resp.json()
来源：http://qr.bookmarksfly.cn

TS:   await resp.json()
来源：http://lp.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xk.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bt.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://lp.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fg.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ou.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kr.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tx.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://gy.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://cq.haigaiapp.cn

Java: resp.statusCode()
来源：http://yp.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://qy.hnjuh.cn

Ruby: resp.code.to_i
来源：http://lc.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://eh.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://si.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sc.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://to.521024.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lo.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://af.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ys.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ks.nszjky.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vz.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kg.panjiajie.cn

================================================================================
来源：http://vr.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://yc.jianghongdianzi.cn

================================================================================
来源：http://ey.shxzukj.cn

[M01] 读取命令行参数
来源：http://yw.szxytkj.cn

Py:   sys.argv[1:]
来源：http://ra.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ff.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://ga.colortex.cn

TS:   process.argv.slice(2)
来源：http://bn.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://kj.huanxung.cn

Go:   os.Args[1:]
来源：http://pm.jctech888.com.cn

Ruby: ARGV
来源：http://sf.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://mc.muxihuayi.cn

[M02] 读取环境变量
来源：http://dh.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://bx.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wm.shxzskj.cn

JS:   process.env.HOME
来源：http://vx.panjiajie.cn

TS:   process.env.HOME
来源：http://qj.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://so.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mo.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://ug.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ge.yuexingan06.cn

[M03] 执行外部命令
来源：http://bv.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wz.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qh.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vb.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://be.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wr.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qy.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rv.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ou.hnjuh.cn

[M04] 获取当前工作目录
来源：http://fo.nicolike.cn

Py:   os.getcwd()
来源：http://bh.newstarts.cn

PHP:  getcwd();
来源：http://hc.szxytkj.cn

JS:   process.cwd()
来源：http://bj.yuntaijiaju.cn

TS:   process.cwd()
来源：http://au.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yv.huixiangedu.cn

Go:   os.Getwd()
来源：http://pf.huanxung.cn

Ruby: Dir.pwd
来源：http://ie.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zf.521024.cn

[M05] 设置退出码
来源：http://vz.haigaiapp.cn

Py:   sys.exit(1)
来源：http://rc.jctech888.com.cn

PHP:  exit(1);
来源：http://oz.szxytkj.cn

JS:   process.exit(1)
来源：http://qi.yuexingan06.cn

TS:   process.exit(1)
来源：http://qr.panjiajie.cn

Java: System.exit(1)
来源：http://zp.hahajie.cn

Go:   os.Exit(1)
来源：http://no.haigaiapp.cn

Ruby: exit 1
来源：http://kr.szsharing.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://my.9csxet.cn

[M06] 向标准错误输出
来源：http://xv.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://mi.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://th.newstarts.cn

JS:   console.error("err")
来源：http://fs.9csxet.cn

TS:   console.error("err")
来源：http://ik.shtwfgs.cn

Java: System.err.println("err")
来源：http://bv.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ny.9csxet.cn

Ruby: warn "err"
来源：http://su.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ug.hahajie.cn

[M07] 判断是否为主入口
来源：http://hi.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://gr.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zc.nicolike.cn

JS:   require.main === module
来源：http://wj.yuntaijiaju.cn

TS:   require.main === module
来源：http://fr.9csxet.cn

Java: public static void main(String[] args)
来源：http://ky.asd995.cn

Go:   func main()
来源：http://ll.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fm.huanxung.cn

C#:   static void Main(string[] args)
来源：http://kc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://yw.wgjwhj.cn

Py:   platform.system();  platform.python_version()
来源：http://am.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://gn.9csxet.cn

JS:   process.platform;  process.version
来源：http://wv.szsharing.cn

TS:   process.platform;  process.version
来源：http://qo.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zu.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cc.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kl.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://go.muxihuayi.cn

================================================================================
来源：http://jx.colortex.cn

N. 数据结构与算法
来源：http://gh.bjjhwx.cn

================================================================================
来源：http://bu.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://xt.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rc.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yb.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dz.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ds.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lo.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://cb.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ni.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mj.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://mo.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://gq.asd995.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qx.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xv.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rh.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jx.nicolike.cn

Go:   slices.Sort(arr)
来源：http://xn.521024.cn

Ruby: arr.sort
来源：http://aw.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bl.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://ca.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ch.newstarts.cn

PHP:  // 递归实现，或用 usort
来源：http://it.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bj.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mg.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cy.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tc.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wx.hahajie.cn

[N04] 斐波那契数列
来源：http://oq.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fy.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xg.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://am.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ww.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iq.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jg.colortex.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gt.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://md.yuntaijiaju.cn

[N05] 最大公约数
来源：http://we.nszjky.cn

Py:   math.gcd(a, b)
来源：http://hd.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://es.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cl.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://no.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tb.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tk.521024.cn

Ruby: a.gcd(b)
来源：http://vj.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wd.hahajie.cn

[N06] 判断回文字符串
来源：http://bm.yuexingan06.cn

Py:   s == s[::-1]
来源：http://op.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://ua.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://sp.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://je.lnxyls.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ri.szsharing.cn

Go:   // 双指针从两端比较
来源：http://fp.hahajie.cn

Ruby: s == s.reverse
来源：http://pt.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ol.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://ft.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://je.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qc.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sy.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://eb.hnjuh.cn

Java: // 手写 HashMap
来源：http://li.huanxung.cn

Go:   // 手写 map[int]int
来源：http://ih.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://zv.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gh.muxihuayi.cn

[N08] 生成全排列
来源：http://uw.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://ns.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://gt.asd995.cn

JS:   // 手写回溯递归
来源：http://kg.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://sk.shxzukj.cn

Java: // 手写回溯递归
来源：http://vv.jctech888.com.cn

Go:   // 手写回溯递归
来源：http://vx.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://dv.shxzukj.cn

C#:   // 手写回溯递归
来源：http://vc.nszjky.cn

[N09] 栈与队列
来源：http://eq.szsharing.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pb.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lj.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dg.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://va.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vk.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bk.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cr.colortex.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pq.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://zq.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wb.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://si.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://th.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wn.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://ii.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gd.huixinmuqiang.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ea.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mc.shtwfgs.cn

[N11] 二叉树中序遍历
来源：http://wy.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://el.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://ze.bookmarksfly.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sf.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kf.wgjwhj.cn

Java: // 手写递归
来源：http://jo.szxytkj.cn

Go:   // 手写递归
来源：http://hy.colortex.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yy.lnxyls.cn

C#:   // 手写递归
来源：http://wx.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nu.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ud.9csxet.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fe.bjjhwx.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ej.yuntaijiaju.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ps.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hb.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ln.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ld.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ec.chemitech.net.cn

================================================================================
来源：http://dj.muxihuayi.cn

O. 并发与异步
来源：http://dt.szsharing.cn

================================================================================
来源：http://rh.asd995.cn

[O01] 启动一个线程
来源：http://al.asd995.cn


<!-- 参考信息 -->