代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ny.9csxet.cn

Go:   json.Marshal(obj)
来源：http://zb.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ya.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tv.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://qa.szsharing.cn

Py:   json.loads(s)
来源：http://ze.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gp.shxzukj.cn

JS:   JSON.parse(s)
来源：http://xp.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://pq.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fj.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://jp.9csxet.cn

Ruby: JSON.parse(s)
来源：http://er.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ot.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://kq.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dt.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gm.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dr.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wx.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sx.gzmigu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qk.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qc.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hb.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://up.haigaiapp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sh.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ii.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ct.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oj.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ii.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xs.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ob.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wk.asd995.cn

[K05] 深拷贝对象
来源：http://yx.gzmigu.cn

Py:   copy.deepcopy(obj)
来源：http://jj.colortex.cn

PHP:  unserialize(serialize($obj));
来源：http://tz.shxzskj.cn

JS:   structuredClone(obj)
来源：http://pf.panjiajie.cn

TS:   structuredClone(obj)
来源：http://mk.haigaiapp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qb.muxihuayi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ji.nszjky.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yo.colortex.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hm.szsharing.cn

[K06] 解析 URL 查询串
来源：http://my.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cm.yuntaijiaju.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ld.521024.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yu.huixinmuqiang.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dy.yuntaijiaju.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://el.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mu.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tv.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ho.szxytkj.cn

[K07] 进制转换
来源：http://yo.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hv.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vd.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vf.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hw.yuexingan06.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vy.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://za.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fu.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mj.colortex.cn

[K08] 二进制序列化（非 JSON）
来源：http://ha.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://re.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ot.9csxet.cn

JS:   v8.serialize(obj)        // Node
来源：http://tm.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://qh.huixiangedu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ux.nszjky.cn

Go:   encoding/gob
来源：http://nc.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://ut.chemitech.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ru.muxihuayi.cn

================================================================================
来源：http://ez.newstarts.cn

L. 网络请求
来源：http://ap.nicolike.cn

================================================================================
来源：http://az.gzmigu.cn

[L01] 发送 GET 请求
来源：http://mp.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ck.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kv.gzmigu.cn

JS:   await fetch(url)
来源：http://xt.huanxung.cn

TS:   await fetch(url)
来源：http://dx.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ns.muxihuayi.cn

Go:   resp, err := http.Get(url)
来源：http://li.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lt.haigaiapp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rl.huanxung.cn

[L02] 发送 POST JSON
来源：http://iq.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sx.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hs.nicolike.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bv.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jm.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kq.bookmarksfly.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ym.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mr.huixiangedu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vp.nicolike.cn

[L03] 设置自定义请求头
来源：http://kx.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ng.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ad.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sd.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pm.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vp.chemitech.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ms.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bs.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xp.newstarts.cn

[L04] 设置超时
来源：http://db.yuntaijiaju.cn

Py:   requests.get(url, timeout=5)
来源：http://fg.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jt.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ap.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://af.nszjky.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vu.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wg.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wk.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ot.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://ab.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hb.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fi.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wt.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ry.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ne.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ny.szsharing.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dm.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mt.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://qm.huixinmuqiang.cn

Py:   resp.json()
来源：http://qk.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://ul.hahajie.cn

JS:   await resp.json()
来源：http://ja.colortex.cn

TS:   await resp.json()
来源：http://lx.shxzskj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ih.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zu.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://bk.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mr.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://ct.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://af.shxzukj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rw.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://xs.muxihuayi.cn

TS:   resp.ok;  resp.status
来源：http://ps.wgjwhj.cn

Java: resp.statusCode()
来源：http://ir.huanxung.cn

Go:   resp.StatusCode
来源：http://vf.shxzskj.cn

Ruby: resp.code.to_i
来源：http://zm.521024.cn

C#:   (int)resp.StatusCode
来源：http://lk.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://yj.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wr.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://fs.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kr.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wf.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zl.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qe.lnxyls.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ww.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tl.muxihuayi.cn

================================================================================
来源：http://tz.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://cm.hnjuh.cn

================================================================================
来源：http://mq.muxihuayi.cn

[M01] 读取命令行参数
来源：http://di.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://jm.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://ky.colortex.cn

JS:   process.argv.slice(2)
来源：http://ag.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://hv.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://bb.521024.cn

Go:   os.Args[1:]
来源：http://cp.521024.cn

Ruby: ARGV
来源：http://kj.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://zw.521024.cn

[M02] 读取环境变量
来源：http://yn.colortex.cn

Py:   os.environ.get("HOME")
来源：http://in.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rd.huixiangedu.cn

JS:   process.env.HOME
来源：http://oq.chemitech.net.cn

TS:   process.env.HOME
来源：http://zo.gzmigu.cn

Java: System.getenv("HOME")
来源：http://mb.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ak.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://bw.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sh.hnjuh.cn

[M03] 执行外部命令
来源：http://nl.lnxyls.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oi.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bv.szsharing.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jo.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ti.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://or.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cd.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://co.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://gm.lnxyls.cn

