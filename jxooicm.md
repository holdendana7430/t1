代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ln.szxytkj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ff.huanxung.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gl.huanxung.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mg.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://at.panjiajie.cn

[K07] 进制转换
来源：http://wa.hahajie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vp.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gv.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zr.bjjhwx.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gb.newstarts.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gt.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fe.bookmarksfly.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vy.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gs.szsharing.cn

[K08] 二进制序列化（非 JSON）
来源：http://kz.newstarts.cn

Py:   pickle.dumps(obj)
来源：http://dt.colortex.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zl.chemitech.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://qv.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://mi.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://se.huixinmuqiang.cn

Go:   encoding/gob
来源：http://lh.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://ra.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hi.yuntaijiaju.cn

================================================================================
来源：http://tj.szxytkj.cn

L. 网络请求
来源：http://lw.9csxet.cn

================================================================================
来源：http://zi.newstarts.cn

[L01] 发送 GET 请求
来源：http://in.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zv.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fg.hnjuh.cn

JS:   await fetch(url)
来源：http://uk.nicolike.cn

TS:   await fetch(url)
来源：http://ac.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mt.hnjuh.cn

Go:   resp, err := http.Get(url)
来源：http://lh.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wr.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dx.hnjuh.cn

[L02] 发送 POST JSON
来源：http://vq.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://us.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zu.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://he.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ze.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vj.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oj.newstarts.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wo.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rj.gzmigu.cn

[L03] 设置自定义请求头
来源：http://mj.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bm.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nr.bookmarksfly.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://an.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://en.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ow.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kt.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hu.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jv.huixinmuqiang.cn

[L04] 设置超时
来源：http://ci.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://wc.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sr.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ty.hnjuh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ss.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cp.lnxyls.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://os.gzmigu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hh.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sr.gzmigu.cn

[L05] 上传文件（multipart）
来源：http://lb.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fa.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ti.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gv.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rg.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vq.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nc.nszjky.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ce.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bu.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://dv.521024.cn

Py:   resp.json()
来源：http://kz.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://bq.newstarts.cn

JS:   await resp.json()
来源：http://uf.colortex.cn

TS:   await resp.json()
来源：http://un.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ix.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://td.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://jo.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pc.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://qo.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rr.gzmigu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rh.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://gn.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://co.szxytkj.cn

Java: resp.statusCode()
来源：http://li.panjiajie.cn

Go:   resp.StatusCode
来源：http://sh.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://ia.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://sv.hahajie.cn

[L08] 并发请求多个地址
来源：http://oo.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://te.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://gh.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gh.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jn.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://an.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rn.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gg.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cp.muxihuayi.cn

================================================================================
来源：http://bu.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://wz.bjjhwx.cn

================================================================================
来源：http://eg.shxzukj.cn

[M01] 读取命令行参数
来源：http://df.shxzukj.cn

Py:   sys.argv[1:]
来源：http://fb.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://rt.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://uf.colortex.cn

TS:   process.argv.slice(2)
来源：http://gm.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://ep.521024.cn

Go:   os.Args[1:]
来源：http://hy.asd995.cn

Ruby: ARGV
来源：http://ln.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ax.nszjky.cn

[M02] 读取环境变量
来源：http://yf.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://mu.asd995.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bv.jctech888.com.cn

JS:   process.env.HOME
来源：http://gx.chemitech.net.cn

TS:   process.env.HOME
来源：http://vh.gzmigu.cn

Java: System.getenv("HOME")
来源：http://la.shxzskj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://te.szsharing.cn

Ruby: ENV["HOME"]
来源：http://rq.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vp.panjiajie.cn

[M03] 执行外部命令
来源：http://gt.huixiangedu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://al.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lr.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://db.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ki.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qp.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bf.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kj.yuntaijiaju.cn

C#:   Process.Start("ls", "-l");
来源：http://kg.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://px.nszjky.cn

Py:   os.getcwd()
来源：http://sr.szxytkj.cn

PHP:  getcwd();
来源：http://ea.yuexingan06.cn

JS:   process.cwd()
来源：http://zc.gzmigu.cn

TS:   process.cwd()
来源：http://tp.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ge.gzmigu.cn

Go:   os.Getwd()
来源：http://bc.colortex.cn

Ruby: Dir.pwd
来源：http://wj.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cy.shxzskj.cn

[M05] 设置退出码
来源：http://ih.shxzukj.cn

Py:   sys.exit(1)
来源：http://dl.panjiajie.cn

PHP:  exit(1);
来源：http://tp.jianghongdianzi.cn

JS:   process.exit(1)
来源：http://af.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://wx.hahajie.cn

Java: System.exit(1)
来源：http://ls.shtwfgs.cn

Go:   os.Exit(1)
来源：http://il.hahajie.cn

Ruby: exit 1
来源：http://bg.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qa.szsharing.cn

[M06] 向标准错误输出
来源：http://ue.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://dx.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tf.yuntaijiaju.cn

JS:   console.error("err")
来源：http://fu.wgjwhj.cn

