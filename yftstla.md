代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yd.yuntaijiaju.cn

[K07] 进制转换
来源：http://kl.jianghongdianzi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rj.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yh.colortex.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ft.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qu.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gm.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lm.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wm.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://km.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://oo.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://qi.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://be.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://ih.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://tp.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zk.nicolike.cn

Go:   encoding/gob
来源：http://gl.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://st.szxytkj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dl.lnxyls.cn

================================================================================
来源：http://ep.9csxet.cn

L. 网络请求
来源：http://qa.haigaiapp.cn

================================================================================
来源：http://uw.lnxyls.cn

[L01] 发送 GET 请求
来源：http://fp.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wo.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ze.panjiajie.cn

JS:   await fetch(url)
来源：http://cy.shxzukj.cn

TS:   await fetch(url)
来源：http://cl.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ly.huixinmuqiang.cn

Go:   resp, err := http.Get(url)
来源：http://qu.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://at.gzmigu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://up.nszjky.cn

[L02] 发送 POST JSON
来源：http://wa.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gw.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ga.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://el.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pd.hahajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mc.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://st.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hx.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mg.521024.cn

[L03] 设置自定义请求头
来源：http://sp.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rc.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bb.lnxyls.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hg.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eb.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xk.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xq.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lq.jianghongdianzi.cn

[L04] 设置超时
来源：http://zx.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://wn.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ve.panjiajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iu.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jg.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vo.bookmarksfly.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kj.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cs.shtwfgs.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://av.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://ny.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ff.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ia.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nd.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qa.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fl.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ag.hnjuh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cn.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://om.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://tt.muxihuayi.cn

Py:   resp.json()
来源：http://mw.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://ke.jianghongdianzi.cn

JS:   await resp.json()
来源：http://kc.newstarts.cn

TS:   await resp.json()
来源：http://oi.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ci.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fr.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://py.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dd.haigaiapp.cn

[L07] 处理 HTTP 状态码
来源：http://qv.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rk.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bg.521024.cn

JS:   resp.ok;  resp.status
来源：http://mt.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://xh.panjiajie.cn

Java: resp.statusCode()
来源：http://ps.yuntaijiaju.cn

Go:   resp.StatusCode
来源：http://ma.9csxet.cn

Ruby: resp.code.to_i
来源：http://eh.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://kn.szsharing.cn

[L08] 并发请求多个地址
来源：http://ib.bookmarksfly.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hb.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://es.panjiajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rh.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ay.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://um.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gj.9csxet.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wo.szsharing.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tf.9csxet.cn

================================================================================
来源：http://ef.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://ro.haigaiapp.cn

================================================================================
来源：http://eu.nicolike.cn

[M01] 读取命令行参数
来源：http://zi.shxzukj.cn

Py:   sys.argv[1:]
来源：http://kp.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://en.colortex.cn

JS:   process.argv.slice(2)
来源：http://wh.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://qj.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://zo.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ck.hnjuh.cn

Ruby: ARGV
来源：http://ol.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://wc.huixiangedu.cn

[M02] 读取环境变量
来源：http://hl.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://yh.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ra.jctech888.com.cn

JS:   process.env.HOME
来源：http://kk.9csxet.cn

TS:   process.env.HOME
来源：http://pn.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://fe.yuntaijiaju.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ip.colortex.cn

Ruby: ENV["HOME"]
来源：http://np.bjjhwx.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gf.wgjwhj.cn

[M03] 执行外部命令
来源：http://ah.yuexingan06.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qz.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fp.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ny.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tq.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qm.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jo.huixinmuqiang.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jz.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://ij.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://cg.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://sc.lnxyls.cn

PHP:  getcwd();
来源：http://gk.colortex.cn

JS:   process.cwd()
来源：http://ad.colortex.cn

TS:   process.cwd()
来源：http://dh.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ex.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://rh.wgjwhj.cn

Ruby: Dir.pwd
来源：http://ap.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qh.yuexingan06.cn

[M05] 设置退出码
来源：http://bt.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://ff.szxytkj.cn

PHP:  exit(1);
来源：http://fc.nszjky.cn

JS:   process.exit(1)
来源：http://ec.szxytkj.cn

TS:   process.exit(1)
来源：http://bp.szsharing.cn

Java: System.exit(1)
来源：http://or.nszjky.cn

Go:   os.Exit(1)
来源：http://xc.huixinmuqiang.cn

Ruby: exit 1
来源：http://ud.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lj.bjjhwx.cn

[M06] 向标准错误输出
来源：http://pp.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://ts.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hg.nicolike.cn

JS:   console.error("err")
来源：http://pl.yuntaijiaju.cn

TS:   console.error("err")
来源：http://fn.bookmarksfly.cn

