代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://xm.wgjwhj.cn

PHP:  unserialize(serialize($obj));
来源：http://ed.colortex.cn

JS:   structuredClone(obj)
来源：http://ma.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://zj.shxzskj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://if.asd995.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gh.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cg.521024.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ky.huixiangedu.cn

[K06] 解析 URL 查询串
来源：http://fs.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://to.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jd.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bo.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lc.jctech888.com.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zn.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gf.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ws.bjjhwx.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bt.huixinmuqiang.cn

[K07] 进制转换
来源：http://ih.shxzskj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wd.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ie.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iz.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nj.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ht.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ud.9csxet.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cd.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cl.muxihuayi.cn

[K08] 二进制序列化（非 JSON）
来源：http://so.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://iz.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://do.huixiangedu.cn

JS:   v8.serialize(obj)        // Node
来源：http://yt.newstarts.cn

TS:   v8.serialize(obj)        // Node
来源：http://vz.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://id.yuntaijiaju.cn

Go:   encoding/gob
来源：http://dc.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://wl.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hf.521024.cn

================================================================================
来源：http://hs.shxzskj.cn

L. 网络请求
来源：http://fo.hnjuh.cn

================================================================================
来源：http://iq.panjiajie.cn

[L01] 发送 GET 请求
来源：http://vh.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://de.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dr.haigaiapp.cn

JS:   await fetch(url)
来源：http://kz.gzmigu.cn

TS:   await fetch(url)
来源：http://oa.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bt.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://rx.gzmigu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qx.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rs.huanxung.cn

[L02] 发送 POST JSON
来源：http://bu.jianghongdianzi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qw.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wj.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lh.hahajie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://az.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yd.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gk.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tp.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bw.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://kv.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dz.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gq.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ns.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://et.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ud.hnjuh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jj.szxytkj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tq.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zz.shxzukj.cn

[L04] 设置超时
来源：http://mi.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://cy.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lx.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hq.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lh.lnxyls.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ps.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qg.jctech888.com.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bi.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jl.hnjuh.cn

[L05] 上传文件（multipart）
来源：http://nj.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ho.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xp.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tq.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vm.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mk.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sl.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://co.nszjky.cn

[L06] 解析响应为 JSON
来源：http://jr.szxytkj.cn

Py:   resp.json()
来源：http://wo.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://zi.9csxet.cn

JS:   await resp.json()
来源：http://tv.muxihuayi.cn

TS:   await resp.json()
来源：http://tc.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wa.9csxet.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dn.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://xg.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gb.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ci.asd995.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://se.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sq.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://lw.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://rm.yuexingan06.cn

Java: resp.statusCode()
来源：http://up.panjiajie.cn

Go:   resp.StatusCode
来源：http://kp.hnjuh.cn

Ruby: resp.code.to_i
来源：http://rh.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://as.9csxet.cn

[L08] 并发请求多个地址
来源：http://tn.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kh.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://jt.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ck.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://um.huixinmuqiang.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bz.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vk.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wn.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vd.bjjhwx.cn

================================================================================
来源：http://vo.jctech888.com.cn

M. 命令行 / 进程 / 环境
来源：http://fo.9csxet.cn

================================================================================
来源：http://ug.asd995.cn

[M01] 读取命令行参数
来源：http://rw.521024.cn

Py:   sys.argv[1:]
来源：http://sx.colortex.cn

PHP:  $argv;  $argc;
来源：http://iy.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://cm.szsharing.cn

TS:   process.argv.slice(2)
来源：http://fu.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://sc.shtwfgs.cn

Go:   os.Args[1:]
来源：http://wp.chemitech.net.cn

Ruby: ARGV
来源：http://wb.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://ab.colortex.cn

[M02] 读取环境变量
来源：http://ne.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://fq.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kp.muxihuayi.cn

JS:   process.env.HOME
来源：http://vn.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://pg.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://bb.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mo.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://ub.shxzukj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ak.huanxung.cn

[M03] 执行外部命令
来源：http://ex.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kn.nszjky.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cb.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hq.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jj.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bj.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ek.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qd.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://xb.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://dl.huanxung.cn

Py:   os.getcwd()
来源：http://nh.huanxung.cn

PHP:  getcwd();
来源：http://iq.panjiajie.cn

JS:   process.cwd()
来源：http://ey.huixinmuqiang.cn

TS:   process.cwd()
来源：http://qg.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://ww.huixinmuqiang.cn

Go:   os.Getwd()
来源：http://rf.shxzskj.cn

Ruby: Dir.pwd
来源：http://db.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gw.szxytkj.cn

