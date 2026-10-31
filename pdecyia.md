代发 wailian999

================================================================================
来源：http://cx.bjjhwx.cn

K. JSON 与序列化
来源：http://by.panjiajie.cn

================================================================================
来源：http://sk.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ka.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qd.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://re.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://en.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://he.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aa.asd995.cn

Go:   json.Marshal(obj)
来源：http://ou.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qu.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pb.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://ea.521024.cn

Py:   json.loads(s)
来源：http://jf.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qm.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://lg.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://rn.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://er.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://oa.colortex.cn

Ruby: JSON.parse(s)
来源：http://ei.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dn.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://ji.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tf.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kf.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dh.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://au.haigaiapp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gf.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://db.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nq.gzmigu.cn

[K04] 读取 JSON 文件
来源：http://wj.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mw.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ao.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yk.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iv.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vf.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hg.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rp.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://or.szxytkj.cn

[K05] 深拷贝对象
来源：http://xi.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://jf.gzmigu.cn

PHP:  unserialize(serialize($obj));
来源：http://pr.shtwfgs.cn

JS:   structuredClone(obj)
来源：http://zn.nicolike.cn

TS:   structuredClone(obj)
来源：http://il.nszjky.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sm.521024.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://po.lnxyls.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vv.wgjwhj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://se.hahajie.cn

[K06] 解析 URL 查询串
来源：http://uj.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pm.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xe.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dv.bookmarksfly.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cv.haigaiapp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jh.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ip.bookmarksfly.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ax.muxihuayi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uj.panjiajie.cn

[K07] 进制转换
来源：http://at.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hf.shxzskj.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iv.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pd.huixiangedu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bl.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pl.9csxet.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yx.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xe.gzmigu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ad.wgjwhj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ve.asd995.cn

Py:   pickle.dumps(obj)
来源：http://wj.chemitech.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xh.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://gm.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://mi.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pq.szsharing.cn

Go:   encoding/gob
来源：http://fz.yuexingan06.cn

Ruby: Marshal.dump(obj)
来源：http://nv.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qw.panjiajie.cn

================================================================================
来源：http://gt.huanxung.cn

L. 网络请求
来源：http://kr.huixinmuqiang.cn

================================================================================
来源：http://pb.bookmarksfly.cn

[L01] 发送 GET 请求
来源：http://sm.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rl.lnxyls.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fn.shxzukj.cn

JS:   await fetch(url)
来源：http://hi.wgjwhj.cn

TS:   await fetch(url)
来源：http://jt.huanxung.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dt.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://qh.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wa.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zl.lnxyls.cn

[L02] 发送 POST JSON
来源：http://vh.nszjky.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sa.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bm.521024.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qz.nicolike.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oa.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rp.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nu.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zm.huixinmuqiang.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zq.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://rz.shxzskj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uj.bjjhwx.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fo.bookmarksfly.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://md.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cc.colortex.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eb.wgjwhj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vg.shxzukj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vj.521024.cn

[L04] 设置超时
来源：http://dp.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://ag.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rd.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xx.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nu.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ua.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://es.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tx.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://vv.szsharing.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bi.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jb.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oh.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lx.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tm.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ii.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vg.asd995.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xd.9csxet.cn

[L06] 解析响应为 JSON
来源：http://qu.yuntaijiaju.cn

Py:   resp.json()
来源：http://yk.hahajie.cn

PHP:  json_decode($body, true);
来源：http://tj.shxzukj.cn

JS:   await resp.json()
来源：http://xi.hahajie.cn

TS:   await resp.json()
来源：http://uc.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nx.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oq.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://gq.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://va.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://qs.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cn.huanxung.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ym.chemitech.net.cn

JS:   resp.ok;  resp.status
来源：http://jh.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://nl.colortex.cn

Java: resp.statusCode()
来源：http://oi.huanxung.cn

Go:   resp.StatusCode
来源：http://sr.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://dx.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ud.521024.cn

[L08] 并发请求多个地址
来源：http://ir.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nc.521024.cn

PHP:  curl_multi_init() 系列
来源：http://ba.shxzukj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pe.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mt.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jh.shxzskj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rg.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wv.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qa.huixiangedu.cn

================================================================================
来源：http://zw.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://nx.asd995.cn

================================================================================
来源：http://or.wgjwhj.cn

[M01] 读取命令行参数
来源：http://ay.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://po.hahajie.cn

PHP:  $argv;  $argc;
来源：http://ty.szsharing.cn

JS:   process.argv.slice(2)
来源：http://zb.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://jh.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://mu.nszjky.cn

Go:   os.Args[1:]
来源：http://tx.szxytkj.cn

Ruby: ARGV
来源：http://ii.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://kw.nszjky.cn

[M02] 读取环境变量
来源：http://yv.asd995.cn

Py:   os.environ.get("HOME")
来源：http://ym.hnjuh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://os.yuntaijiaju.cn

JS:   process.env.HOME
来源：http://zh.gzmigu.cn

