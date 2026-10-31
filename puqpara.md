代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hr.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://na.shxzskj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gd.huanxung.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zu.yuexingan06.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vo.shtwfgs.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wo.newstarts.cn

[K08] 二进制序列化（非 JSON）
来源：http://zy.shtwfgs.cn

Py:   pickle.dumps(obj)
来源：http://ep.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wp.panjiajie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bg.shxzukj.cn

TS:   v8.serialize(obj)        // Node
来源：http://it.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eq.shtwfgs.cn

Go:   encoding/gob
来源：http://ud.jianghongdianzi.cn

Ruby: Marshal.dump(obj)
来源：http://hm.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yc.521024.cn

================================================================================
来源：http://mw.9csxet.cn

L. 网络请求
来源：http://ds.yuntaijiaju.cn

================================================================================
来源：http://ps.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://cg.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zm.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ht.9csxet.cn

JS:   await fetch(url)
来源：http://di.nicolike.cn

TS:   await fetch(url)
来源：http://dv.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lc.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://el.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ra.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sd.haigaiapp.cn

[L02] 发送 POST JSON
来源：http://hr.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://be.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xo.chemitech.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ey.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gv.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lw.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zg.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nr.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sh.bookmarksfly.cn

[L03] 设置自定义请求头
来源：http://xg.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mr.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pg.muxihuayi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tz.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bg.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gl.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pj.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uc.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://do.asd995.cn

[L04] 设置超时
来源：http://xs.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://rc.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://di.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ia.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xw.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zd.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mw.bjjhwx.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://az.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://so.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://vw.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lt.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sy.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hq.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vc.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nm.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fe.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uz.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://in.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://ce.muxihuayi.cn

Py:   resp.json()
来源：http://gf.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://ub.szsharing.cn

JS:   await resp.json()
来源：http://el.wgjwhj.cn

TS:   await resp.json()
来源：http://xz.chemitech.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://um.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uz.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://vf.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://je.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://sx.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ao.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://si.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://iq.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://uu.yuexingan06.cn

Java: resp.statusCode()
来源：http://vm.huixiangedu.cn

Go:   resp.StatusCode
来源：http://va.newstarts.cn

Ruby: resp.code.to_i
来源：http://pk.colortex.cn

C#:   (int)resp.StatusCode
来源：http://ig.yuntaijiaju.cn

[L08] 并发请求多个地址
来源：http://tw.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xp.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://ad.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ff.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wq.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vy.newstarts.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tf.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xo.huixinmuqiang.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xd.bjjhwx.cn

================================================================================
来源：http://vg.huixiangedu.cn

M. 命令行 / 进程 / 环境
来源：http://ew.panjiajie.cn

================================================================================
来源：http://yi.9csxet.cn

[M01] 读取命令行参数
来源：http://di.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://ln.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://vg.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://vm.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://dn.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://qm.szxytkj.cn

Go:   os.Args[1:]
来源：http://if.gzmigu.cn

Ruby: ARGV
来源：http://pp.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://pm.huixiangedu.cn

[M02] 读取环境变量
来源：http://pc.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://dw.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yp.szxytkj.cn

JS:   process.env.HOME
来源：http://kb.chemitech.net.cn

TS:   process.env.HOME
来源：http://yn.bookmarksfly.cn

Java: System.getenv("HOME")
来源：http://nu.lnxyls.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jb.nszjky.cn

Ruby: ENV["HOME"]
来源：http://xg.huixiangedu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zi.521024.cn

[M03] 执行外部命令
来源：http://nh.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yo.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cv.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kr.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ac.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qs.gzmigu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ih.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ac.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://pe.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://no.bjjhwx.cn

Py:   os.getcwd()
来源：http://fv.jctech888.com.cn

PHP:  getcwd();
来源：http://oo.bookmarksfly.cn

JS:   process.cwd()
来源：http://qj.hnjuh.cn

TS:   process.cwd()
来源：http://yr.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://os.shxzukj.cn

Go:   os.Getwd()
来源：http://ve.huanxung.cn

Ruby: Dir.pwd
来源：http://yn.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mm.yuntaijiaju.cn

[M05] 设置退出码
来源：http://iu.9csxet.cn

Py:   sys.exit(1)
来源：http://ga.chemitech.net.cn

PHP:  exit(1);
来源：http://yr.hahajie.cn

JS:   process.exit(1)
来源：http://vo.chemitech.net.cn

TS:   process.exit(1)
来源：http://ma.nicolike.cn

Java: System.exit(1)
来源：http://ql.asd995.cn

Go:   os.Exit(1)
来源：http://ww.huanxung.cn

Ruby: exit 1
来源：http://ud.haigaiapp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zh.colortex.cn

[M06] 向标准错误输出
来源：http://uf.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://qh.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vu.szsharing.cn

JS:   console.error("err")
来源：http://yo.wgjwhj.cn

TS:   console.error("err")
来源：http://sf.newstarts.cn

