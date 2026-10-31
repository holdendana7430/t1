代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://op.hahajie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sr.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://du.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lk.colortex.cn

[K06] 解析 URL 查询串
来源：http://bb.hnjuh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ap.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zj.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fd.newstarts.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ib.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qe.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fk.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bo.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://se.asd995.cn

[K07] 进制转换
来源：http://jo.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://il.huanxung.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dc.huixinmuqiang.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cj.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://en.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oe.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kb.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cv.shxzskj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aj.bjjhwx.cn

[K08] 二进制序列化（非 JSON）
来源：http://jz.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://xc.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cz.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://xn.jctech888.com.cn

TS:   v8.serialize(obj)        // Node
来源：http://ar.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kw.szxytkj.cn

Go:   encoding/gob
来源：http://ii.lnxyls.cn

Ruby: Marshal.dump(obj)
来源：http://ed.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sw.nicolike.cn

================================================================================
来源：http://dm.shxzukj.cn

L. 网络请求
来源：http://lf.shxzskj.cn

================================================================================
来源：http://tl.huanxung.cn

[L01] 发送 GET 请求
来源：http://qj.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tt.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ul.haigaiapp.cn

JS:   await fetch(url)
来源：http://ne.hnjuh.cn

TS:   await fetch(url)
来源：http://in.panjiajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ff.yuexingan06.cn

Go:   resp, err := http.Get(url)
来源：http://gt.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kr.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fc.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://ey.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xi.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zq.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nc.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qs.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ry.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gu.yuntaijiaju.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://io.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ds.shxzskj.cn

[L03] 设置自定义请求头
来源：http://es.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hs.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rg.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sq.shxzukj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hi.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bk.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lx.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pg.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ph.hahajie.cn

[L04] 设置超时
来源：http://jo.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://ft.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jb.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sb.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vi.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jg.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hs.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tf.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pj.nicolike.cn

[L05] 上传文件（multipart）
来源：http://tg.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fe.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vh.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lo.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wt.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tz.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tu.muxihuayi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sw.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sr.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://nc.asd995.cn

Py:   resp.json()
来源：http://me.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://qf.haigaiapp.cn

JS:   await resp.json()
来源：http://lt.panjiajie.cn

TS:   await resp.json()
来源：http://ix.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ra.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rj.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://uf.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xg.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://vc.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jj.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wu.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://yb.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://xh.haigaiapp.cn

Java: resp.statusCode()
来源：http://ed.521024.cn

Go:   resp.StatusCode
来源：http://qc.yuntaijiaju.cn

Ruby: resp.code.to_i
来源：http://hs.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://tw.shxzskj.cn

[L08] 并发请求多个地址
来源：http://pp.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qn.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://tm.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aw.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oc.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ce.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ev.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mi.szxytkj.cn

================================================================================
来源：http://wf.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://dz.lnxyls.cn

================================================================================
来源：http://wh.shxzukj.cn

[M01] 读取命令行参数
来源：http://ms.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://gg.nicolike.cn

PHP:  $argv;  $argc;
来源：http://be.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://eq.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://du.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://zd.gzmigu.cn

Go:   os.Args[1:]
来源：http://to.shxzukj.cn

Ruby: ARGV
来源：http://rw.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://sd.lnxyls.cn

[M02] 读取环境变量
来源：http://lv.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://io.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qo.haigaiapp.cn

JS:   process.env.HOME
来源：http://hu.wgjwhj.cn

TS:   process.env.HOME
来源：http://ai.shxzskj.cn

Java: System.getenv("HOME")
来源：http://kk.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gx.nszjky.cn

Ruby: ENV["HOME"]
来源：http://mp.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ce.gzmigu.cn

[M03] 执行外部命令
来源：http://qq.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yj.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ni.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ba.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tv.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qf.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gh.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://td.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://eu.hahajie.cn

[M04] 获取当前工作目录
来源：http://gt.wgjwhj.cn

Py:   os.getcwd()
来源：http://sg.shtwfgs.cn

PHP:  getcwd();
来源：http://od.shxzskj.cn

JS:   process.cwd()
来源：http://bv.huanxung.cn

TS:   process.cwd()
来源：http://ju.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://jg.nicolike.cn

Go:   os.Getwd()
来源：http://mg.colortex.cn

Ruby: Dir.pwd
来源：http://mm.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xm.bjjhwx.cn

[M05] 设置退出码
来源：http://zi.yuexingan06.cn

Py:   sys.exit(1)
来源：http://yj.szxytkj.cn

PHP:  exit(1);
来源：http://ki.huanxung.cn

JS:   process.exit(1)
来源：http://rs.521024.cn

TS:   process.exit(1)
来源：http://qo.shxzskj.cn

