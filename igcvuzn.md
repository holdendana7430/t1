代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hp.nszjky.cn

[K07] 进制转换
来源：http://fx.yuexingan06.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jw.szxytkj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ek.wgjwhj.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ww.yuntaijiaju.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cc.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wh.yuntaijiaju.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ql.colortex.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fx.haigaiapp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cj.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://xi.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://dl.panjiajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ij.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://kx.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://ji.szxytkj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mk.jctech888.com.cn

Go:   encoding/gob
来源：http://bp.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://fa.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aa.shxzukj.cn

================================================================================
来源：http://ku.wgjwhj.cn

L. 网络请求
来源：http://dj.huixinmuqiang.cn

================================================================================
来源：http://of.shtwfgs.cn

[L01] 发送 GET 请求
来源：http://ok.shxzukj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jt.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bi.bjjhwx.cn

JS:   await fetch(url)
来源：http://rb.muxihuayi.cn

TS:   await fetch(url)
来源：http://sp.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nz.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://op.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vx.szsharing.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kj.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://bv.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qt.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xc.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xj.huixiangedu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yv.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ub.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://od.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gg.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ir.shxzskj.cn

[L03] 设置自定义请求头
来源：http://zh.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kf.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://px.shxzskj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yb.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dh.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://if.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://do.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ec.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cr.gzmigu.cn

[L04] 设置超时
来源：http://vf.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://wp.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zp.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gx.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kt.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vo.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xw.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zt.panjiajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vf.colortex.cn

[L05] 上传文件（multipart）
来源：http://xa.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kc.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jq.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mr.jianghongdianzi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pa.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://et.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dh.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hd.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wk.nicolike.cn

[L06] 解析响应为 JSON
来源：http://xx.yuntaijiaju.cn

Py:   resp.json()
来源：http://ug.huixinmuqiang.cn

PHP:  json_decode($body, true);
来源：http://nn.szsharing.cn

JS:   await resp.json()
来源：http://ru.yuntaijiaju.cn

TS:   await resp.json()
来源：http://yf.yuexingan06.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oc.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qy.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://ce.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rp.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://ev.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uc.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wk.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://kg.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://mf.bookmarksfly.cn

Java: resp.statusCode()
来源：http://dg.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://gc.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://wb.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://bi.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://zj.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://js.hahajie.cn

PHP:  curl_multi_init() 系列
来源：http://ny.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rw.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eo.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xx.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cw.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://en.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dc.colortex.cn

================================================================================
来源：http://mn.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://rw.nszjky.cn

================================================================================
来源：http://mx.521024.cn

[M01] 读取命令行参数
来源：http://vj.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://kk.nszjky.cn

PHP:  $argv;  $argc;
来源：http://nl.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://km.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://cq.yuntaijiaju.cn

Java: args 数组（main 方法参数）
来源：http://qm.nszjky.cn

Go:   os.Args[1:]
来源：http://yx.newstarts.cn

Ruby: ARGV
来源：http://am.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://yc.bjjhwx.cn

[M02] 读取环境变量
来源：http://tf.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://wi.wgjwhj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ri.colortex.cn

JS:   process.env.HOME
来源：http://on.bjjhwx.cn

TS:   process.env.HOME
来源：http://jm.9csxet.cn

Java: System.getenv("HOME")
来源：http://ta.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eg.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://ys.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hg.shxzskj.cn

[M03] 执行外部命令
来源：http://zu.szxytkj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cx.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yr.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uc.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qw.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ty.jctech888.com.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://my.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ga.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://dp.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://hf.jctech888.com.cn

Py:   os.getcwd()
来源：http://tv.yuexingan06.cn

PHP:  getcwd();
来源：http://xv.yuexingan06.cn

JS:   process.cwd()
来源：http://qr.huixinmuqiang.cn

TS:   process.cwd()
来源：http://an.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://de.haigaiapp.cn

Go:   os.Getwd()
来源：http://bg.huanxung.cn

Ruby: Dir.pwd
来源：http://vz.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zx.shtwfgs.cn

[M05] 设置退出码
来源：http://ab.shxzukj.cn

Py:   sys.exit(1)
来源：http://hm.asd995.cn

PHP:  exit(1);
来源：http://bk.asd995.cn

JS:   process.exit(1)
来源：http://ys.nicolike.cn

TS:   process.exit(1)
来源：http://rk.huixiangedu.cn

Java: System.exit(1)
来源：http://ke.muxihuayi.cn

Go:   os.Exit(1)
来源：http://qq.521024.cn

Ruby: exit 1
来源：http://ee.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oh.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://ha.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://nx.shxzskj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xv.hnjuh.cn

JS:   console.error("err")
来源：http://pk.asd995.cn

TS:   console.error("err")
来源：http://vk.asd995.cn

