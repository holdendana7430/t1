代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ee.szsharing.cn

[K07] 进制转换
来源：http://xd.bjjhwx.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ii.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pj.jianghongdianzi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pa.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zx.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pc.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ze.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bs.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wu.huanxung.cn

[K08] 二进制序列化（非 JSON）
来源：http://cv.jianghongdianzi.cn

Py:   pickle.dumps(obj)
来源：http://cm.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uv.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://il.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://fs.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qx.chemitech.net.cn

Go:   encoding/gob
来源：http://rd.chemitech.net.cn

Ruby: Marshal.dump(obj)
来源：http://gb.colortex.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ka.wgjwhj.cn

================================================================================
来源：http://mf.szxytkj.cn

L. 网络请求
来源：http://mt.chemitech.net.cn

================================================================================
来源：http://nd.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://au.bjjhwx.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ef.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ta.gzmigu.cn

JS:   await fetch(url)
来源：http://qn.huixinmuqiang.cn

TS:   await fetch(url)
来源：http://we.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oy.bookmarksfly.cn

Go:   resp, err := http.Get(url)
来源：http://wz.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kj.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zn.nicolike.cn

[L02] 发送 POST JSON
来源：http://wh.gzmigu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ox.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tz.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mw.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ya.huanxung.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oi.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jr.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yc.yuexingan06.cn

[L03] 设置自定义请求头
来源：http://vc.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gk.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ic.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gd.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ir.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://md.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jk.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fu.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ix.panjiajie.cn

[L04] 设置超时
来源：http://az.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://dk.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gi.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sb.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ma.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ku.huanxung.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cl.shxzukj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nf.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aq.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://kl.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://re.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wg.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oq.hahajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zq.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hx.yuntaijiaju.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://us.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aj.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cq.chemitech.net.cn

[L06] 解析响应为 JSON
来源：http://di.521024.cn

Py:   resp.json()
来源：http://zj.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://cx.shxzukj.cn

JS:   await resp.json()
来源：http://hi.hahajie.cn

TS:   await resp.json()
来源：http://vo.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yi.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xl.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://rv.gzmigu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zy.shtwfgs.cn

[L07] 处理 HTTP 状态码
来源：http://jv.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ms.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yc.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://rx.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://kk.gzmigu.cn

Java: resp.statusCode()
来源：http://vi.newstarts.cn

Go:   resp.StatusCode
来源：http://ns.bookmarksfly.cn

Ruby: resp.code.to_i
来源：http://ro.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://ff.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://kn.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hb.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://ae.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://om.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xh.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gh.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fz.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pd.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tr.shtwfgs.cn

================================================================================
来源：http://zh.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://cg.wgjwhj.cn

================================================================================
来源：http://cc.lnxyls.cn

[M01] 读取命令行参数
来源：http://iy.hahajie.cn

Py:   sys.argv[1:]
来源：http://fh.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://ga.shxzukj.cn

JS:   process.argv.slice(2)
来源：http://ul.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://uk.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://go.panjiajie.cn

Go:   os.Args[1:]
来源：http://rl.huixiangedu.cn

Ruby: ARGV
来源：http://hf.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://rf.lnxyls.cn

[M02] 读取环境变量
来源：http://zl.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://uw.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ti.shtwfgs.cn

JS:   process.env.HOME
来源：http://ok.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://nv.huanxung.cn

Java: System.getenv("HOME")
来源：http://aw.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fg.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://xo.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wm.gzmigu.cn

[M03] 执行外部命令
来源：http://qt.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yi.lnxyls.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hh.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://of.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ug.hnjuh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sh.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gc.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zd.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://tb.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://lc.panjiajie.cn

Py:   os.getcwd()
来源：http://ej.wgjwhj.cn

PHP:  getcwd();
来源：http://pm.9csxet.cn

JS:   process.cwd()
来源：http://sh.colortex.cn

TS:   process.cwd()
来源：http://zd.huixiangedu.cn

Java: Path.of("").toAbsolutePath()
来源：http://ao.asd995.cn

Go:   os.Getwd()
来源：http://ld.9csxet.cn

Ruby: Dir.pwd
来源：http://ae.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xj.shtwfgs.cn

[M05] 设置退出码
来源：http://td.newstarts.cn

Py:   sys.exit(1)
来源：http://fr.bjjhwx.cn

PHP:  exit(1);
来源：http://sw.gzmigu.cn

JS:   process.exit(1)
来源：http://bb.gzmigu.cn

TS:   process.exit(1)
来源：http://fw.jianghongdianzi.cn

Java: System.exit(1)
来源：http://fk.huanxung.cn

Go:   os.Exit(1)
来源：http://jk.szsharing.cn

Ruby: exit 1
来源：http://fc.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zd.panjiajie.cn

[M06] 向标准错误输出
来源：http://ro.bookmarksfly.cn

Py:   print("err", file=sys.stderr)
来源：http://gs.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cd.huanxung.cn

JS:   console.error("err")
来源：http://yx.lnxyls.cn

TS:   console.error("err")
来源：http://ng.panjiajie.cn

