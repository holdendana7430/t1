代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://ts.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cs.hnjuh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gw.lnxyls.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sv.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://wo.muxihuayi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pz.lnxyls.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yo.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ey.bjjhwx.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ho.chemitech.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://da.asd995.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ul.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gp.yuntaijiaju.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kh.szxytkj.cn

[K07] 进制转换
来源：http://kf.521024.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vn.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://le.jctech888.com.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bj.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://og.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://di.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yk.asd995.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gm.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ms.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://mp.colortex.cn

Py:   pickle.dumps(obj)
来源：http://cu.hnjuh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gi.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://ah.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://lb.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fm.bjjhwx.cn

Go:   encoding/gob
来源：http://zh.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://yr.shtwfgs.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yg.huanxung.cn

================================================================================
来源：http://xa.asd995.cn

L. 网络请求
来源：http://bf.wgjwhj.cn

================================================================================
来源：http://mz.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://ri.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ee.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zl.521024.cn

JS:   await fetch(url)
来源：http://fr.wgjwhj.cn

TS:   await fetch(url)
来源：http://zb.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fy.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://dd.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lb.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ez.wgjwhj.cn

[L02] 发送 POST JSON
来源：http://rw.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://od.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xr.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kl.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lz.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bi.szxytkj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ve.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jq.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qm.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://qj.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yu.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rm.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yl.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xz.colortex.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oj.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yt.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uw.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xm.asd995.cn

[L04] 设置超时
来源：http://rq.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://aj.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://me.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mp.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ok.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iz.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ar.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rv.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://us.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://wo.shxzskj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bd.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ah.haigaiapp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ld.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://te.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rd.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yi.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ao.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nt.nicolike.cn

[L06] 解析响应为 JSON
来源：http://xo.hnjuh.cn

Py:   resp.json()
来源：http://rn.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://cd.yuexingan06.cn

JS:   await resp.json()
来源：http://ge.huixinmuqiang.cn

TS:   await resp.json()
来源：http://wr.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rn.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gv.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://yi.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://be.yuntaijiaju.cn

[L07] 处理 HTTP 状态码
来源：http://ye.szxytkj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ny.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mv.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://uu.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://tm.colortex.cn

Java: resp.statusCode()
来源：http://zf.yuexingan06.cn

Go:   resp.StatusCode
来源：http://ov.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://pa.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://jj.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://qj.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lq.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://ss.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xv.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nu.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yl.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zb.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fj.huanxung.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rw.colortex.cn

================================================================================
来源：http://nv.521024.cn

M. 命令行 / 进程 / 环境
来源：http://ac.shxzskj.cn

================================================================================
来源：http://yk.wgjwhj.cn

[M01] 读取命令行参数
来源：http://as.shxzukj.cn

Py:   sys.argv[1:]
来源：http://jq.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://up.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://oa.szsharing.cn

TS:   process.argv.slice(2)
来源：http://gj.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://gy.huanxung.cn

Go:   os.Args[1:]
来源：http://kj.jctech888.com.cn

Ruby: ARGV
来源：http://ma.yuntaijiaju.cn

C#:   args 数组（Main 方法参数）
来源：http://la.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://os.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://yp.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vx.hnjuh.cn

JS:   process.env.HOME
来源：http://uz.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://hi.nicolike.cn

Java: System.getenv("HOME")
来源：http://ju.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gc.szsharing.cn

Ruby: ENV["HOME"]
来源：http://dt.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ys.wgjwhj.cn

[M03] 执行外部命令
来源：http://jy.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yt.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gj.huixinmuqiang.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gn.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vj.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xx.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lt.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://on.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://hz.521024.cn

[M04] 获取当前工作目录
来源：http://sq.haigaiapp.cn

Py:   os.getcwd()
来源：http://sa.huanxung.cn

PHP:  getcwd();
来源：http://jr.yuntaijiaju.cn

JS:   process.cwd()
来源：http://st.yuntaijiaju.cn

TS:   process.cwd()
来源：http://vi.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://ss.nicolike.cn

Go:   os.Getwd()
来源：http://kj.haigaiapp.cn

Ruby: Dir.pwd
来源：http://zz.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kz.szsharing.cn

[M05] 设置退出码
来源：http://gg.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://sy.huixinmuqiang.cn

PHP:  exit(1);
来源：http://ne.asd995.cn

JS:   process.exit(1)
来源：http://xy.huanxung.cn

TS:   process.exit(1)
来源：http://uq.haigaiapp.cn

Java: System.exit(1)
来源：http://dx.szxytkj.cn

Go:   os.Exit(1)
来源：http://if.9csxet.cn