[M05] 设置退出码
来源：http://hj.szsharing.cn

Py:   sys.exit(1)
来源：http://cp.lnxyls.cn

PHP:  exit(1);
来源：http://yb.9csxet.cn

JS:   process.exit(1)
来源：http://vf.gzmigu.cn

TS:   process.exit(1)
来源：http://ir.szsharing.cn

Java: System.exit(1)
来源：http://el.szxytkj.cn

Go:   os.Exit(1)
来源：http://hg.hahajie.cn

Ruby: exit 1
来源：http://uw.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yk.hnjuh.cn

[M06] 向标准错误输出
来源：http://vg.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://wt.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mt.panjiajie.cn

JS:   console.error("err")
来源：http://qh.jctech888.com.cn

TS:   console.error("err")
来源：http://aa.chemitech.net.cn

Java: System.err.println("err")
来源：http://mc.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ta.huixiangedu.cn

Ruby: warn "err"
来源：http://zb.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://eo.colortex.cn

[M07] 判断是否为主入口
来源：http://by.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://xv.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pg.yuntaijiaju.cn

JS:   require.main === module
来源：http://mx.bjjhwx.cn

TS:   require.main === module
来源：http://mh.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://dw.newstarts.cn

Go:   func main()
来源：http://nv.yuntaijiaju.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jj.521024.cn

C#:   static void Main(string[] args)
来源：http://bq.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://sp.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://it.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://hp.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://kd.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://rc.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ln.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qp.huixinmuqiang.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ac.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jx.szsharing.cn

================================================================================
来源：http://yd.bjjhwx.cn

N. 数据结构与算法
来源：http://ey.lnxyls.cn

================================================================================
来源：http://yb.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://um.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://re.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zc.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cw.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xh.colortex.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wu.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://my.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://of.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ou.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://lm.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://nh.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ev.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ih.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mw.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ir.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://vt.panjiajie.cn

Ruby: arr.sort
来源：http://ty.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ei.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://lz.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xd.muxihuayi.cn

PHP:  // 递归实现，或用 usort
来源：http://un.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iu.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://am.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://li.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iw.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qz.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://we.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://iz.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hj.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tj.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qd.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qw.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ig.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rj.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gp.huixiangedu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://be.bookmarksfly.cn

[N05] 最大公约数
来源：http://iu.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://gc.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qu.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nj.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qt.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kp.nszjky.cn

Ruby: a.gcd(b)
来源：http://oq.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yf.newstarts.cn

[N06] 判断回文字符串
来源：http://rw.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://tm.huanxung.cn

PHP:  $s === strrev($s);
来源：http://sc.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://vf.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://xd.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://my.521024.cn

Go:   // 双指针从两端比较
来源：http://wm.lnxyls.cn

Ruby: s == s.reverse
来源：http://iz.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pu.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://oy.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ah.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jp.hnjuh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bm.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://cc.chemitech.net.cn

Java: // 手写 HashMap
来源：http://gi.hahajie.cn

Go:   // 手写 map[int]int
来源：http://qo.gzmigu.cn

Ruby: // 手写 Hash
来源：http://ys.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qt.521024.cn

[N08] 生成全排列
来源：http://pk.521024.cn

Py:   itertools.permutations(arr)
来源：http://bg.szsharing.cn

PHP:  // 手写递归交换
来源：http://xl.9csxet.cn

JS:   // 手写回溯递归
来源：http://wg.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://bo.huixiangedu.cn

Java: // 手写回溯递归
来源：http://gc.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://ss.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://er.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://ft.hahajie.cn

[N09] 栈与队列
来源：http://sr.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ja.szxytkj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ws.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lq.colortex.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ys.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uf.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nd.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://of.lnxyls.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jv.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://bc.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://df.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kj.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rr.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mt.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://mn.yuntaijiaju.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xn.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jm.asd995.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lo.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://ca.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ov.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://eg.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ma.nicolike.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vx.jianghongdianzi.cn

Java: // 手写递归
来源：http://yg.colortex.cn

Go:   // 手写递归
来源：http://pm.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aj.colortex.cn

C#:   // 手写递归
来源：http://ea.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wp.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iw.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ot.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://au.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yi.newstarts.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cd.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sf.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qz.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cb.huanxung.cn

================================================================================
来源：http://vt.huixinmuqiang.cn

O. 并发与异步
来源：http://cu.panjiajie.cn

================================================================================
来源：http://kv.chemitech.net.cn

[O01] 启动一个线程
来源：http://jx.yuexingan06.cn


<!-- 参考信息 -->