TS:   process.env.HOME
来源：http://sd.panjiajie.cn

Java: System.getenv("HOME")
来源：http://ep.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dp.shtwfgs.cn

Ruby: ENV["HOME"]
来源：http://ju.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sy.huixinmuqiang.cn

[M03] 执行外部命令
来源：http://rv.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ml.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ze.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qb.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xj.nszjky.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sx.lnxyls.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kb.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ck.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://ee.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://fb.panjiajie.cn

Py:   os.getcwd()
来源：http://yo.bjjhwx.cn

PHP:  getcwd();
来源：http://cd.panjiajie.cn

JS:   process.cwd()
来源：http://yo.jianghongdianzi.cn

TS:   process.cwd()
来源：http://bb.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://wq.lnxyls.cn

Go:   os.Getwd()
来源：http://xm.shxzukj.cn

Ruby: Dir.pwd
来源：http://pf.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fg.panjiajie.cn

[M05] 设置退出码
来源：http://hf.bjjhwx.cn

Py:   sys.exit(1)
来源：http://ew.shxzukj.cn

PHP:  exit(1);
来源：http://so.gzmigu.cn

JS:   process.exit(1)
来源：http://ju.hahajie.cn

TS:   process.exit(1)
来源：http://jl.szsharing.cn

Java: System.exit(1)
来源：http://kj.hnjuh.cn

Go:   os.Exit(1)
来源：http://eu.shxzukj.cn

Ruby: exit 1
来源：http://fv.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sg.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://iw.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://bq.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fd.huixiangedu.cn

JS:   console.error("err")
来源：http://ow.wgjwhj.cn

TS:   console.error("err")
来源：http://rl.bjjhwx.cn

Java: System.err.println("err")
来源：http://ld.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://in.bjjhwx.cn

Ruby: warn "err"
来源：http://gj.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://iq.colortex.cn

[M07] 判断是否为主入口
来源：http://ju.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://bs.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ab.shxzskj.cn

JS:   require.main === module
来源：http://ac.colortex.cn

TS:   require.main === module
来源：http://oe.szxytkj.cn

Java: public static void main(String[] args)
来源：http://we.newstarts.cn

Go:   func main()
来源：http://hu.huixiangedu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://os.asd995.cn

C#:   static void Main(string[] args)
来源：http://qx.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://qq.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://ag.colortex.cn

PHP:  PHP_OS;  phpversion();
来源：http://qn.hahajie.cn

JS:   process.platform;  process.version
来源：http://ur.shxzukj.cn

TS:   process.platform;  process.version
来源：http://bg.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yt.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hb.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yz.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nc.hahajie.cn

================================================================================
来源：http://lz.asd995.cn

N. 数据结构与算法
来源：http://tj.szsharing.cn

================================================================================
来源：http://df.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://bc.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lw.jctech888.com.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sa.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ac.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xe.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zg.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://xl.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://do.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oe.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://rl.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bg.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ya.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oh.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eq.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pg.9csxet.cn

Go:   slices.Sort(arr)
来源：http://am.szsharing.cn

Ruby: arr.sort
来源：http://hg.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kk.521024.cn

[N03] 快速排序（分治示例）
来源：http://ks.szxytkj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tr.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://ag.newstarts.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lr.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://le.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://il.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ro.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rj.yuexingan06.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ji.shtwfgs.cn

[N04] 斐波那契数列
来源：http://km.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://td.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bj.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ta.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ut.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vn.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qp.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ti.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gs.huixiangedu.cn

[N05] 最大公约数
来源：http://hj.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://lu.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pk.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://np.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nq.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vh.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ua.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://qc.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ok.lnxyls.cn

[N06] 判断回文字符串
来源：http://qf.nszjky.cn

Py:   s == s[::-1]
来源：http://nw.521024.cn

PHP:  $s === strrev($s);
来源：http://lp.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://kn.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://jv.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ac.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ls.521024.cn

Ruby: s == s.reverse
来源：http://dr.nszjky.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ux.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://bw.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://si.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hd.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mj.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://sm.asd995.cn

Java: // 手写 HashMap
来源：http://ew.szxytkj.cn

Go:   // 手写 map[int]int
来源：http://hf.gzmigu.cn

Ruby: // 手写 Hash
来源：http://sm.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wi.yuntaijiaju.cn

[N08] 生成全排列
来源：http://iu.huixinmuqiang.cn

Py:   itertools.permutations(arr)
来源：http://iy.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://lx.shxzskj.cn

JS:   // 手写回溯递归
来源：http://wk.gzmigu.cn

TS:   // 手写回溯递归
来源：http://xf.yuexingan06.cn

Java: // 手写回溯递归
来源：http://az.muxihuayi.cn

Go:   // 手写回溯递归
来源：http://sz.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://nm.lnxyls.cn

C#:   // 手写回溯递归
来源：http://gz.jianghongdianzi.cn


<!-- 参考信息 -->