代发 wailian999

================================================================================
来源：http://nu.bjjhwx.cn

K. JSON 与序列化
来源：http://ox.jianghongdianzi.cn

================================================================================
来源：http://mj.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ga.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ku.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yd.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://cg.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://vk.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qc.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://mm.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rq.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xs.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://tn.chemitech.net.cn

Py:   json.loads(s)
来源：http://ct.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dr.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://pu.gzmigu.cn

TS:   JSON.parse(s)
来源：http://da.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://js.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ep.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://zx.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ou.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://rh.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fb.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fa.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mu.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://us.yuntaijiaju.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dt.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://me.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://my.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qo.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://wo.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iq.hnjuh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://su.gzmigu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dv.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rl.521024.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cj.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tz.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kj.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ek.shtwfgs.cn

[K05] 深拷贝对象
来源：http://nr.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://gq.asd995.cn

PHP:  unserialize(serialize($obj));
来源：http://ho.gzmigu.cn

JS:   structuredClone(obj)
来源：http://no.huixiangedu.cn

TS:   structuredClone(obj)
来源：http://fx.muxihuayi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://te.hnjuh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://do.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ro.yuntaijiaju.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xm.wgjwhj.cn

[K06] 解析 URL 查询串
来源：http://kw.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qo.gzmigu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ut.newstarts.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kj.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.wgjwhj.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gx.panjiajie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qr.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bk.newstarts.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jm.szxytkj.cn

[K07] 进制转换
来源：http://gz.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sf.jianghongdianzi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sn.gzmigu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tl.haigaiapp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rn.nszjky.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ap.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ik.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hn.shxzukj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ga.asd995.cn

[K08] 二进制序列化（非 JSON）
来源：http://fq.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://ua.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iz.haigaiapp.cn

JS:   v8.serialize(obj)        // Node
来源：http://zb.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://xu.nszjky.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ck.huixiangedu.cn

Go:   encoding/gob
来源：http://ep.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ux.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cu.hahajie.cn

================================================================================
来源：http://ik.lnxyls.cn

L. 网络请求
来源：http://dq.bjjhwx.cn

================================================================================
来源：http://ih.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://kf.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bm.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hv.chemitech.net.cn

JS:   await fetch(url)
来源：http://tm.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://or.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ic.gzmigu.cn

Go:   resp, err := http.Get(url)
来源：http://qa.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uu.huanxung.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ah.jianghongdianzi.cn

[L02] 发送 POST JSON
来源：http://lb.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yx.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bj.muxihuayi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vf.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vh.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qn.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hf.szxytkj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mk.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zp.hnjuh.cn

[L03] 设置自定义请求头
来源：http://ra.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qq.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wq.colortex.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bs.newstarts.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wq.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tt.szsharing.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vg.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tp.chemitech.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jt.bjjhwx.cn

[L04] 设置超时
来源：http://xf.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://yl.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yv.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zf.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dn.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bl.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mf.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uj.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kn.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://bp.bookmarksfly.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dq.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pz.szsharing.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hl.chemitech.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uq.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zz.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jr.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hr.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mm.huanxung.cn

[L06] 解析响应为 JSON
来源：http://dw.huixinmuqiang.cn

Py:   resp.json()
来源：http://kv.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://oh.bookmarksfly.cn

JS:   await resp.json()
来源：http://xn.colortex.cn

TS:   await resp.json()
来源：http://lg.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uh.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iz.yuexingan06.cn

Ruby: JSON.parse(resp.body)
来源：http://pu.huixinmuqiang.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qi.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://br.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wa.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ll.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://pk.nicolike.cn

TS:   resp.ok;  resp.status
来源：http://uk.nicolike.cn

Java: resp.statusCode()
来源：http://ru.wgjwhj.cn

Go:   resp.StatusCode
来源：http://zq.asd995.cn

Ruby: resp.code.to_i
来源：http://id.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://wp.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://tq.colortex.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pb.shxzukj.cn

PHP:  curl_multi_init() 系列
来源：http://ze.asd995.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tt.szsharing.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qc.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ir.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xu.jctech888.com.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jk.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vi.jctech888.com.cn

================================================================================
来源：http://er.521024.cn

M. 命令行 / 进程 / 环境
来源：http://fj.newstarts.cn

================================================================================
来源：http://az.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://zv.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://xl.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://td.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://gn.panjiajie.cn

TS:   process.argv.slice(2)
来源：http://jt.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://dd.9csxet.cn

Go:   os.Args[1:]
来源：http://wt.nszjky.cn

Ruby: ARGV
来源：http://nu.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://pi.bookmarksfly.cn

[M02] 读取环境变量
来源：http://lw.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://ww.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jh.lnxyls.cn

JS:   process.env.HOME
来源：http://mi.huixiangedu.cn

TS:   process.env.HOME
来源：http://xf.huanxung.cn

Java: System.getenv("HOME")
来源：http://wk.colortex.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hy.bjjhwx.cn

