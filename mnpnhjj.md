代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xp.nicolike.cn

Go:   json.Marshal(obj)
来源：http://ya.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mg.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mh.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://bt.chemitech.net.cn

Py:   json.loads(s)
来源：http://hf.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wo.lnxyls.cn

JS:   JSON.parse(s)
来源：http://hy.newstarts.cn

TS:   JSON.parse(s)
来源：http://ct.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yt.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://wx.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://cl.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eg.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://fe.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kt.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pn.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eo.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ob.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qs.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fw.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xo.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sb.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://hu.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jl.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pb.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fp.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ff.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sf.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://em.chemitech.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cw.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mj.hnjuh.cn

[K05] 深拷贝对象
来源：http://xa.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://hu.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ex.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://tp.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://so.colortex.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://na.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oa.bjjhwx.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tm.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sf.newstarts.cn

[K06] 解析 URL 查询串
来源：http://ts.lnxyls.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bj.huixiangedu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ju.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rj.hahajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wo.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jq.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qv.hahajie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gc.jianghongdianzi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ek.9csxet.cn

[K07] 进制转换
来源：http://lm.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jt.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ce.521024.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dn.jianghongdianzi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://do.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vz.chemitech.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wq.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sx.bookmarksfly.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jz.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://ee.nszjky.cn

Py:   pickle.dumps(obj)
来源：http://hc.szsharing.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kj.szxytkj.cn

JS:   v8.serialize(obj)        // Node
来源：http://oc.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://jm.shxzukj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ix.chemitech.net.cn

Go:   encoding/gob
来源：http://kw.hahajie.cn

Ruby: Marshal.dump(obj)
来源：http://qr.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sw.szxytkj.cn

================================================================================
来源：http://nz.panjiajie.cn

L. 网络请求
来源：http://vj.panjiajie.cn

================================================================================
来源：http://gb.lnxyls.cn

[L01] 发送 GET 请求
来源：http://eu.hahajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nx.haigaiapp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rh.shxzskj.cn

JS:   await fetch(url)
来源：http://rl.panjiajie.cn

TS:   await fetch(url)
来源：http://tj.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vq.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://ov.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ur.newstarts.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vd.yuntaijiaju.cn

[L02] 发送 POST JSON
来源：http://mb.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sp.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qx.huixinmuqiang.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nf.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ry.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nx.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://se.asd995.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jl.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://it.521024.cn

[L03] 设置自定义请求头
来源：http://ye.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rg.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vc.521024.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://py.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pk.shxzskj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zf.huixinmuqiang.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iz.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vl.szxytkj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ul.huixinmuqiang.cn

[L04] 设置超时
来源：http://dk.colortex.cn

Py:   requests.get(url, timeout=5)
来源：http://pj.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yd.muxihuayi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mq.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jp.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yb.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ro.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mp.521024.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zm.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://rw.huixinmuqiang.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ak.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wb.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uq.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ue.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ix.huixinmuqiang.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fg.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dc.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kp.521024.cn

[L06] 解析响应为 JSON
来源：http://nw.shxzukj.cn

Py:   resp.json()
来源：http://hr.panjiajie.cn

PHP:  json_decode($body, true);
来源：http://ks.jctech888.com.cn

JS:   await resp.json()
来源：http://um.huanxung.cn

TS:   await resp.json()
来源：http://vc.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qh.jctech888.com.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rf.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://or.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pg.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://jw.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oe.nicolike.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lq.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://zn.bjjhwx.cn

TS:   resp.ok;  resp.status
来源：http://xj.muxihuayi.cn

Java: resp.statusCode()
来源：http://ym.shxzskj.cn

Go:   resp.StatusCode
来源：http://ta.newstarts.cn

Ruby: resp.code.to_i
来源：http://rj.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://gt.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://ia.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://db.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://cf.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bl.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zt.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://id.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xe.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pv.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ja.bookmarksfly.cn

================================================================================
来源：http://jw.521024.cn

M. 命令行 / 进程 / 环境
来源：http://vx.9csxet.cn

================================================================================
来源：http://po.bookmarksfly.cn

[M01] 读取命令行参数
来源：http://cx.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://zp.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://cn.asd995.cn

JS:   process.argv.slice(2)
来源：http://iq.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://ch.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://gc.gzmigu.cn

Go:   os.Args[1:]
来源：http://ku.colortex.cn

Ruby: ARGV
来源：http://oc.huanxung.cn

C#:   args 数组（Main 方法参数）
来源：http://xk.shxzskj.cn

[M02] 读取环境变量
来源：http://gz.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://jw.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rr.szsharing.cn

JS:   process.env.HOME
来源：http://ov.lnxyls.cn

TS:   process.env.HOME
来源：http://yr.newstarts.cn

