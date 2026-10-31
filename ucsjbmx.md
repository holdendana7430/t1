代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qy.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rm.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://pm.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://hk.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vv.newstarts.cn

Go:   json.Marshal(obj)
来源：http://hr.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lq.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nt.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://hv.szsharing.cn

Py:   json.loads(s)
来源：http://ms.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pa.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://zn.asd995.cn

TS:   JSON.parse(s)
来源：http://ri.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ql.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://hb.szsharing.cn

Ruby: JSON.parse(s)
来源：http://dr.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mj.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://rm.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zs.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bn.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fy.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://co.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rd.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iz.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sr.szsharing.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zq.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://zl.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dj.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mk.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ub.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rk.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gb.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pn.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rg.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sb.haigaiapp.cn

[K05] 深拷贝对象
来源：http://kx.asd995.cn

Py:   copy.deepcopy(obj)
来源：http://mx.lnxyls.cn

PHP:  unserialize(serialize($obj));
来源：http://vx.hahajie.cn

JS:   structuredClone(obj)
来源：http://jo.yuexingan06.cn

TS:   structuredClone(obj)
来源：http://wj.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ho.szxytkj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sg.newstarts.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zu.huanxung.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ee.shxzukj.cn

[K06] 解析 URL 查询串
来源：http://sv.hahajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pn.jianghongdianzi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sv.bookmarksfly.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vd.shxzskj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ve.szsharing.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ts.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gf.szsharing.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mj.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tb.newstarts.cn

[K07] 进制转换
来源：http://lv.haigaiapp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ut.huixinmuqiang.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tt.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ol.nszjky.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ai.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iz.asd995.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lp.hahajie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fw.jctech888.com.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dr.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pp.szsharing.cn

Py:   pickle.dumps(obj)
来源：http://cf.shxzskj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://te.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://eq.nicolike.cn

TS:   v8.serialize(obj)        // Node
来源：http://mt.huixinmuqiang.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wp.hnjuh.cn

Go:   encoding/gob
来源：http://ie.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://xh.lnxyls.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zi.jctech888.com.cn

================================================================================
来源：http://lr.shtwfgs.cn

L. 网络请求
来源：http://uv.jianghongdianzi.cn

================================================================================
来源：http://lr.yuexingan06.cn

[L01] 发送 GET 请求
来源：http://vz.muxihuayi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zn.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sh.panjiajie.cn

JS:   await fetch(url)
来源：http://yo.bjjhwx.cn

TS:   await fetch(url)
来源：http://za.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vq.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://as.chemitech.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cw.asd995.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fd.shtwfgs.cn

[L02] 发送 POST JSON
来源：http://le.shxzukj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hl.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://km.nszjky.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dc.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ky.chemitech.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ss.chemitech.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sr.huixinmuqiang.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xf.szsharing.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ib.huanxung.cn

[L03] 设置自定义请求头
来源：http://gz.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lx.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hx.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sv.wgjwhj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jw.shtwfgs.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yr.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xd.521024.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uk.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lf.lnxyls.cn

[L04] 设置超时
来源：http://aj.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://mm.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hg.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ef.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://az.szsharing.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fd.yuexingan06.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ks.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kd.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cs.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://pa.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gz.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hq.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uq.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lh.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aw.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wr.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gd.bookmarksfly.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fl.521024.cn

[L06] 解析响应为 JSON
来源：http://ul.jctech888.com.cn

Py:   resp.json()
来源：http://cj.szxytkj.cn

PHP:  json_decode($body, true);
来源：http://jt.wgjwhj.cn

JS:   await resp.json()
来源：http://jy.szxytkj.cn

TS:   await resp.json()
来源：http://mk.szsharing.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pc.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://br.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://qs.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oc.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://ep.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bw.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://je.yuexingan06.cn

JS:   resp.ok;  resp.status
来源：http://sm.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://bo.colortex.cn

Java: resp.statusCode()
来源：http://no.wgjwhj.cn

Go:   resp.StatusCode
来源：http://fc.lnxyls.cn

Ruby: resp.code.to_i
来源：http://ds.colortex.cn

C#:   (int)resp.StatusCode
来源：http://br.nszjky.cn

[L08] 并发请求多个地址
来源：http://xg.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lm.huixiangedu.cn

PHP:  curl_multi_init() 系列
来源：http://de.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://st.asd995.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tv.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sv.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mk.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://al.szxytkj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tl.yuexingan06.cn

================================================================================
来源：http://ei.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://ow.nszjky.cn

================================================================================
来源：http://cb.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://ej.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://km.521024.cn

PHP:  $argv;  $argc;
来源：http://ti.hnjuh.cn

JS:   process.argv.slice(2)
来源：http://qj.jianghongdianzi.cn

TS:   process.argv.slice(2)
来源：http://nj.nicolike.cn

Java: args 数组（main 方法参数）
来源：http://or.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ih.bookmarksfly.cn

Ruby: ARGV
来源：http://fr.huixiangedu.cn

C#:   args 数组（Main 方法参数）
来源：http://he.nicolike.cn

[M02] 读取环境变量
来源：http://tv.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://ep.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sk.hahajie.cn

