代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://of.9csxet.cn

[K07] 进制转换
来源：http://ns.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hy.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hs.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mr.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ne.9csxet.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ai.jianghongdianzi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zg.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sc.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hc.panjiajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://lj.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://jg.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wr.yuntaijiaju.cn

JS:   v8.serialize(obj)        // Node
来源：http://ev.colortex.cn

TS:   v8.serialize(obj)        // Node
来源：http://aj.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wa.bookmarksfly.cn

Go:   encoding/gob
来源：http://kw.bjjhwx.cn

Ruby: Marshal.dump(obj)
来源：http://ge.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ij.gzmigu.cn

================================================================================
来源：http://ig.haigaiapp.cn

L. 网络请求
来源：http://oj.muxihuayi.cn

================================================================================
来源：http://zu.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://nx.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zm.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ci.gzmigu.cn

JS:   await fetch(url)
来源：http://ek.gzmigu.cn

TS:   await fetch(url)
来源：http://fk.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ly.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://bw.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rc.colortex.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pu.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://ni.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eq.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qb.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rb.bjjhwx.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sw.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pn.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ce.huanxung.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pb.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ba.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://tn.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fq.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ma.jctech888.com.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sg.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wb.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://op.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hn.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yf.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tl.yuexingan06.cn

[L04] 设置超时
来源：http://gs.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://ma.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://he.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mf.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wb.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jz.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cj.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vs.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vc.colortex.cn

[L05] 上传文件（multipart）
来源：http://vf.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nu.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eg.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ek.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jf.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vy.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ca.chemitech.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uc.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ys.colortex.cn

[L06] 解析响应为 JSON
来源：http://nh.szxytkj.cn

Py:   resp.json()
来源：http://ku.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://vh.9csxet.cn

JS:   await resp.json()
来源：http://ni.gzmigu.cn

TS:   await resp.json()
来源：http://lv.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vl.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bw.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://ka.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xc.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://wy.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lo.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dg.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://ti.jianghongdianzi.cn

TS:   resp.ok;  resp.status
来源：http://wu.panjiajie.cn

Java: resp.statusCode()
来源：http://me.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://jz.nszjky.cn

Ruby: resp.code.to_i
来源：http://sz.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://hu.shxzukj.cn

[L08] 并发请求多个地址
来源：http://jz.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eb.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://xi.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://km.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cq.huanxung.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xn.shxzukj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jy.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zc.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cs.shtwfgs.cn

================================================================================
来源：http://mh.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://cj.jctech888.com.cn

================================================================================
来源：http://we.chemitech.net.cn

[M01] 读取命令行参数
来源：http://zx.hahajie.cn

Py:   sys.argv[1:]
来源：http://au.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://yr.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://ma.newstarts.cn

TS:   process.argv.slice(2)
来源：http://qj.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://zw.521024.cn

Go:   os.Args[1:]
来源：http://rq.huanxung.cn

Ruby: ARGV
来源：http://oh.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://qo.wgjwhj.cn

[M02] 读取环境变量
来源：http://ww.521024.cn

Py:   os.environ.get("HOME")
来源：http://vn.huixiangedu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ep.wgjwhj.cn

JS:   process.env.HOME
来源：http://vt.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://ll.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://qq.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ld.521024.cn

Ruby: ENV["HOME"]
来源：http://yf.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rj.asd995.cn

[M03] 执行外部命令
来源：http://mh.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ps.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iw.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fv.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bf.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gr.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yv.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ec.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://fl.bookmarksfly.cn

[M04] 获取当前工作目录
来源：http://kl.huixinmuqiang.cn

Py:   os.getcwd()
来源：http://oe.chemitech.net.cn

PHP:  getcwd();
来源：http://fa.muxihuayi.cn

JS:   process.cwd()
来源：http://dd.9csxet.cn

TS:   process.cwd()
来源：http://ez.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://er.muxihuayi.cn

Go:   os.Getwd()
来源：http://sl.chemitech.net.cn

Ruby: Dir.pwd
来源：http://rf.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pf.jianghongdianzi.cn

[M05] 设置退出码
来源：http://er.haigaiapp.cn

Py:   sys.exit(1)
来源：http://ae.bjjhwx.cn

PHP:  exit(1);
来源：http://fo.asd995.cn

JS:   process.exit(1)
来源：http://zw.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://ov.szsharing.cn

Java: System.exit(1)
来源：http://kj.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://uh.521024.cn

Ruby: exit 1
来源：http://os.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nb.szsharing.cn

[M06] 向标准错误输出
来源：http://zy.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://hc.colortex.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ku.521024.cn

JS:   console.error("err")
来源：http://sn.yuntaijiaju.cn