Java: System.exit(1)
来源：http://it.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://ra.asd995.cn

Ruby: exit 1
来源：http://ht.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zu.szxytkj.cn

[M06] 向标准错误输出
来源：http://it.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://wz.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://di.bookmarksfly.cn

JS:   console.error("err")
来源：http://mt.colortex.cn

TS:   console.error("err")
来源：http://uw.nicolike.cn

Java: System.err.println("err")
来源：http://tq.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hn.wgjwhj.cn

Ruby: warn "err"
来源：http://ij.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ae.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://yg.521024.cn

Py:   if __name__ == "__main__":
来源：http://cr.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ob.chemitech.net.cn

JS:   require.main === module
来源：http://vx.newstarts.cn

TS:   require.main === module
来源：http://ek.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://bu.szsharing.cn

Go:   func main()
来源：http://mz.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ut.jianghongdianzi.cn

C#:   static void Main(string[] args)
来源：http://lk.shxzskj.cn

[M08] 获取系统与运行时信息
来源：http://eg.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ee.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ww.shxzskj.cn

JS:   process.platform;  process.version
来源：http://lz.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://ab.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wp.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wg.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ot.bookmarksfly.cn

================================================================================
来源：http://sk.521024.cn

N. 数据结构与算法
来源：http://fb.huanxung.cn

================================================================================
来源：http://pt.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://uc.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aa.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gn.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tx.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tu.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jy.9csxet.cn

Go:   sort.SearchInts(arr, x)
来源：http://uk.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ef.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ar.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://av.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://yv.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://et.yuntaijiaju.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sr.bjjhwx.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oa.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ff.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://vg.shxzskj.cn

Ruby: arr.sort
来源：http://vr.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ng.nszjky.cn

[N03] 快速排序（分治示例）
来源：http://oz.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ug.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://hj.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rz.nszjky.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rt.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uy.9csxet.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rq.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gp.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wg.shxzskj.cn

[N04] 斐波那契数列
来源：http://zr.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vi.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mx.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gj.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://js.hnjuh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pp.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sp.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tj.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gr.gzmigu.cn

[N05] 最大公约数
来源：http://eu.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://ul.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ai.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qo.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uc.shxzukj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vg.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ey.9csxet.cn

Ruby: a.gcd(b)
来源：http://uz.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lj.huixiangedu.cn

[N06] 判断回文字符串
来源：http://tg.shtwfgs.cn

Py:   s == s[::-1]
来源：http://rq.huanxung.cn

PHP:  $s === strrev($s);
来源：http://dw.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://az.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://tq.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dr.wgjwhj.cn

Go:   // 双指针从两端比较
来源：http://of.szsharing.cn

Ruby: s == s.reverse
来源：http://hn.nicolike.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://eo.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://kr.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zs.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yo.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jx.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://yo.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ov.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://ri.hnjuh.cn

Ruby: // 手写 Hash
来源：http://ui.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kk.huixiangedu.cn

[N08] 生成全排列
来源：http://kn.haigaiapp.cn

Py:   itertools.permutations(arr)
来源：http://pz.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://tt.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://zl.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://qs.jianghongdianzi.cn

Java: // 手写回溯递归
来源：http://rt.huanxung.cn

Go:   // 手写回溯递归
来源：http://ei.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://ud.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://bn.panjiajie.cn

[N09] 栈与队列
来源：http://yh.gzmigu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bj.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ea.9csxet.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zb.szsharing.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mv.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xn.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eu.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nn.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mx.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://gr.hnjuh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rd.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ez.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tl.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ow.jctech888.com.cn

Java: class Node { int v; Node next; }
来源：http://mt.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zm.panjiajie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://om.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rl.huanxung.cn

[N11] 二叉树中序遍历
来源：http://rz.szsharing.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ny.colortex.cn

PHP:  // 手写递归函数
来源：http://eo.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ln.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cg.nicolike.cn

Java: // 手写递归
来源：http://rz.shxzskj.cn

Go:   // 手写递归
来源：http://br.jianghongdianzi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://in.bjjhwx.cn

C#:   // 手写递归
来源：http://mc.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ys.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://je.muxihuayi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ly.huanxung.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://py.asd995.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yh.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ap.chemitech.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lh.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gr.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ox.jianghongdianzi.cn

================================================================================
来源：http://lh.panjiajie.cn

O. 并发与异步
来源：http://ba.huanxung.cn

================================================================================
来源：http://jp.lnxyls.cn

[O01] 启动一个线程
来源：http://fx.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vb.yuexingan06.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bg.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kl.newstarts.cn

TS:   // 同 JS
来源：http://ct.panjiajie.cn


<!-- 参考信息 -->