代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lb.colortex.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ed.huixinmuqiang.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yu.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pm.huanxung.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hd.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sh.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://gx.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://dl.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wd.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://kz.wgjwhj.cn

TS:   v8.serialize(obj)        // Node
来源：http://fn.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ms.hnjuh.cn

Go:   encoding/gob
来源：http://bl.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ar.nicolike.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bn.szsharing.cn

================================================================================
来源：http://eh.bjjhwx.cn

L. 网络请求
来源：http://sm.bjjhwx.cn

================================================================================
来源：http://ak.newstarts.cn

[L01] 发送 GET 请求
来源：http://ce.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rw.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fe.nszjky.cn

JS:   await fetch(url)
来源：http://nr.gzmigu.cn

TS:   await fetch(url)
来源：http://sh.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qo.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://xw.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yu.panjiajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sb.yuexingan06.cn

[L02] 发送 POST JSON
来源：http://rk.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hb.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fk.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sw.hnjuh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sh.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ud.jctech888.com.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gy.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ay.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mn.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://ep.chemitech.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ez.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eb.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.lnxyls.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ro.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tz.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sv.yuexingan06.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hp.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nt.gzmigu.cn

[L04] 设置超时
来源：http://en.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://dl.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xq.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yj.shxzukj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pc.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cd.muxihuayi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cf.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rx.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://so.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://jo.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vd.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wb.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yh.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://id.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vg.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sy.lnxyls.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oi.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lc.jianghongdianzi.cn

[L06] 解析响应为 JSON
来源：http://re.colortex.cn

Py:   resp.json()
来源：http://yv.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://tw.lnxyls.cn

JS:   await resp.json()
来源：http://xy.haigaiapp.cn

TS:   await resp.json()
来源：http://ki.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lm.panjiajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wr.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://tj.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mz.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://nz.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qq.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mf.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://js.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://vu.hahajie.cn

Java: resp.statusCode()
来源：http://ki.nszjky.cn

Go:   resp.StatusCode
来源：http://jp.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://yg.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://rz.szsharing.cn

[L08] 并发请求多个地址
来源：http://xs.bjjhwx.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ce.nszjky.cn

PHP:  curl_multi_init() 系列
来源：http://zu.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zy.panjiajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://un.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nd.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tw.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://se.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kq.nszjky.cn

================================================================================
来源：http://yf.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://at.nicolike.cn

================================================================================
来源：http://wp.muxihuayi.cn

[M01] 读取命令行参数
来源：http://es.huanxung.cn

Py:   sys.argv[1:]
来源：http://ql.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://no.newstarts.cn

JS:   process.argv.slice(2)
来源：http://vy.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://cy.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://fq.panjiajie.cn

Go:   os.Args[1:]
来源：http://ic.panjiajie.cn

Ruby: ARGV
来源：http://to.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://fc.521024.cn

[M02] 读取环境变量
来源：http://es.gzmigu.cn

Py:   os.environ.get("HOME")
来源：http://yw.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ub.9csxet.cn

JS:   process.env.HOME
来源：http://pu.nicolike.cn

TS:   process.env.HOME
来源：http://yo.shxzskj.cn

Java: System.getenv("HOME")
来源：http://ea.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ly.colortex.cn

Ruby: ENV["HOME"]
来源：http://ud.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vz.shxzukj.cn

[M03] 执行外部命令
来源：http://rr.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://za.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jw.szxytkj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lu.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jg.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://od.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ar.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pp.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://um.huanxung.cn

[M04] 获取当前工作目录
来源：http://by.nicolike.cn

Py:   os.getcwd()
来源：http://tn.szsharing.cn

PHP:  getcwd();
来源：http://dz.haigaiapp.cn

JS:   process.cwd()
来源：http://wx.bookmarksfly.cn

TS:   process.cwd()
来源：http://ct.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://uf.9csxet.cn

Go:   os.Getwd()
来源：http://mk.yuexingan06.cn

Ruby: Dir.pwd
来源：http://is.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vy.9csxet.cn

[M05] 设置退出码
来源：http://sw.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://tz.nicolike.cn

PHP:  exit(1);
来源：http://ce.521024.cn

JS:   process.exit(1)
来源：http://tw.muxihuayi.cn

TS:   process.exit(1)
来源：http://lp.wgjwhj.cn

Java: System.exit(1)
来源：http://ft.hahajie.cn

Go:   os.Exit(1)
来源：http://sp.szxytkj.cn

Ruby: exit 1
来源：http://yt.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qv.haigaiapp.cn

[M06] 向标准错误输出
来源：http://zi.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://bz.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kx.hnjuh.cn

JS:   console.error("err")
来源：http://nr.nszjky.cn

TS:   console.error("err")
来源：http://gd.nicolike.cn

Java: System.err.println("err")
来源：http://zu.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yk.jianghongdianzi.cn

Ruby: warn "err"
来源：http://xb.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://fh.yuexingan06.cn

