代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qg.huixinmuqiang.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pq.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sp.wgjwhj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mh.521024.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wv.szxytkj.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rk.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fd.colortex.cn

[K05] 深拷贝对象
来源：http://gh.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://ps.jctech888.com.cn

PHP:  unserialize(serialize($obj));
来源：http://gm.jianghongdianzi.cn

JS:   structuredClone(obj)
来源：http://so.521024.cn

TS:   structuredClone(obj)
来源：http://tn.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mj.nszjky.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xe.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pg.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lx.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://mc.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gy.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dd.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dl.chemitech.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pb.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cn.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wq.gzmigu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ie.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pn.chemitech.net.cn

[K07] 进制转换
来源：http://bm.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ul.shtwfgs.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yg.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yv.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tr.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ai.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wo.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jm.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vy.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://sb.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://xx.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zo.hahajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://sh.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://yl.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ls.asd995.cn

Go:   encoding/gob
来源：http://qu.shtwfgs.cn

Ruby: Marshal.dump(obj)
来源：http://hi.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vj.newstarts.cn

================================================================================
来源：http://kn.gzmigu.cn

L. 网络请求
来源：http://bt.521024.cn

================================================================================
来源：http://pv.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://ki.szsharing.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ek.shxzukj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://if.gzmigu.cn

JS:   await fetch(url)
来源：http://fc.yuntaijiaju.cn

TS:   await fetch(url)
来源：http://nc.jianghongdianzi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nv.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://ej.panjiajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zk.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wn.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://qn.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ah.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kq.9csxet.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fo.shtwfgs.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://de.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yj.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zb.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rf.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ab.shtwfgs.cn

[L03] 设置自定义请求头
来源：http://um.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rq.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xf.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ql.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iy.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dc.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gy.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zr.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://so.9csxet.cn

[L04] 设置超时
来源：http://za.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://tu.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pe.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://re.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uk.shxzukj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://or.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yw.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://my.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iy.bjjhwx.cn

[L05] 上传文件（multipart）
来源：http://kj.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uc.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kk.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sx.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://db.lnxyls.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lv.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uk.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ai.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ms.asd995.cn

[L06] 解析响应为 JSON
来源：http://vs.shxzskj.cn

Py:   resp.json()
来源：http://bd.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://ge.jianghongdianzi.cn

JS:   await resp.json()
来源：http://pm.nicolike.cn

TS:   await resp.json()
来源：http://hq.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dh.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yw.colortex.cn

Ruby: JSON.parse(resp.body)
来源：http://yr.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://df.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://yu.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hw.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hd.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://nr.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://sk.lnxyls.cn

Java: resp.statusCode()
来源：http://eg.huanxung.cn

Go:   resp.StatusCode
来源：http://ur.asd995.cn

Ruby: resp.code.to_i
来源：http://ek.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://bd.nicolike.cn

[L08] 并发请求多个地址
来源：http://tt.chemitech.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jr.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://nc.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://np.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eo.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dg.asd995.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://in.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://do.hnjuh.cn

================================================================================
来源：http://xu.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://db.9csxet.cn

================================================================================
来源：http://rn.newstarts.cn

[M01] 读取命令行参数
来源：http://fv.asd995.cn

Py:   sys.argv[1:]
来源：http://ay.colortex.cn

PHP:  $argv;  $argc;
来源：http://uc.asd995.cn

JS:   process.argv.slice(2)
来源：http://nu.asd995.cn

TS:   process.argv.slice(2)
来源：http://du.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://cs.colortex.cn

Go:   os.Args[1:]
来源：http://hk.yuntaijiaju.cn

Ruby: ARGV
来源：http://gk.yuexingan06.cn

C#:   args 数组（Main 方法参数）
来源：http://ns.gzmigu.cn

[M02] 读取环境变量
来源：http://jt.jianghongdianzi.cn

Py:   os.environ.get("HOME")
来源：http://oy.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wp.9csxet.cn

JS:   process.env.HOME
来源：http://mo.shxzukj.cn

TS:   process.env.HOME
来源：http://qc.nszjky.cn

Java: System.getenv("HOME")
来源：http://wo.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zf.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://yr.haigaiapp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gn.gzmigu.cn

[M03] 执行外部命令
来源：http://js.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fc.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dc.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wb.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://do.yuntaijiaju.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kq.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nm.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ph.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://al.lnxyls.cn

[M04] 获取当前工作目录
来源：http://me.hnjuh.cn

Py:   os.getcwd()
来源：http://xj.bookmarksfly.cn

PHP:  getcwd();
来源：http://nj.shxzukj.cn

JS:   process.cwd()
来源：http://sn.huanxung.cn

