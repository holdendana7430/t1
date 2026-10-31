代发 wailian999

================================================================================
来源：http://hd.shxzukj.cn

K. JSON 与序列化
来源：http://rq.haigaiapp.cn

================================================================================
来源：http://xp.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://xw.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://db.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qo.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://dk.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://nl.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fb.szxytkj.cn

Go:   json.Marshal(obj)
来源：http://ls.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vv.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wr.hahajie.cn

[K02] JSON 字符串转对象
来源：http://jx.chemitech.net.cn

Py:   json.loads(s)
来源：http://zz.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.shxzskj.cn

JS:   JSON.parse(s)
来源：http://cm.haigaiapp.cn

TS:   JSON.parse(s)
来源：http://ay.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lh.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://br.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://nu.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://le.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://dq.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ck.asd995.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://al.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hj.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zh.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pk.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ek.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mf.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zn.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://vf.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jw.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xi.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zz.chemitech.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gz.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yw.szsharing.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eb.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gz.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ep.asd995.cn

[K05] 深拷贝对象
来源：http://xg.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://lr.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://wu.nszjky.cn

JS:   structuredClone(obj)
来源：http://vg.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://oi.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ia.jctech888.com.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://li.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oj.huixiangedu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kd.shxzskj.cn

[K06] 解析 URL 查询串
来源：http://bw.bookmarksfly.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pj.nszjky.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ci.chemitech.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zn.yuexingan06.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bh.shxzskj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ew.bookmarksfly.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sw.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://li.jctech888.com.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pk.hnjuh.cn

[K07] 进制转换
来源：http://ch.nszjky.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yk.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ch.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://li.shxzskj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gv.bjjhwx.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fa.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pa.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rl.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://se.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://kx.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://df.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gi.huanxung.cn

JS:   v8.serialize(obj)        // Node
来源：http://nk.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://ld.asd995.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hp.huixinmuqiang.cn

Go:   encoding/gob
来源：http://qi.9csxet.cn

Ruby: Marshal.dump(obj)
来源：http://lf.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ix.gzmigu.cn

================================================================================
来源：http://ab.bjjhwx.cn

L. 网络请求
来源：http://jy.haigaiapp.cn

================================================================================
来源：http://xd.szxytkj.cn

[L01] 发送 GET 请求
来源：http://op.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qw.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lh.colortex.cn

JS:   await fetch(url)
来源：http://fk.jctech888.com.cn

TS:   await fetch(url)
来源：http://wd.gzmigu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mw.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://or.huixinmuqiang.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yh.huixiangedu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xt.panjiajie.cn

[L02] 发送 POST JSON
来源：http://vh.hnjuh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dj.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ff.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rv.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ys.shxzukj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xa.szsharing.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rh.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ll.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://er.newstarts.cn

[L03] 设置自定义请求头
来源：http://gs.huixinmuqiang.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://co.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://no.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lv.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ik.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://um.panjiajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pj.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ms.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yg.shxzukj.cn

[L04] 设置超时
来源：http://hc.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://rf.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cn.yuntaijiaju.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lp.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qq.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bn.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ex.panjiajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sw.nicolike.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dy.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://sf.szxytkj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ew.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ec.9csxet.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xs.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://za.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.gzmigu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xw.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xz.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nl.colortex.cn

[L06] 解析响应为 JSON
来源：http://tl.shxzukj.cn

Py:   resp.json()
来源：http://wu.colortex.cn

PHP:  json_decode($body, true);
来源：http://pi.colortex.cn

JS:   await resp.json()
来源：http://vz.jctech888.com.cn

TS:   await resp.json()
来源：http://wo.hahajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wy.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xh.huixiangedu.cn

Ruby: JSON.parse(resp.body)
来源：http://wu.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sf.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://yw.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kv.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zy.nszjky.cn

JS:   resp.ok;  resp.status
来源：http://dr.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://td.521024.cn

Java: resp.statusCode()
来源：http://rn.hnjuh.cn

Go:   resp.StatusCode
来源：http://eq.hnjuh.cn

Ruby: resp.code.to_i
来源：http://tq.shtwfgs.cn

C#:   (int)resp.StatusCode
来源：http://dj.521024.cn

[L08] 并发请求多个地址
来源：http://nz.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bm.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://fs.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wu.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://so.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vf.jctech888.com.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bi.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yy.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mf.colortex.cn

================================================================================
来源：http://zb.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://xk.hnjuh.cn

================================================================================
来源：http://dk.lnxyls.cn

[M01] 读取命令行参数
来源：http://kt.chemitech.net.cn

Py:   sys.argv[1:]
来源：http://zz.521024.cn

PHP:  $argv;  $argc;
来源：http://fg.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://va.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://ty.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://jt.asd995.cn

Go:   os.Args[1:]
来源：http://mx.shtwfgs.cn

Ruby: ARGV
来源：http://ju.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://go.yuexingan06.cn