Java: System.err.println("err")
来源：http://wv.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://li.nicolike.cn

Ruby: warn "err"
来源：http://ib.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://fv.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://pb.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://gy.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ne.gzmigu.cn

JS:   require.main === module
来源：http://yn.huixinmuqiang.cn

TS:   require.main === module
来源：http://ut.huixiangedu.cn

Java: public static void main(String[] args)
来源：http://ma.jianghongdianzi.cn

Go:   func main()
来源：http://rp.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gw.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://yz.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://wl.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://ml.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://pa.hahajie.cn

JS:   process.platform;  process.version
来源：http://nn.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://ki.huixiangedu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eq.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ji.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mi.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sb.yuexingan06.cn

================================================================================
来源：http://fi.shtwfgs.cn

N. 数据结构与算法
来源：http://lr.yuexingan06.cn

================================================================================
来源：http://fd.colortex.cn

[N01] 二分查找（有序数组）
来源：http://np.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sn.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rh.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fu.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fj.newstarts.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cs.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://fv.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ti.nicolike.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vp.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://lg.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://gt.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wu.nicolike.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vb.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nc.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ug.521024.cn

Go:   slices.Sort(arr)
来源：http://gn.huixiangedu.cn

Ruby: arr.sort
来源：http://kn.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sj.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://xg.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dh.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://ks.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ep.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xm.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ps.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zm.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://se.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lj.gzmigu.cn

[N04] 斐波那契数列
来源：http://gy.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qk.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://le.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zs.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ro.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hk.nicolike.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nh.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ny.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cb.szxytkj.cn

[N05] 最大公约数
来源：http://qg.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://md.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://um.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kg.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ft.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lb.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jb.lnxyls.cn

Ruby: a.gcd(b)
来源：http://oe.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://md.shxzskj.cn

[N06] 判断回文字符串
来源：http://qz.lnxyls.cn

Py:   s == s[::-1]
来源：http://xn.szsharing.cn

PHP:  $s === strrev($s);
来源：http://yh.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://jb.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://vb.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://os.lnxyls.cn

Go:   // 双指针从两端比较
来源：http://kl.muxihuayi.cn

Ruby: s == s.reverse
来源：http://oi.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kb.asd995.cn

[N07] 两数之和（返回下标）
来源：http://dr.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bu.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fb.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cx.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://in.gzmigu.cn

Java: // 手写 HashMap
来源：http://xo.hahajie.cn

Go:   // 手写 map[int]int
来源：http://fd.asd995.cn

Ruby: // 手写 Hash
来源：http://uw.521024.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bi.hnjuh.cn

[N08] 生成全排列
来源：http://fh.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://al.shxzukj.cn

PHP:  // 手写递归交换
来源：http://mv.9csxet.cn

JS:   // 手写回溯递归
来源：http://lo.asd995.cn

TS:   // 手写回溯递归
来源：http://pf.shtwfgs.cn

Java: // 手写回溯递归
来源：http://lo.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://ez.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://qs.hnjuh.cn

C#:   // 手写回溯递归
来源：http://hu.huixiangedu.cn

[N09] 栈与队列
来源：http://ow.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aa.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oc.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jw.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dz.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nh.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jo.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vw.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vr.hahajie.cn

[N10] 链表节点定义
来源：http://lg.bjjhwx.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ga.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://po.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ha.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jt.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://rb.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wk.nszjky.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lr.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ph.bjjhwx.cn

[N11] 二叉树中序遍历
来源：http://sv.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lz.asd995.cn

PHP:  // 手写递归函数
来源：http://rb.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ow.huixinmuqiang.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vw.bookmarksfly.cn

Java: // 手写递归
来源：http://hw.hnjuh.cn

Go:   // 手写递归
来源：http://qz.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gs.nicolike.cn

C#:   // 手写递归
来源：http://af.huixinmuqiang.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bk.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hf.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hv.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ru.hahajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bk.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zi.shxzukj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jw.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wo.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.chemitech.net.cn

================================================================================
来源：http://mf.shxzskj.cn

O. 并发与异步
来源：http://wv.asd995.cn

================================================================================
来源：http://yf.szsharing.cn

[O01] 启动一个线程
来源：http://oh.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wj.chemitech.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oa.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kg.asd995.cn

TS:   // 同 JS
来源：http://nb.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://wh.hahajie.cn

Go:   go f()
来源：http://nw.nszjky.cn

Ruby: Thread.new { f }
来源：http://zd.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://kh.521024.cn

[O02] 使用线程池
来源：http://ih.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jl.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://by.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://lp.huanxung.cn

TS:   // worker_threads 线程池
来源：http://hw.hnjuh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xe.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bv.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nf.hnjuh.cn


<!-- 参考信息 -->