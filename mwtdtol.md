代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pk.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nr.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://cv.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://zs.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xy.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://zr.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sz.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vk.shtwfgs.cn

[K02] JSON 字符串转对象
来源：http://eq.bjjhwx.cn

Py:   json.loads(s)
来源：http://hk.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://du.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://ma.shxzskj.cn

TS:   JSON.parse(s)
来源：http://va.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ek.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://jz.bjjhwx.cn

Ruby: JSON.parse(s)
来源：http://pw.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pv.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://lf.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dt.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dc.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wo.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://is.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zf.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sc.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kj.huanxung.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ka.huanxung.cn

[K04] 读取 JSON 文件
来源：http://nk.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hq.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fh.szsharing.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://da.haigaiapp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dw.newstarts.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pc.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://is.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ur.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fj.szxytkj.cn

[K05] 深拷贝对象
来源：http://sg.colortex.cn

Py:   copy.deepcopy(obj)
来源：http://hy.chemitech.net.cn

PHP:  unserialize(serialize($obj));
来源：http://id.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://ul.bjjhwx.cn

TS:   structuredClone(obj)
来源：http://qv.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bh.huixinmuqiang.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ec.panjiajie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gk.asd995.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ph.shtwfgs.cn

[K06] 解析 URL 查询串
来源：http://uk.shxzukj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ne.colortex.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dy.panjiajie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bn.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jj.shxzukj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ol.shtwfgs.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oj.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ao.asd995.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fx.bjjhwx.cn

[K07] 进制转换
来源：http://ba.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vg.nicolike.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://il.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rs.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zy.colortex.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pn.hnjuh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iz.nszjky.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uz.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yu.yuntaijiaju.cn

[K08] 二进制序列化（非 JSON）
来源：http://iy.yuexingan06.cn

Py:   pickle.dumps(obj)
来源：http://xv.hahajie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gq.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://iq.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://jf.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aw.hnjuh.cn

Go:   encoding/gob
来源：http://bf.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://ek.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ez.wgjwhj.cn

================================================================================
来源：http://yo.hnjuh.cn

L. 网络请求
来源：http://pl.panjiajie.cn

================================================================================
来源：http://ez.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://bn.yuexingan06.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dk.gzmigu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qk.yuexingan06.cn

JS:   await fetch(url)
来源：http://bh.panjiajie.cn

TS:   await fetch(url)
来源：http://xs.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zc.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://cv.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zl.shxzskj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iu.nszjky.cn

[L02] 发送 POST JSON
来源：http://dy.wgjwhj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ne.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ej.hnjuh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qj.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ge.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://da.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ia.bookmarksfly.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fw.jctech888.com.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dq.jctech888.com.cn

[L03] 设置自定义请求头
来源：http://am.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zu.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pd.jianghongdianzi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oo.hnjuh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qd.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ba.chemitech.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wr.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jm.newstarts.cn

[L04] 设置超时
来源：http://bg.hnjuh.cn

Py:   requests.get(url, timeout=5)
来源：http://ih.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rk.521024.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uf.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ky.gzmigu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ke.hnjuh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eu.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xk.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bx.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://ye.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vg.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mw.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dv.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yf.nszjky.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cb.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://it.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://di.shxzukj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rk.9csxet.cn

[L06] 解析响应为 JSON
来源：http://mn.bookmarksfly.cn

Py:   resp.json()
来源：http://cd.hahajie.cn

PHP:  json_decode($body, true);
来源：http://xw.chemitech.net.cn

JS:   await resp.json()
来源：http://pz.jianghongdianzi.cn

TS:   await resp.json()
来源：http://vx.huanxung.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ue.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://va.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://au.colortex.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://di.521024.cn

[L07] 处理 HTTP 状态码
来源：http://id.muxihuayi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jj.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ck.521024.cn

JS:   resp.ok;  resp.status
来源：http://dq.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://ym.bjjhwx.cn

Java: resp.statusCode()
来源：http://bi.jianghongdianzi.cn

Go:   resp.StatusCode
来源：http://bp.asd995.cn

Ruby: resp.code.to_i
来源：http://ca.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://ik.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://os.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bp.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://sz.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bo.chemitech.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jo.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://st.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gm.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tg.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hc.lnxyls.cn

================================================================================
来源：http://xc.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://ip.jianghongdianzi.cn

================================================================================
来源：http://et.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://es.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://kc.colortex.cn

PHP:  $argv;  $argc;
来源：http://ej.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://mo.9csxet.cn

TS:   process.argv.slice(2)
来源：http://eb.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://kp.shxzukj.cn

Go:   os.Args[1:]
来源：http://th.hahajie.cn

Ruby: ARGV
来源：http://ia.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://qw.9csxet.cn

[M02] 读取环境变量
来源：http://zj.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://xm.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xs.bookmarksfly.cn

JS:   process.env.HOME
来源：http://kf.newstarts.cn

TS:   process.env.HOME
来源：http://pg.panjiajie.cn

Java: System.getenv("HOME")
来源：http://lq.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dq.haigaiapp.cn

Ruby: ENV["HOME"]
来源：http://vu.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xw.szsharing.cn