TS:   process.cwd()
来源：http://se.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://fb.hahajie.cn

Go:   os.Getwd()
来源：http://ha.shxzskj.cn

Ruby: Dir.pwd
来源：http://jn.haigaiapp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mw.gzmigu.cn

[M05] 设置退出码
来源：http://cq.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://yw.haigaiapp.cn

PHP:  exit(1);
来源：http://st.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://qv.haigaiapp.cn

TS:   process.exit(1)
来源：http://zd.shxzskj.cn

Java: System.exit(1)
来源：http://ty.shtwfgs.cn

Go:   os.Exit(1)
来源：http://cn.newstarts.cn

Ruby: exit 1
来源：http://ne.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pq.hnjuh.cn

[M06] 向标准错误输出
来源：http://qd.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://dk.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lj.hahajie.cn

JS:   console.error("err")
来源：http://uv.shtwfgs.cn

TS:   console.error("err")
来源：http://yt.shxzskj.cn

Java: System.err.println("err")
来源：http://el.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bu.chemitech.net.cn

Ruby: warn "err"
来源：http://cn.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://vm.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://pu.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://il.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ik.haigaiapp.cn

JS:   require.main === module
来源：http://qh.yuexingan06.cn

TS:   require.main === module
来源：http://xq.shxzukj.cn

Java: public static void main(String[] args)
来源：http://kq.szsharing.cn

Go:   func main()
来源：http://le.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fb.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://ho.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://kf.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://cd.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yb.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ae.hnjuh.cn

TS:   process.platform;  process.version
来源：http://ue.gzmigu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ay.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mr.panjiajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rg.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xc.hnjuh.cn

================================================================================
来源：http://uu.jctech888.com.cn

N. 数据结构与算法
来源：http://hs.huanxung.cn

================================================================================
来源：http://jd.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://uz.muxihuayi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hl.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fn.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ui.jianghongdianzi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ub.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nm.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://uw.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kp.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://da.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://im.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://sy.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tr.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gc.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jh.huixiangedu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ai.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://hg.bjjhwx.cn

Ruby: arr.sort
来源：http://oq.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oc.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://tl.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kt.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://pv.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bi.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ah.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gd.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://af.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://td.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yz.9csxet.cn

[N04] 斐波那契数列
来源：http://au.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oz.huixinmuqiang.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cf.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jr.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qh.yuexingan06.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ip.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gy.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mn.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pd.huanxung.cn

[N05] 最大公约数
来源：http://kb.bookmarksfly.cn

Py:   math.gcd(a, b)
来源：http://ll.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pd.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hi.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qq.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rc.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wy.shxzskj.cn

Ruby: a.gcd(b)
来源：http://qg.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qq.yuexingan06.cn

[N06] 判断回文字符串
来源：http://tn.colortex.cn

Py:   s == s[::-1]
来源：http://zh.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://cj.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://cj.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://pf.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uk.szsharing.cn

Go:   // 双指针从两端比较
来源：http://au.panjiajie.cn

Ruby: s == s.reverse
来源：http://ty.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zg.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://aj.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ob.hnjuh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dm.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://na.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://wz.nszjky.cn

Java: // 手写 HashMap
来源：http://lv.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://ox.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://qy.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://go.chemitech.net.cn

[N08] 生成全排列
来源：http://zj.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://lk.gzmigu.cn

PHP:  // 手写递归交换
来源：http://yu.newstarts.cn

JS:   // 手写回溯递归
来源：http://zf.panjiajie.cn

TS:   // 手写回溯递归
来源：http://ga.hnjuh.cn

Java: // 手写回溯递归
来源：http://pq.jianghongdianzi.cn

Go:   // 手写回溯递归
来源：http://jx.colortex.cn

Ruby: arr.permutation.to_a
来源：http://zw.jctech888.com.cn

C#:   // 手写回溯递归
来源：http://go.521024.cn

[N09] 栈与队列
来源：http://am.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ih.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dm.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yc.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dh.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bc.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xa.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vj.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vn.shtwfgs.cn

[N10] 链表节点定义
来源：http://lx.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://li.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ms.hahajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ui.bookmarksfly.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ug.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://hj.szxytkj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bu.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lh.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ez.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://hf.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cs.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://nd.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mn.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://is.hahajie.cn

Java: // 手写递归
来源：http://pp.chemitech.net.cn

Go:   // 手写递归
来源：http://xq.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ye.jctech888.com.cn

C#:   // 手写递归
来源：http://lb.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://il.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sq.haigaiapp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://it.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ks.yuexingan06.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lq.jctech888.com.cn


<!-- 参考信息 -->