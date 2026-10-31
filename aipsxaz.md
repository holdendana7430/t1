代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jc.huanxung.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vv.yuntaijiaju.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gm.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tj.nicolike.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gj.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ya.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://me.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://ki.bjjhwx.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zk.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://dh.muxihuayi.cn

TS:   v8.serialize(obj)        // Node
来源：http://hu.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pb.jianghongdianzi.cn

Go:   encoding/gob
来源：http://dg.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://rc.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cd.9csxet.cn

================================================================================
来源：http://sg.bookmarksfly.cn

L. 网络请求
来源：http://mc.muxihuayi.cn

================================================================================
来源：http://dn.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://jg.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rj.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xf.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://mt.wgjwhj.cn

TS:   await fetch(url)
来源：http://wb.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yf.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://kl.huanxung.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wm.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qk.hnjuh.cn

[L02] 发送 POST JSON
来源：http://av.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bi.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fm.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qm.newstarts.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yk.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nf.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yv.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zq.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oa.lnxyls.cn

[L03] 设置自定义请求头
来源：http://yt.jctech888.com.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yi.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yh.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ow.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vb.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dy.huanxung.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ig.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vd.szsharing.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hk.yuntaijiaju.cn

[L04] 设置超时
来源：http://be.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://hb.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pd.szxytkj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hf.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rm.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gc.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sj.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iy.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xd.huixiangedu.cn

[L05] 上传文件（multipart）
来源：http://gh.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fs.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ov.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pj.colortex.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zw.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://di.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://je.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jn.muxihuayi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tl.9csxet.cn

[L06] 解析响应为 JSON
来源：http://bv.szsharing.cn

Py:   resp.json()
来源：http://xn.newstarts.cn

PHP:  json_decode($body, true);
来源：http://mx.jctech888.com.cn

JS:   await resp.json()
来源：http://df.asd995.cn

TS:   await resp.json()
来源：http://hj.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nl.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cg.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://tf.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://li.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://ba.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qy.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kz.huanxung.cn

JS:   resp.ok;  resp.status
来源：http://hs.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://cw.nszjky.cn

Java: resp.statusCode()
来源：http://nd.wgjwhj.cn

Go:   resp.StatusCode
来源：http://vh.hahajie.cn

Ruby: resp.code.to_i
来源：http://pb.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://xe.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://me.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fa.huanxung.cn

PHP:  curl_multi_init() 系列
来源：http://ce.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yr.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qm.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uj.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bk.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://in.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ar.shxzukj.cn

================================================================================
来源：http://fz.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://jn.yuexingan06.cn

================================================================================
来源：http://kd.wgjwhj.cn

[M01] 读取命令行参数
来源：http://vy.521024.cn

Py:   sys.argv[1:]
来源：http://be.szsharing.cn

PHP:  $argv;  $argc;
来源：http://tc.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://eq.nicolike.cn

TS:   process.argv.slice(2)
来源：http://un.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://db.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://hi.yuexingan06.cn

Ruby: ARGV
来源：http://lp.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://nw.asd995.cn

[M02] 读取环境变量
来源：http://jv.521024.cn

Py:   os.environ.get("HOME")
来源：http://bu.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tz.shxzskj.cn

JS:   process.env.HOME
来源：http://pu.yuexingan06.cn

TS:   process.env.HOME
来源：http://ov.chemitech.net.cn

Java: System.getenv("HOME")
来源：http://xn.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tm.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://nj.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ty.wgjwhj.cn

[M03] 执行外部命令
来源：http://yg.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rc.shxzskj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vc.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kr.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pu.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://et.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yq.yuntaijiaju.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sd.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://hg.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ck.shtwfgs.cn

Py:   os.getcwd()
来源：http://oz.asd995.cn

PHP:  getcwd();
来源：http://zz.asd995.cn

JS:   process.cwd()
来源：http://oi.panjiajie.cn

TS:   process.cwd()
来源：http://ar.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://tp.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://jt.colortex.cn

Ruby: Dir.pwd
来源：http://wo.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dq.muxihuayi.cn

[M05] 设置退出码
来源：http://jn.huixiangedu.cn

Py:   sys.exit(1)
来源：http://bx.wgjwhj.cn

PHP:  exit(1);
来源：http://eh.shxzukj.cn

JS:   process.exit(1)
来源：http://iu.hahajie.cn

TS:   process.exit(1)
来源：http://fd.huanxung.cn

Java: System.exit(1)
来源：http://wr.9csxet.cn

Go:   os.Exit(1)
来源：http://hj.bjjhwx.cn

Ruby: exit 1
来源：http://ka.nicolike.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uy.panjiajie.cn

[M06] 向标准错误输出
来源：http://ai.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://ti.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ze.asd995.cn

JS:   console.error("err")
来源：http://wc.panjiajie.cn