[M03] 执行外部命令
来源：http://og.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ag.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sj.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xf.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qe.haigaiapp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yd.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dt.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xq.jianghongdianzi.cn

C#:   Process.Start("ls", "-l");
来源：http://ha.colortex.cn

[M04] 获取当前工作目录
来源：http://vl.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://yt.9csxet.cn

PHP:  getcwd();
来源：http://zt.nicolike.cn

JS:   process.cwd()
来源：http://dr.szxytkj.cn

TS:   process.cwd()
来源：http://ma.szxytkj.cn

Java: Path.of("").toAbsolutePath()
来源：http://eb.shtwfgs.cn

Go:   os.Getwd()
来源：http://xp.huanxung.cn

Ruby: Dir.pwd
来源：http://lg.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zz.yuexingan06.cn

[M05] 设置退出码
来源：http://di.9csxet.cn

Py:   sys.exit(1)
来源：http://rm.shtwfgs.cn

PHP:  exit(1);
来源：http://sb.nicolike.cn

JS:   process.exit(1)
来源：http://ob.asd995.cn

TS:   process.exit(1)
来源：http://lf.yuntaijiaju.cn

Java: System.exit(1)
来源：http://rk.9csxet.cn

Go:   os.Exit(1)
来源：http://po.yuntaijiaju.cn

Ruby: exit 1
来源：http://mr.gzmigu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mb.colortex.cn

[M06] 向标准错误输出
来源：http://yi.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://sq.szxytkj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cc.huixinmuqiang.cn

JS:   console.error("err")
来源：http://mc.szxytkj.cn

TS:   console.error("err")
来源：http://ax.gzmigu.cn

Java: System.err.println("err")
来源：http://pu.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hq.huixinmuqiang.cn

Ruby: warn "err"
来源：http://as.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://bp.hahajie.cn

[M07] 判断是否为主入口
来源：http://wr.huixiangedu.cn

Py:   if __name__ == "__main__":
来源：http://mr.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pw.panjiajie.cn

JS:   require.main === module
来源：http://ia.bjjhwx.cn

TS:   require.main === module
来源：http://ly.shxzskj.cn

Java: public static void main(String[] args)
来源：http://wg.521024.cn

Go:   func main()
来源：http://wy.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dn.huixiangedu.cn

C#:   static void Main(string[] args)
来源：http://fz.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://ix.yuexingan06.cn

Py:   platform.system();  platform.python_version()
来源：http://bt.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://fc.nicolike.cn

JS:   process.platform;  process.version
来源：http://bn.huanxung.cn

TS:   process.platform;  process.version
来源：http://hc.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cv.wgjwhj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oi.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jo.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qc.gzmigu.cn

================================================================================
来源：http://qd.shtwfgs.cn

N. 数据结构与算法
来源：http://mw.lnxyls.cn

================================================================================
来源：http://nh.huixiangedu.cn

[N01] 二分查找（有序数组）
来源：http://xq.colortex.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qx.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mz.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uo.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rb.yuexingan06.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kp.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://zc.9csxet.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uc.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://td.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://cq.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://pt.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fk.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yt.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gg.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tk.asd995.cn

Go:   slices.Sort(arr)
来源：http://fp.szsharing.cn

Ruby: arr.sort
来源：http://aq.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jc.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://rt.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kb.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://jt.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ky.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oc.bjjhwx.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tk.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hh.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ft.szxytkj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ko.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://lm.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gf.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fw.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://od.yuexingan06.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wj.shtwfgs.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pv.newstarts.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://px.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eo.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xe.huanxung.cn

[N05] 最大公约数
来源：http://ul.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://ym.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://my.9csxet.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ez.bjjhwx.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wp.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uo.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ia.shxzskj.cn

Ruby: a.gcd(b)
来源：http://wu.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oz.nicolike.cn

[N06] 判断回文字符串
来源：http://te.lnxyls.cn

Py:   s == s[::-1]
来源：http://bt.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://lx.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ec.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://lp.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sc.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://ha.panjiajie.cn

Ruby: s == s.reverse
来源：http://js.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ue.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://sm.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iq.bjjhwx.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oc.haigaiapp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rx.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ml.huixiangedu.cn

Java: // 手写 HashMap
来源：http://fx.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://af.panjiajie.cn

Ruby: // 手写 Hash
来源：http://jf.nszjky.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rc.huixiangedu.cn

[N08] 生成全排列
来源：http://vd.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://en.shxzskj.cn

PHP:  // 手写递归交换
来源：http://hh.newstarts.cn

JS:   // 手写回溯递归
来源：http://tk.szsharing.cn

TS:   // 手写回溯递归
来源：http://zo.bjjhwx.cn

Java: // 手写回溯递归
来源：http://tn.szxytkj.cn

Go:   // 手写回溯递归
来源：http://jj.lnxyls.cn

Ruby: arr.permutation.to_a
来源：http://nf.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://gq.huixinmuqiang.cn

[N09] 栈与队列
来源：http://wl.yuexingan06.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pu.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wv.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ve.chemitech.net.cn


<!-- 参考信息 -->