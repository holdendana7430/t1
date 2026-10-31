代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nu.nszjky.cn

[K07] 进制转换
来源：http://oh.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xu.hahajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yq.yuntaijiaju.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://be.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cm.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dl.nszjky.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rx.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uq.hnjuh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iz.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://lr.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://gb.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ia.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://hp.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://nf.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wj.nszjky.cn

Go:   encoding/gob
来源：http://pl.huixinmuqiang.cn

Ruby: Marshal.dump(obj)
来源：http://hf.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jq.jianghongdianzi.cn

================================================================================
来源：http://ja.lnxyls.cn

L. 网络请求
来源：http://yd.huixiangedu.cn

================================================================================
来源：http://ux.hnjuh.cn

[L01] 发送 GET 请求
来源：http://ug.huixinmuqiang.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ce.bookmarksfly.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lt.nicolike.cn

JS:   await fetch(url)
来源：http://ux.newstarts.cn

TS:   await fetch(url)
来源：http://mx.shxzukj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ac.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://df.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://im.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://si.nicolike.cn

[L02] 发送 POST JSON
来源：http://fs.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ag.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jd.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rs.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fy.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fg.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fr.hnjuh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yz.shxzukj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ze.huixiangedu.cn

[L03] 设置自定义请求头
来源：http://zr.szxytkj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oa.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gu.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ll.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oy.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lf.nicolike.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pw.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jf.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xm.bookmarksfly.cn

[L04] 设置超时
来源：http://eb.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://pe.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://um.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wx.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rg.szsharing.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aq.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qw.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vo.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://ua.shtwfgs.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lr.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://di.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ue.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rd.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gs.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zp.jianghongdianzi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://su.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qp.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://ka.chemitech.net.cn

Py:   resp.json()
来源：http://jx.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://vn.yuntaijiaju.cn

JS:   await resp.json()
来源：http://cn.szsharing.cn

TS:   await resp.json()
来源：http://nv.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ys.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ar.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://ml.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cq.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://hn.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hh.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fd.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://dn.asd995.cn

TS:   resp.ok;  resp.status
来源：http://mi.lnxyls.cn

Java: resp.statusCode()
来源：http://pl.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://fo.bjjhwx.cn

Ruby: resp.code.to_i
来源：http://bc.wgjwhj.cn

C#:   (int)resp.StatusCode
来源：http://pc.colortex.cn

[L08] 并发请求多个地址
来源：http://ve.huixiangedu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jh.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://td.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qv.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pu.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rj.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jr.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ho.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qe.szsharing.cn

================================================================================
来源：http://qr.521024.cn

M. 命令行 / 进程 / 环境
来源：http://iz.colortex.cn

================================================================================
来源：http://eq.nicolike.cn

[M01] 读取命令行参数
来源：http://yl.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://an.asd995.cn

PHP:  $argv;  $argc;
来源：http://bf.huixinmuqiang.cn

JS:   process.argv.slice(2)
来源：http://na.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://hs.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://kp.lnxyls.cn

Go:   os.Args[1:]
来源：http://ob.yuexingan06.cn

Ruby: ARGV
来源：http://xi.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://il.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://eg.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://ml.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://js.huanxung.cn

JS:   process.env.HOME
来源：http://mj.huanxung.cn

TS:   process.env.HOME
来源：http://ny.newstarts.cn

Java: System.getenv("HOME")
来源：http://ch.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yf.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ns.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pu.panjiajie.cn

[M03] 执行外部命令
来源：http://tv.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nl.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lv.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pn.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sf.colortex.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pg.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uy.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ks.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://rj.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://dw.szxytkj.cn

Py:   os.getcwd()
来源：http://ik.9csxet.cn

PHP:  getcwd();
来源：http://mo.shxzskj.cn

JS:   process.cwd()
来源：http://mk.szxytkj.cn

TS:   process.cwd()
来源：http://co.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://ns.521024.cn

Go:   os.Getwd()
来源：http://ov.huanxung.cn

Ruby: Dir.pwd
来源：http://bz.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bb.bjjhwx.cn

[M05] 设置退出码
来源：http://jh.yuexingan06.cn

Py:   sys.exit(1)
来源：http://lj.9csxet.cn

PHP:  exit(1);
来源：http://tf.hnjuh.cn

JS:   process.exit(1)
来源：http://ew.shxzskj.cn

TS:   process.exit(1)
来源：http://un.panjiajie.cn

Java: System.exit(1)
来源：http://wx.jianghongdianzi.cn

Go:   os.Exit(1)
来源：http://cw.huixiangedu.cn

Ruby: exit 1
来源：http://yf.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yx.haigaiapp.cn

[M06] 向标准错误输出
来源：http://na.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://li.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gx.bjjhwx.cn

JS:   console.error("err")
来源：http://kk.newstarts.cn

TS:   console.error("err")
来源：http://eq.panjiajie.cn

Java: System.err.println("err")
来源：http://tq.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kv.521024.cn