TS:   console.error("err")
来源：http://ba.521024.cn

Java: System.err.println("err")
来源：http://ge.shxzskj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lf.bjjhwx.cn

Ruby: warn "err"
来源：http://vp.wgjwhj.cn

C#:   Console.Error.WriteLine("err")
来源：http://pb.bookmarksfly.cn

[M07] 判断是否为主入口
来源：http://wl.lnxyls.cn

Py:   if __name__ == "__main__":
来源：http://kf.yuntaijiaju.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://of.huanxung.cn

JS:   require.main === module
来源：http://hb.chemitech.net.cn

TS:   require.main === module
来源：http://ae.shxzskj.cn

Java: public static void main(String[] args)
来源：http://fp.hahajie.cn

Go:   func main()
来源：http://ph.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zl.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://st.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://hx.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://ez.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://hp.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://ro.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://kf.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lb.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pl.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mh.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qy.9csxet.cn

================================================================================
来源：http://zz.hahajie.cn

N. 数据结构与算法
来源：http://di.hahajie.cn

================================================================================
来源：http://bf.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://od.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qi.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gu.yuntaijiaju.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gj.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://go.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dn.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://al.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kn.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yr.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://gv.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://aw.9csxet.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ea.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://os.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sa.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jd.hahajie.cn

Go:   slices.Sort(arr)
来源：http://zf.hnjuh.cn

Ruby: arr.sort
来源：http://kr.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fg.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://cy.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yd.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://kz.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lp.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ie.hahajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wz.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lf.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ak.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ji.shxzukj.cn

[N04] 斐波那契数列
来源：http://xw.lnxyls.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sn.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gu.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://au.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tz.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ob.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://di.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sy.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://za.shtwfgs.cn

[N05] 最大公约数
来源：http://mi.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://dr.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xl.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://si.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wn.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ug.panjiajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://no.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://dj.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zq.bjjhwx.cn

[N06] 判断回文字符串
来源：http://mt.szsharing.cn

Py:   s == s[::-1]
来源：http://ci.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://sh.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://hc.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://gv.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://if.gzmigu.cn

Go:   // 双指针从两端比较
来源：http://xm.9csxet.cn

Ruby: s == s.reverse
来源：http://mi.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vp.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://sc.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vl.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hd.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yt.9csxet.cn

TS:   // 手写 Map<string, number>
来源：http://xh.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://nh.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://jr.nszjky.cn

Ruby: // 手写 Hash
来源：http://xy.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fl.asd995.cn

[N08] 生成全排列
来源：http://cj.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://we.jianghongdianzi.cn

PHP:  // 手写递归交换
来源：http://ie.521024.cn

JS:   // 手写回溯递归
来源：http://so.panjiajie.cn

TS:   // 手写回溯递归
来源：http://zg.gzmigu.cn

Java: // 手写回溯递归
来源：http://vg.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://ry.panjiajie.cn

Ruby: arr.permutation.to_a
来源：http://iz.521024.cn

C#:   // 手写回溯递归
来源：http://he.shxzskj.cn

[N09] 栈与队列
来源：http://ay.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ig.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rv.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sg.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zx.hnjuh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xm.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ic.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ud.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tt.hnjuh.cn

[N10] 链表节点定义
来源：http://mz.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bb.panjiajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kx.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pt.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rp.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://db.hnjuh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lp.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nt.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cf.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://jp.521024.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xq.gzmigu.cn

PHP:  // 手写递归函数
来源：http://nk.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lt.newstarts.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lh.colortex.cn

Java: // 手写递归
来源：http://qm.huanxung.cn

Go:   // 手写递归
来源：http://ei.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ip.huanxung.cn

C#:   // 手写递归
来源：http://ip.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pf.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hf.shxzskj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nx.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wj.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.huixiangedu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://el.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sn.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ym.yuexingan06.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ui.wgjwhj.cn

================================================================================
来源：http://qs.huixiangedu.cn

O. 并发与异步
来源：http://ez.asd995.cn

================================================================================
来源：http://me.shtwfgs.cn

[O01] 启动一个线程
来源：http://ie.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ws.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qy.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xy.shxzskj.cn

TS:   // 同 JS
来源：http://cf.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://wr.huanxung.cn

Go:   go f()
来源：http://cm.shxzskj.cn

Ruby: Thread.new { f }
来源：http://br.szxytkj.cn

C#:   Task.Run(() => F());
来源：http://uo.chemitech.net.cn

[O02] 使用线程池
来源：http://dd.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lv.newstarts.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ub.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://hm.9csxet.cn

TS:   // worker_threads 线程池
来源：http://sh.shxzukj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yh.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bm.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gb.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bf.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://zw.lnxyls.cn

Py:   with lock: shared += 1
来源：http://vh.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://jq.huixiangedu.cn


<!-- 参考信息 -->