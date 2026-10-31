代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://nf.shxzukj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sf.hahajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rp.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jv.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://oe.szxytkj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cy.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://no.shxzskj.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ak.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bs.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vs.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yp.panjiajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wf.panjiajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uu.huixinmuqiang.cn

[K07] 进制转换
来源：http://tw.shxzukj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://el.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gk.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tm.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tu.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vi.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ns.szxytkj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xp.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://if.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://li.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://cq.haigaiapp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kk.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://ed.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://hl.521024.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://id.panjiajie.cn

Go:   encoding/gob
来源：http://uk.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://kw.asd995.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ua.haigaiapp.cn

================================================================================
来源：http://eu.newstarts.cn

L. 网络请求
来源：http://id.9csxet.cn

================================================================================
来源：http://ti.nicolike.cn

[L01] 发送 GET 请求
来源：http://kv.521024.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tq.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ka.wgjwhj.cn

JS:   await fetch(url)
来源：http://fq.bjjhwx.cn

TS:   await fetch(url)
来源：http://gv.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://il.panjiajie.cn

Go:   resp, err := http.Get(url)
来源：http://yq.9csxet.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jw.muxihuayi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cw.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://cz.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uu.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kb.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gf.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ps.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bs.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lq.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zr.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ct.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://bt.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cx.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ue.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nr.chemitech.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xi.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zr.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uj.asd995.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gp.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lf.gzmigu.cn

[L04] 设置超时
来源：http://gt.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://ci.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://td.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nz.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jd.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tg.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fy.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pq.colortex.cn

[L05] 上传文件（multipart）
来源：http://ot.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vd.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uc.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://us.nicolike.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zf.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kx.wgjwhj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sf.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fh.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qv.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://bh.wgjwhj.cn

Py:   resp.json()
来源：http://tz.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://fq.panjiajie.cn

JS:   await resp.json()
来源：http://qm.bookmarksfly.cn

TS:   await resp.json()
来源：http://ra.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dz.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ce.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://vz.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oa.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://pl.jianghongdianzi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wb.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tt.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://lr.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://og.bjjhwx.cn

Java: resp.statusCode()
来源：http://lh.shxzukj.cn

Go:   resp.StatusCode
来源：http://xw.colortex.cn

Ruby: resp.code.to_i
来源：http://hq.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://ek.szxytkj.cn

[L08] 并发请求多个地址
来源：http://lh.nszjky.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tg.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://tq.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mk.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pv.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hh.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aq.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zm.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cb.shxzukj.cn

================================================================================
来源：http://fg.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://yi.bjjhwx.cn

================================================================================
来源：http://st.chemitech.net.cn

[M01] 读取命令行参数
来源：http://sv.hahajie.cn

Py:   sys.argv[1:]
来源：http://al.colortex.cn

PHP:  $argv;  $argc;
来源：http://so.huixiangedu.cn

JS:   process.argv.slice(2)
来源：http://qu.bjjhwx.cn

TS:   process.argv.slice(2)
来源：http://ly.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://mv.521024.cn

Go:   os.Args[1:]
来源：http://mt.yuntaijiaju.cn

Ruby: ARGV
来源：http://av.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://dx.lnxyls.cn

[M02] 读取环境变量
来源：http://ac.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://ij.lnxyls.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dk.nszjky.cn

JS:   process.env.HOME
来源：http://mj.panjiajie.cn

TS:   process.env.HOME
来源：http://qb.shxzukj.cn

Java: System.getenv("HOME")
来源：http://un.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ak.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://mz.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nd.yuntaijiaju.cn

[M03] 执行外部命令
来源：http://ov.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kt.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://je.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yq.hahajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xr.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ta.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hf.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hh.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://oo.shxzskj.cn

[M04] 获取当前工作目录
来源：http://nn.huixiangedu.cn

Py:   os.getcwd()
来源：http://sb.chemitech.net.cn

PHP:  getcwd();
来源：http://jb.yuntaijiaju.cn

JS:   process.cwd()
来源：http://uf.newstarts.cn

TS:   process.cwd()
来源：http://vq.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://nf.szxytkj.cn

Go:   os.Getwd()
来源：http://ks.chemitech.net.cn

Ruby: Dir.pwd
来源：http://ew.shtwfgs.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dx.hnjuh.cn

[M05] 设置退出码
来源：http://kr.yuexingan06.cn

Py:   sys.exit(1)
来源：http://zu.shtwfgs.cn

PHP:  exit(1);
来源：http://pg.huanxung.cn

JS:   process.exit(1)
来源：http://vu.huanxung.cn

TS:   process.exit(1)
来源：http://qv.huixiangedu.cn

