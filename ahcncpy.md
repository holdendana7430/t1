代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rf.gzmigu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gr.yuntaijiaju.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kq.newstarts.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hi.chemitech.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wk.shtwfgs.cn

[K07] 进制转换
来源：http://rv.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wl.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oy.huanxung.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cy.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dx.jctech888.com.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ma.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wo.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gf.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kl.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://kc.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://qy.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cg.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://st.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://pt.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xq.huixinmuqiang.cn

Go:   encoding/gob
来源：http://aq.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://sb.shxzskj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fg.9csxet.cn

================================================================================
来源：http://dz.newstarts.cn

L. 网络请求
来源：http://xy.shtwfgs.cn

================================================================================
来源：http://yu.chemitech.net.cn

[L01] 发送 GET 请求
来源：http://bq.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ix.chemitech.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ag.shxzukj.cn

JS:   await fetch(url)
来源：http://zt.jctech888.com.cn

TS:   await fetch(url)
来源：http://mi.lnxyls.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://na.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ac.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vv.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pc.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://vg.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zs.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ag.bjjhwx.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hp.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wn.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ey.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fd.nicolike.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tm.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ok.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://ap.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qn.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xf.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sd.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cq.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://az.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kb.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sz.bjjhwx.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://th.bjjhwx.cn

[L04] 设置超时
来源：http://pl.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://qa.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pr.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qk.newstarts.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gk.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://at.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ks.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://db.colortex.cn

[L05] 上传文件（multipart）
来源：http://ql.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iw.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xb.shxzskj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ta.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lx.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tu.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gn.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yg.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kg.nicolike.cn

[L06] 解析响应为 JSON
来源：http://ie.gzmigu.cn

Py:   resp.json()
来源：http://su.szsharing.cn

PHP:  json_decode($body, true);
来源：http://di.yuexingan06.cn

JS:   await resp.json()
来源：http://hb.yuexingan06.cn

TS:   await resp.json()
来源：http://ns.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tx.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://li.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://xy.szsharing.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xq.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://ea.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ep.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ek.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://nw.yuexingan06.cn

TS:   resp.ok;  resp.status
来源：http://bi.lnxyls.cn

Java: resp.statusCode()
来源：http://zp.hahajie.cn

Go:   resp.StatusCode
来源：http://ey.hnjuh.cn

Ruby: resp.code.to_i
来源：http://co.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://vd.gzmigu.cn

[L08] 并发请求多个地址
来源：http://jh.shxzukj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ue.chemitech.net.cn

PHP:  curl_multi_init() 系列
来源：http://cw.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iy.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ja.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xj.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fm.colortex.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lj.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wg.gzmigu.cn

================================================================================
来源：http://em.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://um.wgjwhj.cn

================================================================================
来源：http://dg.asd995.cn

[M01] 读取命令行参数
来源：http://rr.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://nz.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://oj.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://eq.haigaiapp.cn

TS:   process.argv.slice(2)
来源：http://ww.521024.cn

Java: args 数组（main 方法参数）
来源：http://jf.wgjwhj.cn

Go:   os.Args[1:]
来源：http://sm.huixiangedu.cn

Ruby: ARGV
来源：http://xc.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://mm.haigaiapp.cn

[M02] 读取环境变量
来源：http://lf.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://yl.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ds.wgjwhj.cn

JS:   process.env.HOME
来源：http://nr.9csxet.cn

TS:   process.env.HOME
来源：http://qc.9csxet.cn

Java: System.getenv("HOME")
来源：http://nt.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bt.asd995.cn

Ruby: ENV["HOME"]
来源：http://oh.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fg.521024.cn

[M03] 执行外部命令
来源：http://ky.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://se.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fa.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yf.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wb.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mo.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rx.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ym.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://rw.9csxet.cn

[M04] 获取当前工作目录
来源：http://md.9csxet.cn

Py:   os.getcwd()
来源：http://wf.bjjhwx.cn

PHP:  getcwd();
来源：http://nx.asd995.cn

JS:   process.cwd()
来源：http://jy.9csxet.cn

TS:   process.cwd()
来源：http://ao.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://fx.huanxung.cn

Go:   os.Getwd()
来源：http://wx.chemitech.net.cn

Ruby: Dir.pwd
来源：http://qj.nicolike.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ks.hahajie.cn

[M05] 设置退出码
来源：http://uz.lnxyls.cn

Py:   sys.exit(1)
来源：http://pc.haigaiapp.cn

PHP:  exit(1);
来源：http://ly.hahajie.cn

JS:   process.exit(1)
来源：http://lw.gzmigu.cn

TS:   process.exit(1)
来源：http://yq.gzmigu.cn

Java: System.exit(1)
来源：http://sf.huixiangedu.cn