JS:   process.env.HOME
来源：http://ti.shtwfgs.cn

TS:   process.env.HOME
来源：http://wy.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://mn.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ed.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://ig.yuexingan06.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://at.wgjwhj.cn

[M03] 执行外部命令
来源：http://if.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zn.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ix.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qp.huixiangedu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ps.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oc.muxihuayi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://su.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vs.bjjhwx.cn

C#:   Process.Start("ls", "-l");
来源：http://al.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://wi.nicolike.cn

Py:   os.getcwd()
来源：http://ey.wgjwhj.cn

PHP:  getcwd();
来源：http://yb.bjjhwx.cn

JS:   process.cwd()
来源：http://ts.shxzskj.cn

TS:   process.cwd()
来源：http://yn.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://db.szxytkj.cn

Go:   os.Getwd()
来源：http://pw.yuexingan06.cn

Ruby: Dir.pwd
来源：http://ki.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ye.hahajie.cn

[M05] 设置退出码
来源：http://da.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://jw.bookmarksfly.cn

PHP:  exit(1);
来源：http://cg.panjiajie.cn

JS:   process.exit(1)
来源：http://ct.nicolike.cn

TS:   process.exit(1)
来源：http://vt.9csxet.cn

Java: System.exit(1)
来源：http://fn.huixiangedu.cn

Go:   os.Exit(1)
来源：http://jg.szsharing.cn

Ruby: exit 1
来源：http://co.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qc.szsharing.cn

[M06] 向标准错误输出
来源：http://we.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://rg.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dt.yuntaijiaju.cn

JS:   console.error("err")
来源：http://hi.shtwfgs.cn

TS:   console.error("err")
来源：http://ku.muxihuayi.cn

Java: System.err.println("err")
来源：http://xt.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jk.nicolike.cn

Ruby: warn "err"
来源：http://jr.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://dz.shxzukj.cn

[M07] 判断是否为主入口
来源：http://tz.jianghongdianzi.cn

Py:   if __name__ == "__main__":
来源：http://yz.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.muxihuayi.cn

JS:   require.main === module
来源：http://ik.nszjky.cn

TS:   require.main === module
来源：http://uj.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://jj.szxytkj.cn

Go:   func main()
来源：http://tp.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lx.huanxung.cn

C#:   static void Main(string[] args)
来源：http://dq.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://uj.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://qm.newstarts.cn

PHP:  PHP_OS;  phpversion();
来源：http://nh.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://hy.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://vg.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lf.szxytkj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zw.jctech888.com.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hj.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iw.asd995.cn

================================================================================
来源：http://jm.huixiangedu.cn

N. 数据结构与算法
来源：http://ty.wgjwhj.cn

================================================================================
来源：http://ly.muxihuayi.cn

[N01] 二分查找（有序数组）
来源：http://rp.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fd.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lq.szsharing.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ah.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wc.asd995.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ev.jctech888.com.cn

Go:   sort.SearchInts(arr, x)
来源：http://xh.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dj.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sn.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://qd.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://gn.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dc.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zq.colortex.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vf.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fm.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://ap.szsharing.cn

Ruby: arr.sort
来源：http://wv.huixinmuqiang.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uw.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://xz.panjiajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ix.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://vv.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cp.nicolike.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ul.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dl.muxihuayi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qi.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jh.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dd.521024.cn

[N04] 斐波那契数列
来源：http://bf.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jc.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rv.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yr.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fv.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fz.huanxung.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bm.hahajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mp.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bs.huixinmuqiang.cn

[N05] 最大公约数
来源：http://gg.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ai.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tf.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://es.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ue.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ne.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yc.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://ch.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ly.nszjky.cn

[N06] 判断回文字符串
来源：http://sz.gzmigu.cn

Py:   s == s[::-1]
来源：http://hy.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://js.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://xb.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://tu.gzmigu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vt.newstarts.cn

Go:   // 双指针从两端比较
来源：http://ih.huanxung.cn

Ruby: s == s.reverse
来源：http://ge.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wg.521024.cn

[N07] 两数之和（返回下标）
来源：http://dm.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qv.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://es.yuexingan06.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jl.jianghongdianzi.cn

TS:   // 手写 Map<string, number>
来源：http://qc.colortex.cn

Java: // 手写 HashMap
来源：http://eb.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://yz.newstarts.cn

Ruby: // 手写 Hash
来源：http://as.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kb.shtwfgs.cn

[N08] 生成全排列
来源：http://zc.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://le.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://ou.szsharing.cn

JS:   // 手写回溯递归
来源：http://ih.chemitech.net.cn

TS:   // 手写回溯递归
来源：http://fa.hahajie.cn

Java: // 手写回溯递归
来源：http://rq.huanxung.cn

Go:   // 手写回溯递归
来源：http://ez.colortex.cn

Ruby: arr.permutation.to_a
来源：http://wn.huanxung.cn

C#:   // 手写回溯递归
来源：http://bd.huanxung.cn

[N09] 栈与队列
来源：http://rv.haigaiapp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ko.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zb.panjiajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ip.huixiangedu.cn


<!-- 参考信息 -->