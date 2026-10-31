代发 wailian999

[K06] 解析 URL 查询串
来源：http://dz.shtwfgs.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kp.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gj.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://si.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nm.huanxung.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gy.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vl.asd995.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ff.huanxung.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xk.huixiangedu.cn

[K07] 进制转换
来源：http://os.colortex.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aa.szsharing.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gq.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kl.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sq.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dl.nicolike.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lz.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://be.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yd.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ks.9csxet.cn

Py:   pickle.dumps(obj)
来源：http://jx.521024.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dn.521024.cn

JS:   v8.serialize(obj)        // Node
来源：http://pb.shxzskj.cn

TS:   v8.serialize(obj)        // Node
来源：http://jz.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ho.bookmarksfly.cn

Go:   encoding/gob
来源：http://cw.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://qt.huixinmuqiang.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zp.newstarts.cn

================================================================================
来源：http://qu.huixiangedu.cn

L. 网络请求
来源：http://sf.panjiajie.cn

================================================================================
来源：http://xa.lnxyls.cn

[L01] 发送 GET 请求
来源：http://an.9csxet.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wz.jianghongdianzi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wd.panjiajie.cn

JS:   await fetch(url)
来源：http://jt.nicolike.cn

TS:   await fetch(url)
来源：http://ke.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://za.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://rp.jianghongdianzi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mp.jianghongdianzi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ql.shxzskj.cn

[L02] 发送 POST JSON
来源：http://on.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dr.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zn.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wm.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nj.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nu.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gy.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://od.shtwfgs.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://no.chemitech.net.cn

[L03] 设置自定义请求头
来源：http://cy.huanxung.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bj.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gs.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hh.yuntaijiaju.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ps.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ky.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iv.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://md.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://km.newstarts.cn

[L04] 设置超时
来源：http://cl.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://sx.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uo.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vt.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://no.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wi.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xj.shxzskj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zs.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bi.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://pc.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sh.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aj.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vo.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ky.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yw.jctech888.com.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zi.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hy.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qm.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://ew.bookmarksfly.cn

Py:   resp.json()
来源：http://py.nszjky.cn

PHP:  json_decode($body, true);
来源：http://ep.hnjuh.cn

JS:   await resp.json()
来源：http://ew.shxzukj.cn

TS:   await resp.json()
来源：http://gn.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lw.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dn.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://ra.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rv.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://ec.colortex.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ln.lnxyls.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ge.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://gg.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://vt.muxihuayi.cn

Java: resp.statusCode()
来源：http://fc.hahajie.cn

Go:   resp.StatusCode
来源：http://hm.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://sz.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://dd.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://ak.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sn.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://fb.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gk.bookmarksfly.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vk.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vz.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mx.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fm.521024.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uq.wgjwhj.cn

================================================================================
来源：http://ab.hahajie.cn

M. 命令行 / 进程 / 环境
来源：http://ga.bjjhwx.cn

================================================================================
来源：http://bg.szsharing.cn

[M01] 读取命令行参数
来源：http://vh.haigaiapp.cn

Py:   sys.argv[1:]
来源：http://xc.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://qi.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://jy.gzmigu.cn

TS:   process.argv.slice(2)
来源：http://wk.szxytkj.cn

Java: args 数组（main 方法参数）
来源：http://im.szxytkj.cn

Go:   os.Args[1:]
来源：http://pa.gzmigu.cn

Ruby: ARGV
来源：http://bd.huixinmuqiang.cn

C#:   args 数组（Main 方法参数）
来源：http://fr.521024.cn

[M02] 读取环境变量
来源：http://ak.yuntaijiaju.cn

Py:   os.environ.get("HOME")
来源：http://yt.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bu.muxihuayi.cn

JS:   process.env.HOME
来源：http://np.nszjky.cn

TS:   process.env.HOME
来源：http://ik.szsharing.cn

Java: System.getenv("HOME")
来源：http://hz.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vf.jianghongdianzi.cn

Ruby: ENV["HOME"]
来源：http://oq.jianghongdianzi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ks.nszjky.cn

[M03] 执行外部命令
来源：http://fk.gzmigu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fd.hahajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qu.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dp.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://of.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uw.szsharing.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nd.panjiajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bj.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ot.szsharing.cn

[M04] 获取当前工作目录
来源：http://ih.nicolike.cn

Py:   os.getcwd()
来源：http://hk.bjjhwx.cn

PHP:  getcwd();
来源：http://gf.hahajie.cn

JS:   process.cwd()
来源：http://fn.huixiangedu.cn

TS:   process.cwd()
来源：http://nz.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://at.asd995.cn

Go:   os.Getwd()
来源：http://zn.521024.cn

Ruby: Dir.pwd
来源：http://qv.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rp.hnjuh.cn

[M05] 设置退出码
来源：http://zg.gzmigu.cn

Py:   sys.exit(1)
来源：http://il.huanxung.cn

PHP:  exit(1);
来源：http://co.nszjky.cn

JS:   process.exit(1)
来源：http://sh.shxzukj.cn

TS:   process.exit(1)
来源：http://jk.nicolike.cn

Java: System.exit(1)
来源：http://yg.huixiangedu.cn

