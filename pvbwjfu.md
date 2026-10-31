代发 wailian999

[K06] 解析 URL 查询串
来源：http://lq.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eh.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dr.lnxyls.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rt.lnxyls.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://du.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lz.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mw.haigaiapp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cb.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zu.szxytkj.cn

[K07] 进制转换
来源：http://nn.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yc.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uz.yuexingan06.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oo.nicolike.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jv.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wh.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://as.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jw.asd995.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tu.huixinmuqiang.cn

[K08] 二进制序列化（非 JSON）
来源：http://cw.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://ci.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hd.nszjky.cn

JS:   v8.serialize(obj)        // Node
来源：http://ij.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://lg.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jc.wgjwhj.cn

Go:   encoding/gob
来源：http://iq.muxihuayi.cn

Ruby: Marshal.dump(obj)
来源：http://ot.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pq.szsharing.cn

================================================================================
来源：http://et.newstarts.cn

L. 网络请求
来源：http://rn.hahajie.cn

================================================================================
来源：http://qa.hnjuh.cn

[L01] 发送 GET 请求
来源：http://nw.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kv.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mb.yuexingan06.cn

JS:   await fetch(url)
来源：http://rx.nszjky.cn

TS:   await fetch(url)
来源：http://gm.521024.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dd.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://nb.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qi.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fi.nszjky.cn

[L02] 发送 POST JSON
来源：http://vd.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nz.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://er.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jl.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rj.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ai.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ot.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gr.yuntaijiaju.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mt.szsharing.cn

[L03] 设置自定义请求头
来源：http://io.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qk.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ry.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ef.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pj.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zj.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oy.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vy.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xm.huixinmuqiang.cn

[L04] 设置超时
来源：http://lp.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://rj.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ti.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bw.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ls.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ch.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tc.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oc.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://go.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://mp.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dp.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://co.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pk.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gi.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ya.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wt.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yw.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gq.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ev.szsharing.cn

Py:   resp.json()
来源：http://fw.nicolike.cn

PHP:  json_decode($body, true);
来源：http://wc.wgjwhj.cn

JS:   await resp.json()
来源：http://tp.huixiangedu.cn

TS:   await resp.json()
来源：http://ld.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nr.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kr.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://fi.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://et.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://oz.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fk.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ml.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://ih.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://xs.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://fu.szxytkj.cn

Go:   resp.StatusCode
来源：http://vf.nicolike.cn

Ruby: resp.code.to_i
来源：http://ns.huanxung.cn

C#:   (int)resp.StatusCode
来源：http://ih.panjiajie.cn

[L08] 并发请求多个地址
来源：http://dm.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ny.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://rs.colortex.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gv.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zq.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mj.lnxyls.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pq.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nl.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zr.shxzukj.cn

================================================================================
来源：http://bp.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://dx.haigaiapp.cn

================================================================================
来源：http://ll.yuntaijiaju.cn

[M01] 读取命令行参数
来源：http://xu.colortex.cn

Py:   sys.argv[1:]
来源：http://up.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://fk.521024.cn

JS:   process.argv.slice(2)
来源：http://el.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://da.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://rz.yuexingan06.cn

Go:   os.Args[1:]
来源：http://lj.shxzukj.cn

Ruby: ARGV
来源：http://yp.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://mn.gzmigu.cn

[M02] 读取环境变量
来源：http://vb.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://mk.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vq.521024.cn

JS:   process.env.HOME
来源：http://zr.gzmigu.cn

TS:   process.env.HOME
来源：http://gr.9csxet.cn

Java: System.getenv("HOME")
来源：http://xs.panjiajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://no.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://sz.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ck.bookmarksfly.cn

[M03] 执行外部命令
来源：http://as.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ae.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gh.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wg.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dx.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ox.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ae.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bi.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://rj.colortex.cn

[M04] 获取当前工作目录
来源：http://kw.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://ix.shxzukj.cn

PHP:  getcwd();
来源：http://ec.lnxyls.cn

JS:   process.cwd()
来源：http://ka.bjjhwx.cn

TS:   process.cwd()
来源：http://ue.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://jg.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://ut.gzmigu.cn

Ruby: Dir.pwd
来源：http://ot.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xu.jctech888.com.cn

[M05] 设置退出码
来源：http://wx.hahajie.cn

Py:   sys.exit(1)
来源：http://wp.yuntaijiaju.cn

PHP:  exit(1);
来源：http://vj.wgjwhj.cn

JS:   process.exit(1)
来源：http://qg.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://gh.jianghongdianzi.cn

Java: System.exit(1)
来源：http://qy.jctech888.com.cn

Go:   os.Exit(1)
来源：http://fy.gzmigu.cn