Go:   os.Exit(1)
来源：http://bm.hnjuh.cn

Ruby: exit 1
来源：http://jr.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xt.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://ej.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://kl.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lz.9csxet.cn

JS:   console.error("err")
来源：http://is.szsharing.cn

TS:   console.error("err")
来源：http://ek.hahajie.cn

Java: System.err.println("err")
来源：http://rq.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://be.yuexingan06.cn

Ruby: warn "err"
来源：http://qo.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://ls.hahajie.cn

[M07] 判断是否为主入口
来源：http://cl.shxzukj.cn

Py:   if __name__ == "__main__":
来源：http://fc.nszjky.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lw.huixiangedu.cn

JS:   require.main === module
来源：http://jj.szxytkj.cn

TS:   require.main === module
来源：http://wf.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://lq.jctech888.com.cn

Go:   func main()
来源：http://nn.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gt.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://tt.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://fg.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://gw.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://fr.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://wh.colortex.cn

TS:   process.platform;  process.version
来源：http://at.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kj.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nb.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qz.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xz.shtwfgs.cn

================================================================================
来源：http://fj.yuntaijiaju.cn

N. 数据结构与算法
来源：http://ji.shtwfgs.cn

================================================================================
来源：http://ag.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://nu.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eo.haigaiapp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ih.bjjhwx.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nj.haigaiapp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ua.panjiajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tb.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://pt.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ni.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nw.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://hf.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://wr.jctech888.com.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tz.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ip.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pq.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zq.gzmigu.cn

Go:   slices.Sort(arr)
来源：http://ai.shxzukj.cn

Ruby: arr.sort
来源：http://mm.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lu.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://yw.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oa.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://ef.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mv.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vf.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pe.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eh.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iw.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ku.hnjuh.cn

[N04] 斐波那契数列
来源：http://kl.shtwfgs.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nw.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xi.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ts.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ad.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://li.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://el.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://px.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fz.huanxung.cn

[N05] 最大公约数
来源：http://ne.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ce.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lu.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pi.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rr.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bk.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uh.colortex.cn

Ruby: a.gcd(b)
来源：http://ri.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qj.521024.cn

[N06] 判断回文字符串
来源：http://mo.haigaiapp.cn

Py:   s == s[::-1]
来源：http://ar.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://ol.huixinmuqiang.cn

JS:   s === [...s].reverse().join("")
来源：http://jf.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://ft.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zt.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://tl.nszjky.cn

Ruby: s == s.reverse
来源：http://ff.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ce.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://qz.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bm.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vv.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wb.521024.cn

TS:   // 手写 Map<string, number>
来源：http://kk.shxzskj.cn

Java: // 手写 HashMap
来源：http://fy.szsharing.cn

Go:   // 手写 map[int]int
来源：http://ks.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://dy.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dr.hahajie.cn

[N08] 生成全排列
来源：http://xq.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://sg.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://hl.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://zx.szsharing.cn

TS:   // 手写回溯递归
来源：http://uz.chemitech.net.cn

Java: // 手写回溯递归
来源：http://np.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://gm.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://sa.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://ms.shxzukj.cn

[N09] 栈与队列
来源：http://dk.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jd.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tu.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://th.nszjky.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rr.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pu.bookmarksfly.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://it.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ws.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dm.huixiangedu.cn

[N10] 链表节点定义
来源：http://yy.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://on.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gw.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ca.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yd.shxzskj.cn

Java: class Node { int v; Node next; }
来源：http://lh.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tu.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rl.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gy.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://cn.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zp.wgjwhj.cn

PHP:  // 手写递归函数
来源：http://hs.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ho.hnjuh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yg.hahajie.cn

Java: // 手写递归
来源：http://jc.shxzukj.cn

Go:   // 手写递归
来源：http://vj.gzmigu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tr.jianghongdianzi.cn

C#:   // 手写递归
来源：http://gp.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ad.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yk.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tg.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cf.szxytkj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wo.yuexingan06.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fw.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://md.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vm.hahajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ci.szsharing.cn

================================================================================
来源：http://sf.yuexingan06.cn

O. 并发与异步
来源：http://tp.panjiajie.cn

================================================================================
来源：http://rt.yuexingan06.cn

[O01] 启动一个线程
来源：http://ba.hnjuh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wr.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rm.hnjuh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fj.shxzukj.cn

TS:   // 同 JS
来源：http://hp.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://on.nszjky.cn

Go:   go f()
来源：http://wz.huixinmuqiang.cn

Ruby: Thread.new { f }
来源：http://wo.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ki.colortex.cn

[O02] 使用线程池
来源：http://ky.shxzskj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eo.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zw.shxzskj.cn

JS:   // worker_threads 线程池
来源：http://xq.shtwfgs.cn


<!-- 参考信息 -->