Ruby: exit 1
来源：http://wv.szxytkj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ss.shxzukj.cn

[M06] 向标准错误输出
来源：http://la.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://kc.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://om.muxihuayi.cn

JS:   console.error("err")
来源：http://xo.hnjuh.cn

TS:   console.error("err")
来源：http://gs.nszjky.cn

Java: System.err.println("err")
来源：http://py.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fd.szxytkj.cn

Ruby: warn "err"
来源：http://ic.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://oq.huanxung.cn

[M07] 判断是否为主入口
来源：http://ld.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://jo.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vz.shxzukj.cn

JS:   require.main === module
来源：http://tw.huanxung.cn

TS:   require.main === module
来源：http://wg.panjiajie.cn

Java: public static void main(String[] args)
来源：http://nj.shxzskj.cn

Go:   func main()
来源：http://nx.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cl.521024.cn

C#:   static void Main(string[] args)
来源：http://aj.521024.cn

[M08] 获取系统与运行时信息
来源：http://cj.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://hn.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://en.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://vk.szxytkj.cn

TS:   process.platform;  process.version
来源：http://jd.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vi.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://if.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qw.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://lc.hahajie.cn

N. 数据结构与算法
来源：http://um.wgjwhj.cn

================================================================================
来源：http://hz.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://zk.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ns.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lz.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://al.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://if.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qx.nicolike.cn

Go:   sort.SearchInts(arr, x)
来源：http://vn.colortex.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ri.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ju.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://rx.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ot.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://in.newstarts.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qc.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bb.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://se.huanxung.cn

Go:   slices.Sort(arr)
来源：http://bz.hnjuh.cn

Ruby: arr.sort
来源：http://bc.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ju.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://wo.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://td.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ht.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qz.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://up.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hh.yuexingan06.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hj.shtwfgs.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ea.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vz.colortex.cn

[N04] 斐波那契数列
来源：http://fm.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://in.panjiajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ml.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cf.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pz.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lv.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wi.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gs.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ow.wgjwhj.cn

[N05] 最大公约数
来源：http://dv.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://oz.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dh.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ur.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://br.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hk.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vt.colortex.cn

Ruby: a.gcd(b)
来源：http://ee.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jp.shxzukj.cn

[N06] 判断回文字符串
来源：http://gg.shxzukj.cn

Py:   s == s[::-1]
来源：http://zk.colortex.cn

PHP:  $s === strrev($s);
来源：http://bk.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://dt.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://ki.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://od.9csxet.cn

Go:   // 双指针从两端比较
来源：http://vr.9csxet.cn

Ruby: s == s.reverse
来源：http://pn.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vv.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://jn.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rt.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cy.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sf.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://yv.colortex.cn

Java: // 手写 HashMap
来源：http://sz.hahajie.cn

Go:   // 手写 map[int]int
来源：http://kk.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://ls.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wg.jctech888.com.cn

[N08] 生成全排列
来源：http://ev.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://ex.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://uz.9csxet.cn

JS:   // 手写回溯递归
来源：http://jf.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://wb.chemitech.net.cn

Java: // 手写回溯递归
来源：http://ef.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://bz.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://fw.gzmigu.cn

C#:   // 手写回溯递归
来源：http://de.hahajie.cn

[N09] 栈与队列
来源：http://cp.hnjuh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xr.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xu.bjjhwx.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wm.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ag.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ot.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://da.nszjky.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ds.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lq.shtwfgs.cn

[N10] 链表节点定义
来源：http://mo.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bk.newstarts.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ji.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vi.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mk.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://ei.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hv.shxzskj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gp.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ty.bookmarksfly.cn

[N11] 二叉树中序遍历
来源：http://zx.bookmarksfly.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sd.szxytkj.cn

PHP:  // 手写递归函数
来源：http://qt.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qj.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pt.colortex.cn

Java: // 手写递归
来源：http://ur.gzmigu.cn

Go:   // 手写递归
来源：http://ri.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cd.newstarts.cn

C#:   // 手写递归
来源：http://ff.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ex.nszjky.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ts.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pk.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tw.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pn.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yz.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hf.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wl.chemitech.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mv.hahajie.cn

================================================================================
来源：http://ro.bjjhwx.cn

O. 并发与异步
来源：http://jt.asd995.cn

================================================================================
来源：http://nr.shxzskj.cn

[O01] 启动一个线程
来源：http://ie.shxzukj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://db.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bc.panjiajie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rl.jianghongdianzi.cn

TS:   // 同 JS
来源：http://cc.jctech888.com.cn


<!-- 参考信息 -->