Java: System.getenv("HOME")
来源：http://pv.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ma.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://yu.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xi.nszjky.cn

[M03] 执行外部命令
来源：http://wp.asd995.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dr.colortex.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xh.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ua.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ux.shtwfgs.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zr.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hp.szsharing.cn

Ruby: system("ls -l");  `ls -l`
来源：http://um.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://sj.shtwfgs.cn

[M04] 获取当前工作目录
来源：http://zp.newstarts.cn

Py:   os.getcwd()
来源：http://ps.shtwfgs.cn

PHP:  getcwd();
来源：http://fx.huixinmuqiang.cn

JS:   process.cwd()
来源：http://uc.bookmarksfly.cn

TS:   process.cwd()
来源：http://ab.wgjwhj.cn

Java: Path.of("").toAbsolutePath()
来源：http://pi.shxzukj.cn

Go:   os.Getwd()
来源：http://ee.newstarts.cn

Ruby: Dir.pwd
来源：http://rv.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dn.bookmarksfly.cn

[M05] 设置退出码
来源：http://vg.gzmigu.cn

Py:   sys.exit(1)
来源：http://gi.shxzukj.cn

PHP:  exit(1);
来源：http://zb.newstarts.cn

JS:   process.exit(1)
来源：http://tl.lnxyls.cn

TS:   process.exit(1)
来源：http://rf.newstarts.cn

Java: System.exit(1)
来源：http://eq.szsharing.cn

Go:   os.Exit(1)
来源：http://be.szsharing.cn

Ruby: exit 1
来源：http://xg.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pv.nszjky.cn

[M06] 向标准错误输出
来源：http://qs.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ii.gzmigu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://br.huanxung.cn

JS:   console.error("err")
来源：http://cl.nszjky.cn

TS:   console.error("err")
来源：http://vz.jctech888.com.cn

Java: System.err.println("err")
来源：http://ra.szsharing.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hx.shxzukj.cn

Ruby: warn "err"
来源：http://pb.asd995.cn

C#:   Console.Error.WriteLine("err")
来源：http://ci.szsharing.cn

[M07] 判断是否为主入口
来源：http://wi.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://li.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hg.bjjhwx.cn

JS:   require.main === module
来源：http://dt.yuntaijiaju.cn

TS:   require.main === module
来源：http://zy.lnxyls.cn

Java: public static void main(String[] args)
来源：http://to.yuntaijiaju.cn

Go:   func main()
来源：http://la.yuexingan06.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ye.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://kc.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://kd.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://om.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://vu.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://zq.9csxet.cn

TS:   process.platform;  process.version
来源：http://yd.jctech888.com.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ic.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jn.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xn.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zu.shxzukj.cn

================================================================================
来源：http://fv.jctech888.com.cn

N. 数据结构与算法
来源：http://jr.yuexingan06.cn

================================================================================
来源：http://qw.colortex.cn

[N01] 二分查找（有序数组）
来源：http://vx.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ih.nszjky.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xe.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ah.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mk.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fw.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://aa.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fz.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wc.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://vy.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://sd.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zm.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uq.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lk.bookmarksfly.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vk.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://kj.colortex.cn

Ruby: arr.sort
来源：http://wh.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kn.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://zc.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sk.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://lr.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sh.huanxung.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tg.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xh.panjiajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ms.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iz.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uq.yuntaijiaju.cn

[N04] 斐波那契数列
来源：http://lp.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tg.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lq.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yj.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rp.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sx.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vo.wgjwhj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xf.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cr.jianghongdianzi.cn

[N05] 最大公约数
来源：http://qi.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://kr.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ov.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wi.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wi.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bj.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gu.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ft.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zs.gzmigu.cn

[N06] 判断回文字符串
来源：http://xm.szxytkj.cn

Py:   s == s[::-1]
来源：http://av.shxzukj.cn

PHP:  $s === strrev($s);
来源：http://zu.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://dx.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://dk.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ci.hnjuh.cn

Go:   // 双指针从两端比较
来源：http://yw.bjjhwx.cn

Ruby: s == s.reverse
来源：http://oy.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cs.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://be.panjiajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vs.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ck.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yf.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://pd.yuexingan06.cn

Java: // 手写 HashMap
来源：http://pd.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://gd.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://zx.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://br.jianghongdianzi.cn

[N08] 生成全排列
来源：http://ds.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://ub.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://gz.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://vi.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://qz.lnxyls.cn

Java: // 手写回溯递归
来源：http://yp.gzmigu.cn

Go:   // 手写回溯递归
来源：http://jp.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://xi.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://uh.yuntaijiaju.cn

[N09] 栈与队列
来源：http://bg.chemitech.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yw.nicolike.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wj.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jv.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tv.chemitech.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pw.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pg.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xf.huixiangedu.cn


<!-- 参考信息 -->