代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lq.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mr.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oz.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ii.chemitech.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mi.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ce.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zu.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ka.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://in.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sb.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://yr.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oh.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vd.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pi.huixiangedu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bf.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hs.nicolike.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oi.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yv.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zz.nicolike.cn

[K05] 深拷贝对象
来源：http://kc.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://uw.huixinmuqiang.cn

PHP:  unserialize(serialize($obj));
来源：http://kn.huanxung.cn

JS:   structuredClone(obj)
来源：http://ma.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://lr.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aa.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wi.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nh.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nb.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://sp.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tu.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ot.szsharing.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qb.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gw.bookmarksfly.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tx.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wz.szxytkj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jn.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://to.asd995.cn

[K07] 进制转换
来源：http://hr.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ax.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fv.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dv.jctech888.com.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jo.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fk.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xz.huixiangedu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wh.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rh.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://ei.bookmarksfly.cn

Py:   pickle.dumps(obj)
来源：http://lm.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://va.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://lb.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://jn.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nq.nszjky.cn

Go:   encoding/gob
来源：http://oe.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://pu.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sn.huixinmuqiang.cn

================================================================================
来源：http://xd.gzmigu.cn

L. 网络请求
来源：http://yk.bookmarksfly.cn

================================================================================
来源：http://un.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://fm.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yl.jctech888.com.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zs.nicolike.cn

JS:   await fetch(url)
来源：http://ji.chemitech.net.cn

TS:   await fetch(url)
来源：http://ee.muxihuayi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://si.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://fs.shtwfgs.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zb.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zq.shxzukj.cn

[L02] 发送 POST JSON
来源：http://ml.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eg.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fv.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tl.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gw.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oy.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vm.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jr.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ap.hahajie.cn

[L03] 设置自定义请求头
来源：http://cb.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ao.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fq.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nc.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oq.asd995.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iz.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ht.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zg.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ys.9csxet.cn

[L04] 设置超时
来源：http://ox.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://jt.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://df.bjjhwx.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qf.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nl.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bd.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pf.muxihuayi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xq.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qx.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://lb.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qq.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ed.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dw.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qn.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zb.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pn.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oj.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ek.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://vz.shxzskj.cn

Py:   resp.json()
来源：http://iz.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://tq.jctech888.com.cn

JS:   await resp.json()
来源：http://hl.hnjuh.cn

TS:   await resp.json()
来源：http://uc.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ca.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pu.bjjhwx.cn

Ruby: JSON.parse(resp.body)
来源：http://hv.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vj.wgjwhj.cn

[L07] 处理 HTTP 状态码
来源：http://xz.hahajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://od.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wx.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://cl.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://is.shxzukj.cn

Java: resp.statusCode()
来源：http://oi.shxzukj.cn

Go:   resp.StatusCode
来源：http://ds.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://zm.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://yn.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://kd.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wn.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://qe.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://by.muxihuayi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ys.bjjhwx.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gx.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://py.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://la.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pz.hahajie.cn

================================================================================
来源：http://hk.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://wt.chemitech.net.cn

================================================================================
来源：http://at.nszjky.cn

[M01] 读取命令行参数
来源：http://dc.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://os.hahajie.cn

PHP:  $argv;  $argc;
来源：http://mf.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://bt.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://se.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://ae.bjjhwx.cn

Go:   os.Args[1:]
来源：http://li.hahajie.cn

Ruby: ARGV
来源：http://ht.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://yp.szsharing.cn

[M02] 读取环境变量
来源：http://si.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://ch.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mc.nszjky.cn

JS:   process.env.HOME
来源：http://we.nicolike.cn

TS:   process.env.HOME
来源：http://eg.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ic.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oh.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://kd.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hr.shtwfgs.cn

[M03] 执行外部命令
来源：http://kv.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jy.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://he.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ay.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xd.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://st.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ob.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zf.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://wj.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://ks.szxytkj.cn

Py:   os.getcwd()
来源：http://wp.hnjuh.cn

PHP:  getcwd();
来源：http://lr.hnjuh.cn

JS:   process.cwd()
来源：http://xr.huixiangedu.cn

TS:   process.cwd()
来源：http://rl.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://rk.nszjky.cn

Go:   os.Getwd()
来源：http://so.muxihuayi.cn

Ruby: Dir.pwd
来源：http://yw.panjiajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xp.huanxung.cn