Java: System.err.println("err")
来源：http://ur.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://if.shxzskj.cn

Ruby: warn "err"
来源：http://yu.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://vz.newstarts.cn

[M07] 判断是否为主入口
来源：http://sd.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://vj.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hr.asd995.cn

JS:   require.main === module
来源：http://cg.panjiajie.cn

TS:   require.main === module
来源：http://rl.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://jz.shxzskj.cn

Go:   func main()
来源：http://gw.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qo.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://uq.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://mp.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://xc.nszjky.cn

PHP:  PHP_OS;  phpversion();
来源：http://uj.shxzskj.cn

JS:   process.platform;  process.version
来源：http://vm.shxzskj.cn

TS:   process.platform;  process.version
来源：http://gh.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ej.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fu.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zi.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ou.nicolike.cn

================================================================================
来源：http://eo.szsharing.cn

N. 数据结构与算法
来源：http://sk.jctech888.com.cn

================================================================================
来源：http://hd.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://bh.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://av.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cz.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yl.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qz.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yr.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://ok.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tu.jctech888.com.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wp.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ro.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://yd.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hg.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oi.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oh.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pl.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://jc.szsharing.cn

Ruby: arr.sort
来源：http://sw.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ml.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://wl.bjjhwx.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xa.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://rq.colortex.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ex.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ga.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fd.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zz.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ce.521024.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wm.yuexingan06.cn

[N04] 斐波那契数列
来源：http://im.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lm.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ge.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cq.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eq.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ha.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cj.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://av.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sb.jianghongdianzi.cn

[N05] 最大公约数
来源：http://zj.9csxet.cn

Py:   math.gcd(a, b)
来源：http://ej.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eh.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yc.hnjuh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aq.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ia.jianghongdianzi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rc.colortex.cn

Ruby: a.gcd(b)
来源：http://yo.jianghongdianzi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tk.colortex.cn

[N06] 判断回文字符串
来源：http://xr.szxytkj.cn

Py:   s == s[::-1]
来源：http://js.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://zu.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://pk.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://wf.shxzskj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lt.asd995.cn

Go:   // 双指针从两端比较
来源：http://pv.asd995.cn

Ruby: s == s.reverse
来源：http://gw.521024.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qi.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://mk.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yz.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xi.bjjhwx.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ri.huixinmuqiang.cn

TS:   // 手写 Map<string, number>
来源：http://al.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://dm.wgjwhj.cn

Go:   // 手写 map[int]int
来源：http://yk.gzmigu.cn

Ruby: // 手写 Hash
来源：http://bk.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qr.shtwfgs.cn

[N08] 生成全排列
来源：http://ax.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://vi.colortex.cn

PHP:  // 手写递归交换
来源：http://ws.lnxyls.cn

JS:   // 手写回溯递归
来源：http://ah.nszjky.cn

TS:   // 手写回溯递归
来源：http://ib.bjjhwx.cn

Java: // 手写回溯递归
来源：http://px.nicolike.cn

Go:   // 手写回溯递归
来源：http://hh.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://as.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://qn.huixiangedu.cn

[N09] 栈与队列
来源：http://dg.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ae.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vm.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ek.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://de.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ne.9csxet.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wv.yuntaijiaju.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ft.szsharing.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zi.wgjwhj.cn

[N10] 链表节点定义
来源：http://ir.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zb.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ct.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tm.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fj.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://wo.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ie.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hs.jianghongdianzi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lg.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://cq.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xt.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://yg.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mi.bjjhwx.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zk.chemitech.net.cn

Java: // 手写递归
来源：http://kh.asd995.cn

Go:   // 手写递归
来源：http://eh.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qv.haigaiapp.cn

C#:   // 手写递归
来源：http://sv.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wu.panjiajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ff.huixiangedu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iz.szxytkj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mu.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hp.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://me.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uv.asd995.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ce.szsharing.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tz.huanxung.cn

================================================================================
来源：http://qs.hahajie.cn

O. 并发与异步
来源：http://xq.lnxyls.cn

================================================================================
来源：http://qq.nszjky.cn

[O01] 启动一个线程
来源：http://nh.chemitech.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ne.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://af.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lb.szsharing.cn

TS:   // 同 JS
来源：http://en.521024.cn

Java: new Thread(() -> f()).start()
来源：http://lb.nszjky.cn

Go:   go f()
来源：http://rj.asd995.cn

Ruby: Thread.new { f }
来源：http://fn.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ji.haigaiapp.cn

[O02] 使用线程池
来源：http://hc.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jy.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lm.nicolike.cn

JS:   // worker_threads 线程池
来源：http://rx.shxzukj.cn

TS:   // worker_threads 线程池
来源：http://tt.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nn.nszjky.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yu.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nf.hahajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vp.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://yc.hahajie.cn

Py:   with lock: shared += 1
来源：http://sk.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://ph.hahajie.cn


<!-- 参考信息 -->