Go:   os.Exit(1)
来源：http://ch.yuexingan06.cn

Ruby: exit 1
来源：http://zt.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iv.haigaiapp.cn

[M06] 向标准错误输出
来源：http://ep.gzmigu.cn

Py:   print("err", file=sys.stderr)
来源：http://xz.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ww.jctech888.com.cn

JS:   console.error("err")
来源：http://sk.hahajie.cn

TS:   console.error("err")
来源：http://cs.haigaiapp.cn

Java: System.err.println("err")
来源：http://ht.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qi.hnjuh.cn

Ruby: warn "err"
来源：http://jw.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://zm.huanxung.cn

[M07] 判断是否为主入口
来源：http://bx.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://iv.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hu.colortex.cn

JS:   require.main === module
来源：http://hn.szsharing.cn

TS:   require.main === module
来源：http://qt.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://kh.szxytkj.cn

Go:   func main()
来源：http://gc.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uf.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://yy.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://mu.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://ja.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://lc.muxihuayi.cn

JS:   process.platform;  process.version
来源：http://tv.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://lc.yuntaijiaju.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xm.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ll.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ow.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dj.gzmigu.cn

================================================================================
来源：http://mj.shxzskj.cn

N. 数据结构与算法
来源：http://nz.gzmigu.cn

================================================================================
来源：http://zg.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://nk.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tk.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ds.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lt.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qn.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zp.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://dx.huanxung.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rq.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pz.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://kh.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://rq.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wq.shxzskj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bg.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ag.wgjwhj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dx.szsharing.cn

Go:   slices.Sort(arr)
来源：http://wo.9csxet.cn

Ruby: arr.sort
来源：http://io.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zj.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://nb.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://di.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://ki.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ns.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ow.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uz.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://si.huixiangedu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ed.huixiangedu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ae.jctech888.com.cn

[N04] 斐波那契数列
来源：http://ay.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ea.hnjuh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bs.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fp.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kd.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vf.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cu.jianghongdianzi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cy.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bv.jctech888.com.cn

[N05] 最大公约数
来源：http://gs.huanxung.cn

Py:   math.gcd(a, b)
来源：http://py.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gt.panjiajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iu.lnxyls.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kx.yuexingan06.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://po.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ql.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://df.yuexingan06.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oo.szxytkj.cn

[N06] 判断回文字符串
来源：http://fo.szxytkj.cn

Py:   s == s[::-1]
来源：http://af.yuexingan06.cn

PHP:  $s === strrev($s);
来源：http://wt.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://dq.nicolike.cn

TS:   s === [...s].reverse().join("")
来源：http://wy.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tl.521024.cn

Go:   // 双指针从两端比较
来源：http://lm.muxihuayi.cn

Ruby: s == s.reverse
来源：http://ek.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hy.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://ur.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sr.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://da.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vc.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://og.panjiajie.cn

Java: // 手写 HashMap
来源：http://wt.shxzskj.cn

Go:   // 手写 map[int]int
来源：http://fh.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://up.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bv.shxzukj.cn

[N08] 生成全排列
来源：http://kk.chemitech.net.cn

Py:   itertools.permutations(arr)
来源：http://kb.9csxet.cn

PHP:  // 手写递归交换
来源：http://nc.huixinmuqiang.cn

JS:   // 手写回溯递归
来源：http://kj.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://mo.huixiangedu.cn

Java: // 手写回溯递归
来源：http://gd.9csxet.cn

Go:   // 手写回溯递归
来源：http://un.nicolike.cn

Ruby: arr.permutation.to_a
来源：http://oa.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://aq.bjjhwx.cn

[N09] 栈与队列
来源：http://ln.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hg.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mv.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xj.shtwfgs.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xi.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qh.jianghongdianzi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rn.szxytkj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kd.jianghongdianzi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nr.newstarts.cn

[N10] 链表节点定义
来源：http://jn.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xo.lnxyls.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xi.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sz.9csxet.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zu.yuexingan06.cn

Java: class Node { int v; Node next; }
来源：http://th.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nq.521024.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ut.521024.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://li.newstarts.cn

[N11] 二叉树中序遍历
来源：http://yu.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ov.nszjky.cn

PHP:  // 手写递归函数
来源：http://lb.chemitech.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ue.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ux.nicolike.cn

Java: // 手写递归
来源：http://pf.shxzskj.cn

Go:   // 手写递归
来源：http://gv.shxzukj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://al.lnxyls.cn

C#:   // 手写递归
来源：http://ri.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uj.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ql.gzmigu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pu.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bk.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fn.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tq.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kl.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://au.shxzskj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oc.colortex.cn

================================================================================
来源：http://ty.bookmarksfly.cn

O. 并发与异步
来源：http://ek.szxytkj.cn

================================================================================
来源：http://dw.asd995.cn

[O01] 启动一个线程
来源：http://si.haigaiapp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nb.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sd.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://px.nszjky.cn

TS:   // 同 JS
来源：http://jx.huanxung.cn

Java: new Thread(() -> f()).start()
来源：http://lx.huixiangedu.cn

Go:   go f()
来源：http://rg.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://jb.nicolike.cn

C#:   Task.Run(() => F());
来源：http://gi.hnjuh.cn


<!-- 参考信息 -->