[M05] 设置退出码
来源：http://vt.asd995.cn

Py:   sys.exit(1)
来源：http://ul.colortex.cn

PHP:  exit(1);
来源：http://ow.jctech888.com.cn

JS:   process.exit(1)
来源：http://he.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://ac.huixinmuqiang.cn

Java: System.exit(1)
来源：http://nt.chemitech.net.cn

Go:   os.Exit(1)
来源：http://me.521024.cn

Ruby: exit 1
来源：http://kh.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ne.521024.cn

[M06] 向标准错误输出
来源：http://cn.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://aj.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lk.hnjuh.cn

JS:   console.error("err")
来源：http://nq.9csxet.cn

TS:   console.error("err")
来源：http://wm.wgjwhj.cn

Java: System.err.println("err")
来源：http://wu.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dn.colortex.cn

Ruby: warn "err"
来源：http://sf.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://md.nszjky.cn

[M07] 判断是否为主入口
来源：http://pf.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://zi.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bx.wgjwhj.cn

JS:   require.main === module
来源：http://ha.gzmigu.cn

TS:   require.main === module
来源：http://ga.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://yu.shxzskj.cn

Go:   func main()
来源：http://cb.hnjuh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qj.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://qx.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://fb.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://wx.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://vw.szxytkj.cn

JS:   process.platform;  process.version
来源：http://al.huanxung.cn

TS:   process.platform;  process.version
来源：http://qp.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ux.haigaiapp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gt.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jj.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vv.szxytkj.cn

================================================================================
来源：http://fh.chemitech.net.cn

N. 数据结构与算法
来源：http://xd.chemitech.net.cn

================================================================================
来源：http://yi.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://ah.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zf.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cy.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cp.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sh.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fv.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://im.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://km.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xf.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://lf.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ra.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://we.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rd.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sn.hahajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qg.hahajie.cn

Go:   slices.Sort(arr)
来源：http://hl.chemitech.net.cn

Ruby: arr.sort
来源：http://xd.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jc.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://sp.jianghongdianzi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rn.bookmarksfly.cn

PHP:  // 递归实现，或用 usort
来源：http://rj.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vt.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yn.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jx.wgjwhj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sr.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qd.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bg.shtwfgs.cn

[N04] 斐波那契数列
来源：http://sk.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mm.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qm.huixiangedu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rx.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rt.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cu.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mr.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ax.yuntaijiaju.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://so.shxzskj.cn

[N05] 最大公约数
来源：http://ln.nszjky.cn

Py:   math.gcd(a, b)
来源：http://so.huixiangedu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hj.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rs.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vj.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ff.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wh.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://il.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xu.asd995.cn

[N06] 判断回文字符串
来源：http://tq.asd995.cn

Py:   s == s[::-1]
来源：http://fg.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://on.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://va.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://yv.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cx.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://yz.jianghongdianzi.cn

Ruby: s == s.reverse
来源：http://iq.bookmarksfly.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bo.yuexingan06.cn

[N07] 两数之和（返回下标）
来源：http://fk.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ii.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ul.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oz.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://gz.yuntaijiaju.cn

Java: // 手写 HashMap
来源：http://vk.huanxung.cn

Go:   // 手写 map[int]int
来源：http://nn.szsharing.cn

Ruby: // 手写 Hash
来源：http://mc.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cx.jctech888.com.cn

[N08] 生成全排列
来源：http://qc.colortex.cn

Py:   itertools.permutations(arr)
来源：http://ib.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://am.szxytkj.cn

JS:   // 手写回溯递归
来源：http://gb.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://ai.nszjky.cn

Java: // 手写回溯递归
来源：http://gw.yuexingan06.cn

Go:   // 手写回溯递归
来源：http://sp.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://wf.chemitech.net.cn

C#:   // 手写回溯递归
来源：http://er.chemitech.net.cn

[N09] 栈与队列
来源：http://rx.huanxung.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://of.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mq.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ne.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mh.shxzukj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hf.huixinmuqiang.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ub.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ck.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hs.huanxung.cn

[N10] 链表节点定义
来源：http://gy.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hp.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nj.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qt.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ba.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://ra.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kn.bjjhwx.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zy.9csxet.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ai.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://fc.shtwfgs.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cf.huanxung.cn


<!-- 参考信息 -->