Ruby: warn "err"
来源：http://xz.yuntaijiaju.cn

C#:   Console.Error.WriteLine("err")
来源：http://fn.newstarts.cn

[M07] 判断是否为主入口
来源：http://kd.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://nb.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lm.9csxet.cn

JS:   require.main === module
来源：http://go.hahajie.cn

TS:   require.main === module
来源：http://hm.panjiajie.cn

Java: public static void main(String[] args)
来源：http://sx.bjjhwx.cn

Go:   func main()
来源：http://yt.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cm.huanxung.cn

C#:   static void Main(string[] args)
来源：http://pm.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://mq.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://dn.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://uj.shxzukj.cn

JS:   process.platform;  process.version
来源：http://jq.shxzukj.cn

TS:   process.platform;  process.version
来源：http://jk.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fs.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xc.shxzskj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://am.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sa.shxzskj.cn

================================================================================
来源：http://ha.muxihuayi.cn

N. 数据结构与算法
来源：http://mx.haigaiapp.cn

================================================================================
来源：http://xc.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://it.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ng.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pf.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lz.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lb.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wp.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://xr.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hq.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nk.huixiangedu.cn

[N02] 排序（工程实践用内置实现）
来源：http://wr.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://zb.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sk.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cf.nicolike.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lk.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ab.jctech888.com.cn

Go:   slices.Sort(arr)
来源：http://nw.521024.cn

Ruby: arr.sort
来源：http://pn.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ja.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://wl.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vp.haigaiapp.cn

PHP:  // 递归实现，或用 usort
来源：http://pe.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zx.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mf.nszjky.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ct.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mt.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://og.yuexingan06.cn

[N04] 斐波那契数列
来源：http://sm.newstarts.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yr.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hm.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qs.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nq.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rv.hahajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nk.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gm.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zt.huixiangedu.cn

[N05] 最大公约数
来源：http://yz.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://my.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pr.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dr.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ur.colortex.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hp.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sx.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://bj.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ku.haigaiapp.cn

[N06] 判断回文字符串
来源：http://fn.wgjwhj.cn

Py:   s == s[::-1]
来源：http://au.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://vq.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://gx.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://zd.haigaiapp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kg.shxzskj.cn

Go:   // 双指针从两端比较
来源：http://se.szsharing.cn

Ruby: s == s.reverse
来源：http://do.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jk.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://zb.jctech888.com.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cr.colortex.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://he.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pv.colortex.cn

TS:   // 手写 Map<string, number>
来源：http://uf.haigaiapp.cn

Java: // 手写 HashMap
来源：http://xa.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://nl.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://et.yuntaijiaju.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gh.jianghongdianzi.cn

[N08] 生成全排列
来源：http://wr.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://at.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://lt.9csxet.cn

JS:   // 手写回溯递归
来源：http://ue.huixinmuqiang.cn

TS:   // 手写回溯递归
来源：http://yf.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ca.asd995.cn

Go:   // 手写回溯递归
来源：http://pd.shtwfgs.cn

Ruby: arr.permutation.to_a
来源：http://nv.nicolike.cn

C#:   // 手写回溯递归
来源：http://xn.panjiajie.cn

[N09] 栈与队列
来源：http://xo.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zy.lnxyls.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wv.yuexingan06.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mn.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bb.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sd.hahajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gs.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yq.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fx.jctech888.com.cn

[N10] 链表节点定义
来源：http://vg.shxzukj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nb.nicolike.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://la.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bc.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sb.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://pz.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xp.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bj.yuexingan06.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ht.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://lh.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kj.nszjky.cn

PHP:  // 手写递归函数
来源：http://tt.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lv.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zl.asd995.cn

Java: // 手写递归
来源：http://qu.huixinmuqiang.cn

Go:   // 手写递归
来源：http://ho.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mv.jianghongdianzi.cn

C#:   // 手写递归
来源：http://sl.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oa.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mx.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zi.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mm.muxihuayi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xu.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ac.9csxet.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vv.jianghongdianzi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ln.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ah.chemitech.net.cn

================================================================================
来源：http://dq.521024.cn

O. 并发与异步
来源：http://nw.huixiangedu.cn

================================================================================
来源：http://nr.jctech888.com.cn

[O01] 启动一个线程
来源：http://zd.jianghongdianzi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ue.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yg.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wu.nicolike.cn

TS:   // 同 JS
来源：http://wf.shtwfgs.cn

Java: new Thread(() -> f()).start()
来源：http://zw.newstarts.cn

Go:   go f()
来源：http://gp.colortex.cn

Ruby: Thread.new { f }
来源：http://lr.chemitech.net.cn

C#:   Task.Run(() => F());
来源：http://ls.hahajie.cn

[O02] 使用线程池
来源：http://ck.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qy.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ad.huanxung.cn

JS:   // worker_threads 线程池
来源：http://ak.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://bl.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vm.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fh.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hh.9csxet.cn


<!-- 参考信息 -->