[M07] 判断是否为主入口
来源：http://wm.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://cs.shtwfgs.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://de.lnxyls.cn

JS:   require.main === module
来源：http://sg.shxzskj.cn

TS:   require.main === module
来源：http://xq.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://gp.asd995.cn

Go:   func main()
来源：http://at.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ou.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://cu.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://im.521024.cn

Py:   platform.system();  platform.python_version()
来源：http://yt.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://zm.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://vf.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://pq.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://og.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yl.nszjky.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://al.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uk.newstarts.cn

================================================================================
来源：http://mw.huixiangedu.cn

N. 数据结构与算法
来源：http://el.newstarts.cn

================================================================================
来源：http://oo.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://pb.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vs.huanxung.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mq.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hr.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nz.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pn.lnxyls.cn

Go:   sort.SearchInts(arr, x)
来源：http://ug.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cf.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uk.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://ep.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://xd.szsharing.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zz.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wq.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wn.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ls.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://ti.chemitech.net.cn

Ruby: arr.sort
来源：http://sc.lnxyls.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ad.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://zb.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nt.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://fp.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ni.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mz.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wn.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jm.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bg.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sr.szxytkj.cn

[N04] 斐波那契数列
来源：http://ta.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nv.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gx.jctech888.com.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ru.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xr.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bg.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uf.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yy.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ep.szxytkj.cn

[N05] 最大公约数
来源：http://qe.szxytkj.cn

Py:   math.gcd(a, b)
来源：http://ti.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ek.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dx.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zw.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pl.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cf.shxzskj.cn

Ruby: a.gcd(b)
来源：http://fd.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vr.newstarts.cn

[N06] 判断回文字符串
来源：http://qd.hahajie.cn

Py:   s == s[::-1]
来源：http://pm.nszjky.cn

PHP:  $s === strrev($s);
来源：http://xj.jianghongdianzi.cn

JS:   s === [...s].reverse().join("")
来源：http://xh.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://rk.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xx.9csxet.cn

Go:   // 双指针从两端比较
来源：http://ji.gzmigu.cn

Ruby: s == s.reverse
来源：http://tr.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ew.asd995.cn

[N07] 两数之和（返回下标）
来源：http://xe.nszjky.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hr.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lr.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zq.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://py.huanxung.cn

Java: // 手写 HashMap
来源：http://jq.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://nx.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://lx.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://td.jctech888.com.cn

[N08] 生成全排列
来源：http://iw.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://xb.lnxyls.cn

PHP:  // 手写递归交换
来源：http://cu.panjiajie.cn

JS:   // 手写回溯递归
来源：http://oo.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://cq.panjiajie.cn

Java: // 手写回溯递归
来源：http://fx.colortex.cn

Go:   // 手写回溯递归
来源：http://lr.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://dy.bjjhwx.cn

C#:   // 手写回溯递归
来源：http://yz.colortex.cn

[N09] 栈与队列
来源：http://du.lnxyls.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://og.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://be.chemitech.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pi.huixinmuqiang.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wa.jianghongdianzi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ut.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qy.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rd.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ht.colortex.cn

[N10] 链表节点定义
来源：http://cm.yuexingan06.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xs.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ar.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://be.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zd.huixiangedu.cn

Java: class Node { int v; Node next; }
来源：http://vf.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wb.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sr.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ao.szsharing.cn

[N11] 二叉树中序遍历
来源：http://xi.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rn.jianghongdianzi.cn

PHP:  // 手写递归函数
来源：http://qa.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zt.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qt.shxzskj.cn

Java: // 手写递归
来源：http://gk.panjiajie.cn

Go:   // 手写递归
来源：http://fo.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vx.haigaiapp.cn

C#:   // 手写递归
来源：http://tw.shxzukj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dj.wgjwhj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://be.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lm.newstarts.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kc.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://es.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hv.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ja.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pr.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hv.hahajie.cn

================================================================================
来源：http://an.muxihuayi.cn

O. 并发与异步
来源：http://vb.9csxet.cn

================================================================================
来源：http://qv.bookmarksfly.cn

[O01] 启动一个线程
来源：http://wv.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ym.hahajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dd.shxzukj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bb.9csxet.cn

TS:   // 同 JS
来源：http://ra.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://sn.bookmarksfly.cn

Go:   go f()
来源：http://kc.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://zb.shxzskj.cn

C#:   Task.Run(() => F());
来源：http://uj.yuntaijiaju.cn

[O02] 使用线程池
来源：http://uy.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rt.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mp.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://fv.bjjhwx.cn

TS:   // worker_threads 线程池
来源：http://sy.521024.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aa.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tl.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cs.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hf.521024.cn

[O03] 加锁保护共享数据
来源：http://zi.nicolike.cn

Py:   with lock: shared += 1
来源：http://tw.hnjuh.cn

PHP:  // 用 flock() 做文件锁
来源：http://jj.colortex.cn


<!-- 参考信息 -->