TS:   console.error("err")
来源：http://fp.szxytkj.cn

Java: System.err.println("err")
来源：http://ha.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oo.chemitech.net.cn

Ruby: warn "err"
来源：http://ir.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://nm.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://uy.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://sb.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pv.lnxyls.cn

JS:   require.main === module
来源：http://cz.hahajie.cn

TS:   require.main === module
来源：http://cp.lnxyls.cn

Java: public static void main(String[] args)
来源：http://yq.bjjhwx.cn

Go:   func main()
来源：http://ow.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pc.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://hi.chemitech.net.cn

[M08] 获取系统与运行时信息
来源：http://vd.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://it.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://so.panjiajie.cn

JS:   process.platform;  process.version
来源：http://br.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://xg.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ky.chemitech.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ya.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mg.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mp.gzmigu.cn

================================================================================
来源：http://mu.muxihuayi.cn

N. 数据结构与算法
来源：http://hp.colortex.cn

================================================================================
来源：http://lh.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://bs.asd995.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yx.huixiangedu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ka.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eo.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wu.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://km.yuexingan06.cn

Go:   sort.SearchInts(arr, x)
来源：http://bs.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ih.bookmarksfly.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gx.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://vb.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://pp.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pe.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tn.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yk.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bb.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://pt.huanxung.cn

Ruby: arr.sort
来源：http://mo.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oq.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://nq.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ae.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://un.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fz.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vn.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wb.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jn.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xt.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ca.szxytkj.cn

[N04] 斐波那契数列
来源：http://ve.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dl.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://me.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bz.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yp.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wz.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zn.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dd.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ik.newstarts.cn

[N05] 最大公约数
来源：http://ep.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://iw.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qn.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ec.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kl.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kb.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lt.gzmigu.cn

Ruby: a.gcd(b)
来源：http://ht.hahajie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gf.haigaiapp.cn

[N06] 判断回文字符串
来源：http://op.panjiajie.cn

Py:   s == s[::-1]
来源：http://gj.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://nb.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ps.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://wf.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://an.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://yr.lnxyls.cn

Ruby: s == s.reverse
来源：http://pt.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vf.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://nq.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tl.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vv.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sc.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://bq.lnxyls.cn

Java: // 手写 HashMap
来源：http://zc.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://bf.newstarts.cn

Ruby: // 手写 Hash
来源：http://yr.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ar.hahajie.cn

[N08] 生成全排列
来源：http://ow.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://mt.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://kc.9csxet.cn

JS:   // 手写回溯递归
来源：http://tq.521024.cn

TS:   // 手写回溯递归
来源：http://yp.lnxyls.cn

Java: // 手写回溯递归
来源：http://cv.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://km.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://gi.colortex.cn

C#:   // 手写回溯递归
来源：http://zf.yuntaijiaju.cn

[N09] 栈与队列
来源：http://cb.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ro.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cm.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ku.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yd.colortex.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nr.bjjhwx.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ff.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ea.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://od.nszjky.cn

[N10] 链表节点定义
来源：http://sn.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vm.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ve.huixiangedu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ky.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tp.hahajie.cn

Java: class Node { int v; Node next; }
来源：http://gl.chemitech.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cz.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ox.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uw.521024.cn

[N11] 二叉树中序遍历
来源：http://gx.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://di.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://bg.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qm.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cv.szsharing.cn

Java: // 手写递归
来源：http://qf.huanxung.cn

Go:   // 手写递归
来源：http://yg.huixiangedu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yv.bjjhwx.cn

C#:   // 手写递归
来源：http://oz.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zk.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://as.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wx.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gn.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dp.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lq.yuntaijiaju.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cb.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hq.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jk.gzmigu.cn

================================================================================
来源：http://oz.bjjhwx.cn

O. 并发与异步
来源：http://mg.haigaiapp.cn

================================================================================
来源：http://mj.jctech888.com.cn

[O01] 启动一个线程
来源：http://pp.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kc.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zi.muxihuayi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zf.huixiangedu.cn

TS:   // 同 JS
来源：http://vt.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://ub.nicolike.cn

Go:   go f()
来源：http://pd.9csxet.cn

Ruby: Thread.new { f }
来源：http://rf.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://et.yuntaijiaju.cn

[O02] 使用线程池
来源：http://rt.huixinmuqiang.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rj.nicolike.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ls.szsharing.cn

JS:   // worker_threads 线程池
来源：http://bo.huixinmuqiang.cn

TS:   // worker_threads 线程池
来源：http://tu.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yw.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dq.jianghongdianzi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cq.gzmigu.cn


<!-- 参考信息 -->