Java: System.exit(1)
来源：http://rv.huanxung.cn

Go:   os.Exit(1)
来源：http://av.asd995.cn

Ruby: exit 1
来源：http://ig.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ba.jctech888.com.cn

[M06] 向标准错误输出
来源：http://zc.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://os.huixiangedu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hy.gzmigu.cn

JS:   console.error("err")
来源：http://vd.wgjwhj.cn

TS:   console.error("err")
来源：http://dg.szsharing.cn

Java: System.err.println("err")
来源：http://ch.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qw.bookmarksfly.cn

Ruby: warn "err"
来源：http://dz.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://am.nszjky.cn

[M07] 判断是否为主入口
来源：http://re.haigaiapp.cn

Py:   if __name__ == "__main__":
来源：http://fa.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vc.nszjky.cn

JS:   require.main === module
来源：http://sj.jctech888.com.cn

TS:   require.main === module
来源：http://gf.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://qp.bookmarksfly.cn

Go:   func main()
来源：http://lm.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gb.newstarts.cn

C#:   static void Main(string[] args)
来源：http://tx.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://ie.nicolike.cn

Py:   platform.system();  platform.python_version()
来源：http://pz.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://tf.shxzskj.cn

JS:   process.platform;  process.version
来源：http://hb.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://yw.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gb.shtwfgs.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rs.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yt.521024.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xz.yuntaijiaju.cn

================================================================================
来源：http://sa.newstarts.cn

N. 数据结构与算法
来源：http://ue.wgjwhj.cn

================================================================================
来源：http://vg.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://ne.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bc.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://on.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uh.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nd.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jj.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://op.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://id.panjiajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ug.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://do.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://me.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yj.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fq.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kf.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ee.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://wd.nszjky.cn

Ruby: arr.sort
来源：http://wg.asd995.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ky.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://av.lnxyls.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wi.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://fw.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://as.hahajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xo.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rq.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jd.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vn.wgjwhj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sa.nicolike.cn

[N04] 斐波那契数列
来源：http://na.hnjuh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uw.bjjhwx.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vz.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cl.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://md.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zw.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xo.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tp.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qb.jctech888.com.cn

[N05] 最大公约数
来源：http://ak.colortex.cn

Py:   math.gcd(a, b)
来源：http://no.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rz.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nl.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ic.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pz.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qr.nszjky.cn

Ruby: a.gcd(b)
来源：http://jg.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zr.haigaiapp.cn

[N06] 判断回文字符串
来源：http://sz.nszjky.cn

Py:   s == s[::-1]
来源：http://wu.newstarts.cn

PHP:  $s === strrev($s);
来源：http://om.asd995.cn

JS:   s === [...s].reverse().join("")
来源：http://ry.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://sd.nicolike.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vz.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://id.szxytkj.cn

Ruby: s == s.reverse
来源：http://xt.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rk.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://bt.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://up.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jp.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dw.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://cz.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://uq.bjjhwx.cn

Go:   // 手写 map[int]int
来源：http://up.hahajie.cn

Ruby: // 手写 Hash
来源：http://bc.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ty.nicolike.cn

[N08] 生成全排列
来源：http://bv.colortex.cn

Py:   itertools.permutations(arr)
来源：http://xn.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ao.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://tm.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://gl.shxzskj.cn

Java: // 手写回溯递归
来源：http://sm.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://hw.colortex.cn

Ruby: arr.permutation.to_a
来源：http://uz.panjiajie.cn

C#:   // 手写回溯递归
来源：http://fs.panjiajie.cn

[N09] 栈与队列
来源：http://ft.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sp.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zv.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hw.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fb.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ql.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://np.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kd.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fp.bjjhwx.cn

[N10] 链表节点定义
来源：http://sl.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wn.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bq.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sf.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oc.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://pv.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://as.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fw.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mn.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://km.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nl.nicolike.cn

PHP:  // 手写递归函数
来源：http://kq.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://es.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qp.newstarts.cn

Java: // 手写递归
来源：http://zk.hnjuh.cn

Go:   // 手写递归
来源：http://oc.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://me.9csxet.cn

C#:   // 手写递归
来源：http://jk.haigaiapp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kb.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fb.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oc.jianghongdianzi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fm.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vp.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fa.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uv.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ah.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ta.gzmigu.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

O. 并发与异步
来源：http://jp.shxzskj.cn

================================================================================
来源：http://ca.521024.cn

[O01] 启动一个线程
来源：http://ny.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mp.nszjky.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kn.jctech888.com.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://en.lnxyls.cn

TS:   // 同 JS
来源：http://co.bjjhwx.cn


<!-- 参考信息 -->