Java: System.err.println("err")
来源：http://lb.wgjwhj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wm.yuntaijiaju.cn

Ruby: warn "err"
来源：http://gm.nszjky.cn

C#:   Console.Error.WriteLine("err")
来源：http://dd.haigaiapp.cn

[M07] 判断是否为主入口
来源：http://fr.huanxung.cn

Py:   if __name__ == "__main__":
来源：http://kr.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hc.yuexingan06.cn

JS:   require.main === module
来源：http://sg.asd995.cn

TS:   require.main === module
来源：http://hm.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ky.gzmigu.cn

Go:   func main()
来源：http://gp.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uf.hahajie.cn

C#:   static void Main(string[] args)
来源：http://nt.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://kc.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://cq.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://md.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://qa.gzmigu.cn

TS:   process.platform;  process.version
来源：http://cs.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fm.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://de.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ng.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xn.nszjky.cn

================================================================================
来源：http://os.huixiangedu.cn

N. 数据结构与算法
来源：http://th.chemitech.net.cn

================================================================================
来源：http://ap.shtwfgs.cn

[N01] 二分查找（有序数组）
来源：http://ah.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zb.nicolike.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pi.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hv.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jj.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qg.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://fk.haigaiapp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nl.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fy.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://wt.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qr.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fr.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oi.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ul.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://id.newstarts.cn

Go:   slices.Sort(arr)
来源：http://re.bookmarksfly.cn

Ruby: arr.sort
来源：http://do.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://op.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://vl.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ep.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://wo.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://if.asd995.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hv.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dn.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ez.hahajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ea.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eo.haigaiapp.cn

[N04] 斐波那契数列
来源：http://hr.9csxet.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xn.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ms.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jd.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://td.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ow.gzmigu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bh.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aq.jctech888.com.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zb.chemitech.net.cn

[N05] 最大公约数
来源：http://sv.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://hk.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dj.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://le.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sj.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ut.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vm.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://sz.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rc.haigaiapp.cn

[N06] 判断回文字符串
来源：http://jk.huanxung.cn

Py:   s == s[::-1]
来源：http://gm.wgjwhj.cn

PHP:  $s === strrev($s);
来源：http://le.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://wv.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://mg.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bw.colortex.cn

Go:   // 双指针从两端比较
来源：http://vi.colortex.cn

Ruby: s == s.reverse
来源：http://ns.hahajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jg.colortex.cn

[N07] 两数之和（返回下标）
来源：http://rf.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zn.yuntaijiaju.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oe.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nw.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://mt.521024.cn

Java: // 手写 HashMap
来源：http://pl.nicolike.cn

Go:   // 手写 map[int]int
来源：http://np.szsharing.cn

Ruby: // 手写 Hash
来源：http://ov.bjjhwx.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vw.nszjky.cn

[N08] 生成全排列
来源：http://jp.huanxung.cn

Py:   itertools.permutations(arr)
来源：http://ds.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://zd.panjiajie.cn

JS:   // 手写回溯递归
来源：http://mj.gzmigu.cn

TS:   // 手写回溯递归
来源：http://va.gzmigu.cn

Java: // 手写回溯递归
来源：http://so.szsharing.cn

Go:   // 手写回溯递归
来源：http://so.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://da.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://ko.shxzskj.cn

[N09] 栈与队列
来源：http://rl.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nl.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lg.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ku.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kv.newstarts.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oj.nicolike.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://us.haigaiapp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eh.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xr.chemitech.net.cn

[N10] 链表节点定义
来源：http://ht.muxihuayi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ee.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hm.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gh.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jl.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://wf.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jk.yuexingan06.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vc.huixinmuqiang.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tm.nicolike.cn

[N11] 二叉树中序遍历
来源：http://yu.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mb.nszjky.cn

PHP:  // 手写递归函数
来源：http://df.szsharing.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yn.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dk.jianghongdianzi.cn

Java: // 手写递归
来源：http://xn.chemitech.net.cn

Go:   // 手写递归
来源：http://wj.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ot.huixinmuqiang.cn

C#:   // 手写递归
来源：http://vx.colortex.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cn.muxihuayi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ms.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zc.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aa.jctech888.com.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tj.521024.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wu.asd995.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wc.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hw.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://re.colortex.cn

================================================================================
来源：http://fr.nicolike.cn

O. 并发与异步
来源：http://yr.yuntaijiaju.cn

================================================================================
来源：http://fg.yuexingan06.cn

[O01] 启动一个线程
来源：http://pz.shtwfgs.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://of.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wv.bjjhwx.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rw.yuntaijiaju.cn

TS:   // 同 JS
来源：http://sp.521024.cn

Java: new Thread(() -> f()).start()
来源：http://ad.9csxet.cn

Go:   go f()
来源：http://rq.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://se.huixiangedu.cn

C#:   Task.Run(() => F());
来源：http://ub.panjiajie.cn

[O02] 使用线程池
来源：http://he.bookmarksfly.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://le.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cf.lnxyls.cn

JS:   // worker_threads 线程池
来源：http://pg.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://vf.newstarts.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xq.colortex.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yu.colortex.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ek.szsharing.cn


<!-- 参考信息 -->