Ruby: ENV["HOME"]
来源：http://ku.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pc.huixiangedu.cn

[M03] 执行外部命令
来源：http://ge.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fr.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ho.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qz.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://li.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zc.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vy.haigaiapp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nt.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://hi.hahajie.cn

[M04] 获取当前工作目录
来源：http://ss.hnjuh.cn

Py:   os.getcwd()
来源：http://gt.jctech888.com.cn

PHP:  getcwd();
来源：http://ix.huixinmuqiang.cn

JS:   process.cwd()
来源：http://de.muxihuayi.cn

TS:   process.cwd()
来源：http://zj.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://om.bookmarksfly.cn

Go:   os.Getwd()
来源：http://hp.asd995.cn

Ruby: Dir.pwd
来源：http://vr.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://du.jianghongdianzi.cn

[M05] 设置退出码
来源：http://gg.muxihuayi.cn

Py:   sys.exit(1)
来源：http://cc.huixiangedu.cn

PHP:  exit(1);
来源：http://kl.lnxyls.cn

JS:   process.exit(1)
来源：http://fi.newstarts.cn

TS:   process.exit(1)
来源：http://xq.lnxyls.cn

Java: System.exit(1)
来源：http://yr.shtwfgs.cn

Go:   os.Exit(1)
来源：http://bt.colortex.cn

Ruby: exit 1
来源：http://cz.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ab.jctech888.com.cn

[M06] 向标准错误输出
来源：http://st.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://xf.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uw.newstarts.cn

JS:   console.error("err")
来源：http://mn.9csxet.cn

TS:   console.error("err")
来源：http://dx.haigaiapp.cn

Java: System.err.println("err")
来源：http://lf.9csxet.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://si.lnxyls.cn

Ruby: warn "err"
来源：http://pi.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://vi.panjiajie.cn

[M07] 判断是否为主入口
来源：http://om.asd995.cn

Py:   if __name__ == "__main__":
来源：http://rb.bookmarksfly.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cq.nicolike.cn

JS:   require.main === module
来源：http://jc.yuntaijiaju.cn

TS:   require.main === module
来源：http://cm.hnjuh.cn

Java: public static void main(String[] args)
来源：http://vq.wgjwhj.cn

Go:   func main()
来源：http://ha.newstarts.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gi.wgjwhj.cn

C#:   static void Main(string[] args)
来源：http://vs.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://tu.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://ah.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ec.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://lu.yuexingan06.cn

TS:   process.platform;  process.version
来源：http://ew.shxzskj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ne.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vx.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ce.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pf.huanxung.cn

================================================================================
来源：http://xr.yuexingan06.cn

N. 数据结构与算法
来源：http://qg.hnjuh.cn

================================================================================
来源：http://wu.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://gr.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bb.yuexingan06.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vr.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jx.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cg.szsharing.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xo.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://bs.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://do.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gj.colortex.cn

[N02] 排序（工程实践用内置实现）
来源：http://lr.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://lu.shxzskj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wi.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sh.panjiajie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lg.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ek.asd995.cn

Go:   slices.Sort(arr)
来源：http://sy.asd995.cn

Ruby: arr.sort
来源：http://su.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vx.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://lt.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bc.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://xa.shxzskj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dj.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wr.9csxet.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ny.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gg.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zq.bjjhwx.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jh.hnjuh.cn

[N04] 斐波那契数列
来源：http://kp.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iu.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sf.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lr.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://og.huanxung.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nd.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pv.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eb.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://al.yuexingan06.cn

[N05] 最大公约数
来源：http://sp.wgjwhj.cn

Py:   math.gcd(a, b)
来源：http://uh.gzmigu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mu.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oe.nszjky.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://as.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ni.hahajie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uo.hahajie.cn

Ruby: a.gcd(b)
来源：http://xx.wgjwhj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xr.asd995.cn

[N06] 判断回文字符串
来源：http://jb.gzmigu.cn

Py:   s == s[::-1]
来源：http://ug.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://rb.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://uz.shxzukj.cn

TS:   s === [...s].reverse().join("")
来源：http://tj.huixiangedu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dp.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://io.lnxyls.cn

Ruby: s == s.reverse
来源：http://hu.wgjwhj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xz.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://ee.shxzskj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qn.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://st.yuntaijiaju.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ow.jctech888.com.cn

TS:   // 手写 Map<string, number>
来源：http://jw.bookmarksfly.cn

Java: // 手写 HashMap
来源：http://le.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://uq.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ho.asd995.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ic.newstarts.cn

[N08] 生成全排列
来源：http://nl.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://bw.huanxung.cn

PHP:  // 手写递归交换
来源：http://rz.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://aa.nicolike.cn

TS:   // 手写回溯递归
来源：http://tb.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://qe.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://hz.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://gu.shxzukj.cn

C#:   // 手写回溯递归
来源：http://xa.bjjhwx.cn


<!-- 参考信息 -->