Ruby: exit 1
来源：http://oi.yuntaijiaju.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ti.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://ij.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://nu.wgjwhj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xy.szxytkj.cn

JS:   console.error("err")
来源：http://ls.jctech888.com.cn

TS:   console.error("err")
来源：http://wt.yuexingan06.cn

Java: System.err.println("err")
来源：http://kh.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qn.chemitech.net.cn

Ruby: warn "err"
来源：http://sm.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ct.lnxyls.cn

[M07] 判断是否为主入口
来源：http://hn.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://ao.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ck.shtwfgs.cn

JS:   require.main === module
来源：http://ps.9csxet.cn

TS:   require.main === module
来源：http://lu.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://ao.bookmarksfly.cn

Go:   func main()
来源：http://zz.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kw.szsharing.cn

C#:   static void Main(string[] args)
来源：http://ae.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://jo.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://sd.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ud.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://by.nszjky.cn

TS:   process.platform;  process.version
来源：http://wu.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ml.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eh.yuntaijiaju.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kq.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lh.muxihuayi.cn

================================================================================
来源：http://py.szsharing.cn

N. 数据结构与算法
来源：http://pl.yuexingan06.cn

================================================================================
来源：http://va.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://gx.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tx.szxytkj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ih.gzmigu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xn.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dk.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://di.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://es.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ia.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aw.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://yx.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jw.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gb.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nu.huixinmuqiang.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cg.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lf.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://fm.haigaiapp.cn

Ruby: arr.sort
来源：http://pz.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qo.9csxet.cn

[N03] 快速排序（分治示例）
来源：http://pd.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pd.yuntaijiaju.cn

PHP:  // 递归实现，或用 usort
来源：http://rf.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rm.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ta.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ip.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iw.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qf.haigaiapp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jx.521024.cn

[N04] 斐波那契数列
来源：http://xg.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mz.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dc.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aj.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bv.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wi.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pa.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cs.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pr.chemitech.net.cn

[N05] 最大公约数
来源：http://ek.521024.cn

Py:   math.gcd(a, b)
来源：http://dm.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lq.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://im.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ne.bjjhwx.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pn.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bv.nicolike.cn

Ruby: a.gcd(b)
来源：http://vr.panjiajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yl.asd995.cn

[N06] 判断回文字符串
来源：http://du.jctech888.com.cn

Py:   s == s[::-1]
来源：http://fg.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://ne.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ro.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://pq.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hy.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://la.wgjwhj.cn

Ruby: s == s.reverse
来源：http://nb.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rd.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ih.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qc.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lj.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yt.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://mn.shxzskj.cn

Java: // 手写 HashMap
来源：http://bn.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://jq.hahajie.cn

Ruby: // 手写 Hash
来源：http://yc.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pl.9csxet.cn

[N08] 生成全排列
来源：http://cl.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://ot.nicolike.cn

PHP:  // 手写递归交换
来源：http://es.huanxung.cn

JS:   // 手写回溯递归
来源：http://ay.9csxet.cn

TS:   // 手写回溯递归
来源：http://yf.huixiangedu.cn

Java: // 手写回溯递归
来源：http://ni.szxytkj.cn

Go:   // 手写回溯递归
来源：http://su.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://qr.hahajie.cn

C#:   // 手写回溯递归
来源：http://cv.9csxet.cn

[N09] 栈与队列
来源：http://ri.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fa.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qc.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lg.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nf.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zz.shxzukj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uw.huixinmuqiang.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://td.szsharing.cn

[N10] 链表节点定义
来源：http://so.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://us.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://df.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ty.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ui.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://wc.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jj.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uf.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ph.szsharing.cn

[N11] 二叉树中序遍历
来源：http://tx.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yc.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://wf.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zz.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://af.shxzukj.cn

Java: // 手写递归
来源：http://bt.yuexingan06.cn

Go:   // 手写递归
来源：http://ft.yuntaijiaju.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ow.chemitech.net.cn

C#:   // 手写递归
来源：http://ep.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fr.shtwfgs.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jz.shtwfgs.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nx.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yq.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ye.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sr.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bc.bjjhwx.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://id.shxzukj.cn

================================================================================
来源：http://qv.gzmigu.cn

O. 并发与异步
来源：http://te.9csxet.cn

================================================================================
来源：http://nz.huanxung.cn

[O01] 启动一个线程
来源：http://qx.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://es.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ej.yuexingan06.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eb.haigaiapp.cn

TS:   // 同 JS
来源：http://pa.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://gu.huanxung.cn

Go:   go f()
来源：http://jc.szxytkj.cn

Ruby: Thread.new { f }
来源：http://tv.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://jt.colortex.cn


<!-- 参考信息 -->