[M02] 读取环境变量
来源：http://gr.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://no.jctech888.com.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ai.muxihuayi.cn

JS:   process.env.HOME
来源：http://jy.shxzukj.cn

TS:   process.env.HOME
来源：http://kp.asd995.cn

Java: System.getenv("HOME")
来源：http://ag.muxihuayi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rq.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://cu.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wg.panjiajie.cn

[M03] 执行外部命令
来源：http://gd.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kf.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wp.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://al.lnxyls.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cw.huixiangedu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kk.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://as.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mm.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://pk.huanxung.cn

[M04] 获取当前工作目录
来源：http://pc.huanxung.cn

Py:   os.getcwd()
来源：http://aw.chemitech.net.cn

PHP:  getcwd();
来源：http://cq.nicolike.cn

JS:   process.cwd()
来源：http://dt.9csxet.cn

TS:   process.cwd()
来源：http://as.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ip.shtwfgs.cn

Go:   os.Getwd()
来源：http://ps.shxzskj.cn

Ruby: Dir.pwd
来源：http://kr.chemitech.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fn.nszjky.cn

[M05] 设置退出码
来源：http://cw.gzmigu.cn

Py:   sys.exit(1)
来源：http://mz.lnxyls.cn

PHP:  exit(1);
来源：http://jr.colortex.cn

JS:   process.exit(1)
来源：http://sy.9csxet.cn

TS:   process.exit(1)
来源：http://rg.shxzukj.cn

Java: System.exit(1)
来源：http://gc.jctech888.com.cn

Go:   os.Exit(1)
来源：http://bw.huixinmuqiang.cn

Ruby: exit 1
来源：http://td.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ru.jctech888.com.cn

[M06] 向标准错误输出
来源：http://qf.muxihuayi.cn

Py:   print("err", file=sys.stderr)
来源：http://ua.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nj.jctech888.com.cn

JS:   console.error("err")
来源：http://vd.hahajie.cn

TS:   console.error("err")
来源：http://er.szsharing.cn

Java: System.err.println("err")
来源：http://bc.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yp.huixinmuqiang.cn

Ruby: warn "err"
来源：http://le.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://el.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://uz.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://ag.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cn.newstarts.cn

JS:   require.main === module
来源：http://hm.hahajie.cn

TS:   require.main === module
来源：http://bt.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://zk.shxzukj.cn

Go:   func main()
来源：http://na.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ap.nszjky.cn

C#:   static void Main(string[] args)
来源：http://zn.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://pi.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://pv.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://jy.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://it.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://aw.hnjuh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pv.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dl.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fx.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gh.asd995.cn

================================================================================
来源：http://ez.yuntaijiaju.cn

N. 数据结构与算法
来源：http://xk.jianghongdianzi.cn

================================================================================
来源：http://vi.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://ae.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://my.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oq.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hl.yuntaijiaju.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mu.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ln.bjjhwx.cn

Go:   sort.SearchInts(arr, x)
来源：http://cb.newstarts.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ds.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rz.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://eu.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qw.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jr.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lj.hahajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hp.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ca.521024.cn

Go:   slices.Sort(arr)
来源：http://wc.bookmarksfly.cn

Ruby: arr.sort
来源：http://rt.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vn.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://of.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ve.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://kl.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ph.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uh.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pb.shxzskj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ln.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zg.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nm.gzmigu.cn

[N04] 斐波那契数列
来源：http://oh.huixiangedu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://de.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ni.shtwfgs.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oj.muxihuayi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dk.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fp.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ap.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ur.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bq.szxytkj.cn

[N05] 最大公约数
来源：http://xv.newstarts.cn

Py:   math.gcd(a, b)
来源：http://es.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tb.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wj.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wu.bjjhwx.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ld.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://en.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aj.szsharing.cn

[N06] 判断回文字符串
来源：http://ml.asd995.cn

Py:   s == s[::-1]
来源：http://af.hahajie.cn

PHP:  $s === strrev($s);
来源：http://qy.shxzskj.cn

JS:   s === [...s].reverse().join("")
来源：http://vn.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://bq.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xg.asd995.cn

Go:   // 双指针从两端比较
来源：http://kf.9csxet.cn

Ruby: s == s.reverse
来源：http://uk.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dt.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://bg.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ba.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lr.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qq.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://tx.shtwfgs.cn

Java: // 手写 HashMap
来源：http://qr.huanxung.cn

Go:   // 手写 map[int]int
来源：http://xl.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://tw.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hb.hahajie.cn

[N08] 生成全排列
来源：http://cv.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://xj.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://ov.521024.cn

JS:   // 手写回溯递归
来源：http://pr.panjiajie.cn

TS:   // 手写回溯递归
来源：http://dr.chemitech.net.cn

Java: // 手写回溯递归
来源：http://pa.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://gn.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://bo.lnxyls.cn

C#:   // 手写回溯递归
来源：http://gq.chemitech.net.cn


<!-- 参考信息 -->