TS:   console.error("err")
来源：http://my.asd995.cn

Java: System.err.println("err")
来源：http://jl.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mi.muxihuayi.cn

Ruby: warn "err"
来源：http://pg.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://ny.newstarts.cn

[M07] 判断是否为主入口
来源：http://wp.huixinmuqiang.cn

Py:   if __name__ == "__main__":
来源：http://eh.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://er.colortex.cn

JS:   require.main === module
来源：http://xj.nicolike.cn

TS:   require.main === module
来源：http://xj.asd995.cn

Java: public static void main(String[] args)
来源：http://iz.bjjhwx.cn

Go:   func main()
来源：http://jh.gzmigu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mq.nicolike.cn

C#:   static void Main(string[] args)
来源：http://nu.szxytkj.cn

[M08] 获取系统与运行时信息
来源：http://ez.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://dw.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://yl.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://wk.9csxet.cn

TS:   process.platform;  process.version
来源：http://gf.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bh.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fw.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zr.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cr.lnxyls.cn

================================================================================
来源：http://tq.huanxung.cn

N. 数据结构与算法
来源：http://na.9csxet.cn

================================================================================
来源：http://jo.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://lm.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zy.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fk.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mg.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yk.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lz.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://vl.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rh.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bb.shxzskj.cn

[N02] 排序（工程实践用内置实现）
来源：http://hp.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://on.chemitech.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fv.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://or.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bz.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ks.asd995.cn

Go:   slices.Sort(arr)
来源：http://do.nicolike.cn

Ruby: arr.sort
来源：http://li.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://my.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://pr.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qu.huixiangedu.cn

PHP:  // 递归实现，或用 usort
来源：http://ca.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hl.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://if.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kd.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vy.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fx.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://uv.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lb.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wc.newstarts.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kr.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xi.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vp.jianghongdianzi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bg.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ap.lnxyls.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ex.newstarts.cn

[N05] 最大公约数
来源：http://it.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://pr.nszjky.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tu.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qf.shxzskj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://za.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wx.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://du.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://ba.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ak.huanxung.cn

[N06] 判断回文字符串
来源：http://mu.gzmigu.cn

Py:   s == s[::-1]
来源：http://ny.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://th.hnjuh.cn

JS:   s === [...s].reverse().join("")
来源：http://oo.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://iw.huanxung.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://og.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://wm.yuexingan06.cn

Ruby: s == s.reverse
来源：http://od.hnjuh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ks.asd995.cn

[N07] 两数之和（返回下标）
来源：http://fn.huanxung.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mp.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pk.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ti.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://xs.nicolike.cn

Java: // 手写 HashMap
来源：http://fc.nszjky.cn

Go:   // 手写 map[int]int
来源：http://hu.shxzskj.cn

Ruby: // 手写 Hash
来源：http://is.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ci.newstarts.cn

[N08] 生成全排列
来源：http://rz.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://zz.hnjuh.cn

PHP:  // 手写递归交换
来源：http://oq.muxihuayi.cn

JS:   // 手写回溯递归
来源：http://zj.shxzukj.cn

TS:   // 手写回溯递归
来源：http://pi.szxytkj.cn

Java: // 手写回溯递归
来源：http://up.colortex.cn

Go:   // 手写回溯递归
来源：http://cf.9csxet.cn

Ruby: arr.permutation.to_a
来源：http://ay.huanxung.cn

C#:   // 手写回溯递归
来源：http://kp.chemitech.net.cn

[N09] 栈与队列
来源：http://lj.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://im.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gy.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ql.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rp.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hf.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tp.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xf.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sl.szxytkj.cn

[N10] 链表节点定义
来源：http://sf.jianghongdianzi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uz.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ww.nicolike.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hv.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ls.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://vl.nszjky.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xg.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qx.panjiajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ck.gzmigu.cn

[N11] 二叉树中序遍历
来源：http://jq.newstarts.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kp.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://ql.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ah.szsharing.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ks.colortex.cn

Java: // 手写递归
来源：http://wv.shtwfgs.cn

Go:   // 手写递归
来源：http://br.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qa.9csxet.cn

C#:   // 手写递归
来源：http://og.nicolike.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gw.521024.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qn.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ji.521024.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cw.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ut.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iw.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dt.chemitech.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lu.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mm.bjjhwx.cn

================================================================================
来源：http://et.panjiajie.cn

O. 并发与异步
来源：http://uf.szsharing.cn

================================================================================
来源：http://fo.jctech888.com.cn

[O01] 启动一个线程
来源：http://mp.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://my.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yo.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kx.panjiajie.cn

TS:   // 同 JS
来源：http://oy.haigaiapp.cn

Java: new Thread(() -> f()).start()
来源：http://he.gzmigu.cn

Go:   go f()
来源：http://pu.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://iv.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://il.szsharing.cn

[O02] 使用线程池
来源：http://bw.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wr.521024.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cz.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://ui.gzmigu.cn


<!-- 参考信息 -->