Java: System.err.println("err")
来源：http://gl.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xm.muxihuayi.cn

Ruby: warn "err"
来源：http://sb.chemitech.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://kl.lnxyls.cn

[M07] 判断是否为主入口
来源：http://wo.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://mg.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://di.muxihuayi.cn

JS:   require.main === module
来源：http://ew.hnjuh.cn

TS:   require.main === module
来源：http://gd.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://lq.nszjky.cn

Go:   func main()
来源：http://gi.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kq.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://ny.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://cz.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://st.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://dl.shxzskj.cn

JS:   process.platform;  process.version
来源：http://wt.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://um.521024.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lu.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://af.szsharing.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jb.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wq.bookmarksfly.cn

================================================================================
来源：http://vg.chemitech.net.cn

N. 数据结构与算法
来源：http://er.gzmigu.cn

================================================================================
来源：http://vs.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://je.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gc.panjiajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bq.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eg.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dv.huixiangedu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ac.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://xc.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lo.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xr.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://gm.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://gn.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ho.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pl.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tl.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://si.newstarts.cn

Go:   slices.Sort(arr)
来源：http://jz.huixinmuqiang.cn

Ruby: arr.sort
来源：http://hb.jctech888.com.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ji.colortex.cn

[N03] 快速排序（分治示例）
来源：http://pl.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ho.panjiajie.cn

PHP:  // 递归实现，或用 usort
来源：http://vq.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yk.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tt.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jf.nszjky.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nr.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qn.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zf.chemitech.net.cn

[N04] 斐波那契数列
来源：http://xo.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fh.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xb.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vs.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ru.wgjwhj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ap.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ir.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ts.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ic.muxihuayi.cn

[N05] 最大公约数
来源：http://ra.nszjky.cn

Py:   math.gcd(a, b)
来源：http://sg.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://io.jctech888.com.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://do.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://im.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nf.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ol.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://ku.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xz.chemitech.net.cn

[N06] 判断回文字符串
来源：http://mi.chemitech.net.cn

Py:   s == s[::-1]
来源：http://jo.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://ok.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://bq.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://kh.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wf.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://io.shtwfgs.cn

Ruby: s == s.reverse
来源：http://fk.huanxung.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ob.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://ae.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fj.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lx.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cf.shxzukj.cn

TS:   // 手写 Map<string, number>
来源：http://yf.yuexingan06.cn

Java: // 手写 HashMap
来源：http://mo.szsharing.cn

Go:   // 手写 map[int]int
来源：http://fp.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://yg.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yv.szxytkj.cn

[N08] 生成全排列
来源：http://zl.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://mj.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://zc.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://ax.gzmigu.cn

TS:   // 手写回溯递归
来源：http://mx.chemitech.net.cn

Java: // 手写回溯递归
来源：http://ta.nicolike.cn

Go:   // 手写回溯递归
来源：http://zr.haigaiapp.cn

Ruby: arr.permutation.to_a
来源：http://vr.521024.cn

C#:   // 手写回溯递归
来源：http://ab.lnxyls.cn

[N09] 栈与队列
来源：http://zl.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yi.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pa.yuntaijiaju.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ay.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://na.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vy.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://el.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wt.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qo.9csxet.cn

[N10] 链表节点定义
来源：http://od.colortex.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kz.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lo.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cz.jianghongdianzi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ii.521024.cn

Java: class Node { int v; Node next; }
来源：http://ta.newstarts.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nu.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bj.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ej.shxzskj.cn

[N11] 二叉树中序遍历
来源：http://cf.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fn.shxzskj.cn

PHP:  // 手写递归函数
来源：http://mk.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kh.shtwfgs.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://br.colortex.cn

Java: // 手写递归
来源：http://uk.wgjwhj.cn

Go:   // 手写递归
来源：http://fr.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ue.jctech888.com.cn

C#:   // 手写递归
来源：http://ra.jianghongdianzi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uu.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pi.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ol.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ly.szsharing.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qu.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pq.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dm.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zf.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dt.shtwfgs.cn

================================================================================
来源：http://hj.hahajie.cn

O. 并发与异步
来源：http://lj.lnxyls.cn

================================================================================
来源：http://yo.shxzukj.cn

[O01] 启动一个线程
来源：http://xd.huixiangedu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rr.bjjhwx.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ym.haigaiapp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wo.bjjhwx.cn

TS:   // 同 JS
来源：http://sd.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://wg.shtwfgs.cn

Go:   go f()
来源：http://ie.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://ro.newstarts.cn

C#:   Task.Run(() => F());
来源：http://kg.colortex.cn

[O02] 使用线程池
来源：http://gj.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bt.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dw.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wy.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://ii.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tx.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tk.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rp.muxihuayi.cn


<!-- 参考信息 -->