[M04] 获取当前工作目录
来源：http://le.yuexingan06.cn

Py:   os.getcwd()
来源：http://cp.panjiajie.cn

PHP:  getcwd();
来源：http://yo.shtwfgs.cn

JS:   process.cwd()
来源：http://rw.shxzukj.cn

TS:   process.cwd()
来源：http://iu.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://vu.szxytkj.cn

Go:   os.Getwd()
来源：http://pe.9csxet.cn

Ruby: Dir.pwd
来源：http://yr.asd995.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gt.haigaiapp.cn

[M05] 设置退出码
来源：http://od.shxzskj.cn

Py:   sys.exit(1)
来源：http://ah.hnjuh.cn

PHP:  exit(1);
来源：http://vh.asd995.cn

JS:   process.exit(1)
来源：http://ck.huixiangedu.cn

TS:   process.exit(1)
来源：http://sb.bjjhwx.cn

Java: System.exit(1)
来源：http://kc.lnxyls.cn

Go:   os.Exit(1)
来源：http://fp.9csxet.cn

Ruby: exit 1
来源：http://gv.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rj.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://ua.asd995.cn

Py:   print("err", file=sys.stderr)
来源：http://vu.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ur.shxzukj.cn

JS:   console.error("err")
来源：http://yh.9csxet.cn

TS:   console.error("err")
来源：http://xr.panjiajie.cn

Java: System.err.println("err")
来源：http://gi.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sm.chemitech.net.cn

Ruby: warn "err"
来源：http://sg.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://do.shxzukj.cn

[M07] 判断是否为主入口
来源：http://dx.jctech888.com.cn

Py:   if __name__ == "__main__":
来源：http://hk.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zu.muxihuayi.cn

JS:   require.main === module
来源：http://zc.bookmarksfly.cn

TS:   require.main === module
来源：http://uu.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ze.nicolike.cn

Go:   func main()
来源：http://st.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://du.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://fy.huanxung.cn

[M08] 获取系统与运行时信息
来源：http://fn.haigaiapp.cn

Py:   platform.system();  platform.python_version()
来源：http://ss.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://hp.521024.cn

JS:   process.platform;  process.version
来源：http://xk.521024.cn

TS:   process.platform;  process.version
来源：http://zv.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zi.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mm.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qb.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pf.jianghongdianzi.cn

================================================================================
来源：http://tc.nicolike.cn

N. 数据结构与算法
来源：http://to.szsharing.cn

================================================================================
来源：http://qw.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://hc.gzmigu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hb.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cs.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://es.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://he.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cs.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://er.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://up.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sa.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ll.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://lu.newstarts.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tc.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uo.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fh.huanxung.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://py.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://yg.muxihuayi.cn

Ruby: arr.sort
来源：http://pe.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://is.bookmarksfly.cn

[N03] 快速排序（分治示例）
来源：http://gi.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dy.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://co.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jy.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aw.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://os.jianghongdianzi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://py.jctech888.com.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ae.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bd.521024.cn

[N04] 斐波那契数列
来源：http://pc.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sk.521024.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pl.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ks.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bw.bookmarksfly.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lr.wgjwhj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xd.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nw.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://es.yuntaijiaju.cn

[N05] 最大公约数
来源：http://fw.gzmigu.cn

Py:   math.gcd(a, b)
来源：http://ls.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bq.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mw.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dm.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pa.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ao.gzmigu.cn

Ruby: a.gcd(b)
来源：http://bk.huixiangedu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ae.nszjky.cn

[N06] 判断回文字符串
来源：http://kh.yuexingan06.cn

Py:   s == s[::-1]
来源：http://fx.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://iw.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://pa.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://vi.yuexingan06.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ke.colortex.cn

Go:   // 双指针从两端比较
来源：http://th.szsharing.cn

Ruby: s == s.reverse
来源：http://ws.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fp.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://sw.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wz.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://li.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gu.chemitech.net.cn

TS:   // 手写 Map<string, number>
来源：http://da.haigaiapp.cn

Java: // 手写 HashMap
来源：http://om.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://hp.panjiajie.cn

Ruby: // 手写 Hash
来源：http://rt.jctech888.com.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ri.panjiajie.cn

[N08] 生成全排列
来源：http://ox.shtwfgs.cn

Py:   itertools.permutations(arr)
来源：http://hj.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://tj.wgjwhj.cn

JS:   // 手写回溯递归
来源：http://df.huanxung.cn

TS:   // 手写回溯递归
来源：http://yt.huanxung.cn

Java: // 手写回溯递归
来源：http://uf.hahajie.cn

Go:   // 手写回溯递归
来源：http://qw.hahajie.cn

Ruby: arr.permutation.to_a
来源：http://yc.hahajie.cn

C#:   // 手写回溯递归
来源：http://ad.nszjky.cn

[N09] 栈与队列
来源：http://od.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sc.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mx.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cx.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qk.asd995.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://de.jctech888.com.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sf.nicolike.cn


<!-- 参考信息 -->