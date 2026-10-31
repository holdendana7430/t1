代发 wailian999

================================================================================
来源：http://xj.shtwfgs.cn

K. JSON 与序列化
来源：http://so.panjiajie.cn

================================================================================
来源：http://uy.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://ob.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nx.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bd.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://aa.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://so.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oq.newstarts.cn

Go:   json.Marshal(obj)
来源：http://qt.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ny.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fw.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://eb.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://bo.huanxung.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hj.hnjuh.cn

JS:   JSON.parse(s)
来源：http://bn.nicolike.cn

TS:   JSON.parse(s)
来源：http://ci.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wl.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://om.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://lk.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ov.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://yb.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uo.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gz.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kc.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ru.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bk.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://np.shxzskj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ik.asd995.cn

[K04] 读取 JSON 文件
来源：http://eg.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aq.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iz.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vo.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bb.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lh.huixinmuqiang.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jx.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fg.shxzukj.cn

[K05] 深拷贝对象
来源：http://xa.521024.cn

Py:   copy.deepcopy(obj)
来源：http://la.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://zp.shxzukj.cn

JS:   structuredClone(obj)
来源：http://fv.yuntaijiaju.cn

TS:   structuredClone(obj)
来源：http://oy.hahajie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://as.lnxyls.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rg.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zo.jianghongdianzi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dm.bookmarksfly.cn

[K06] 解析 URL 查询串
来源：http://am.haigaiapp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://st.huanxung.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fm.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tb.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zj.colortex.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qy.hnjuh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xi.shtwfgs.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pl.szxytkj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nh.bjjhwx.cn

[K07] 进制转换
来源：http://lo.hnjuh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://do.gzmigu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://di.chemitech.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tw.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ed.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://na.shxzukj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ws.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ls.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://df.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://vm.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nz.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://qp.huixiangedu.cn

TS:   v8.serialize(obj)        // Node
来源：http://np.bjjhwx.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ip.muxihuayi.cn

Go:   encoding/gob
来源：http://dw.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ka.panjiajie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rg.9csxet.cn

================================================================================
来源：http://py.colortex.cn

L. 网络请求
来源：http://iz.shxzskj.cn

================================================================================
来源：http://ql.newstarts.cn

[L01] 发送 GET 请求
来源：http://kj.szxytkj.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jl.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bn.shtwfgs.cn

JS:   await fetch(url)
来源：http://ie.chemitech.net.cn

TS:   await fetch(url)
来源：http://rh.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pk.shxzukj.cn

Go:   resp, err := http.Get(url)
来源：http://nq.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://im.yuntaijiaju.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ss.nszjky.cn

[L02] 发送 POST JSON
来源：http://sf.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pd.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vz.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vv.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ut.muxihuayi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yw.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vz.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eo.haigaiapp.cn

[L03] 设置自定义请求头
来源：http://os.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yw.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tp.newstarts.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dp.shxzskj.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://go.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nf.shtwfgs.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vw.muxihuayi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rg.hahajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wm.hahajie.cn

[L04] 设置超时
来源：http://vc.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://st.521024.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ga.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://js.yuntaijiaju.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ys.huixinmuqiang.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://te.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ag.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qb.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yh.9csxet.cn

[L05] 上传文件（multipart）
来源：http://ve.colortex.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ru.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://po.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zw.bjjhwx.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nj.shtwfgs.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://af.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oz.huanxung.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oy.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ut.haigaiapp.cn

[L06] 解析响应为 JSON
来源：http://mi.521024.cn

Py:   resp.json()
来源：http://bw.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://wk.nicolike.cn

JS:   await resp.json()
来源：http://ai.bjjhwx.cn

TS:   await resp.json()
来源：http://tm.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nu.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nj.muxihuayi.cn

Ruby: JSON.parse(resp.body)
来源：http://bz.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dh.bjjhwx.cn

[L07] 处理 HTTP 状态码
来源：http://ni.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dr.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mk.shtwfgs.cn

JS:   resp.ok;  resp.status
来源：http://cm.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://lz.szxytkj.cn

Java: resp.statusCode()
来源：http://hq.shxzskj.cn

Go:   resp.StatusCode
来源：http://zr.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://ji.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://du.9csxet.cn

[L08] 并发请求多个地址
来源：http://ij.gzmigu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sh.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://ij.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://te.muxihuayi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bx.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uc.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sr.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ot.asd995.cn

================================================================================
来源：http://wd.nicolike.cn

M. 命令行 / 进程 / 环境
来源：http://rw.nicolike.cn

================================================================================
来源：http://so.newstarts.cn

[M01] 读取命令行参数
来源：http://ug.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://ds.newstarts.cn

PHP:  $argv;  $argc;
来源：http://ws.szsharing.cn

JS:   process.argv.slice(2)
来源：http://ik.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://bb.shxzukj.cn

Java: args 数组（main 方法参数）
来源：http://yu.lnxyls.cn

Go:   os.Args[1:]
来源：http://cm.nicolike.cn

Ruby: ARGV
来源：http://da.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://lm.colortex.cn

[M02] 读取环境变量
来源：http://ff.bjjhwx.cn

Py:   os.environ.get("HOME")
来源：http://md.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lc.521024.cn

JS:   process.env.HOME
来源：http://ok.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://oc.huanxung.cn

Java: System.getenv("HOME")
来源：http://gb.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ky.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://wh.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.colortex.cn

[M03] 执行外部命令
来源：http://aa.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fy.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ds.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ad.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rh.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wo.nszjky.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pn.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hf.huanxung.cn

C#:   Process.Start("ls", "-l");
来源：http://cy.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://tv.hnjuh.cn

Py:   os.getcwd()
来源：http://vw.asd995.cn

PHP:  getcwd();
来源：http://zn.huixiangedu.cn

JS:   process.cwd()
来源：http://of.asd995.cn

TS:   process.cwd()
来源：http://ha.asd995.cn

Java: Path.of("").toAbsolutePath()
来源：http://mf.wgjwhj.cn

Go:   os.Getwd()
来源：http://hi.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://tj.huixiangedu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jc.szsharing.cn

[M05] 设置退出码
来源：http://br.haigaiapp.cn

Py:   sys.exit(1)
来源：http://cg.bookmarksfly.cn

PHP:  exit(1);
来源：http://xe.panjiajie.cn

JS:   process.exit(1)
来源：http://pd.jctech888.com.cn

TS:   process.exit(1)
来源：http://zp.chemitech.net.cn

Java: System.exit(1)
来源：http://lc.asd995.cn

Go:   os.Exit(1)
来源：http://dq.bookmarksfly.cn

Ruby: exit 1
来源：http://db.521024.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dr.hahajie.cn

[M06] 向标准错误输出
来源：http://jo.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://zq.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kc.shxzskj.cn

JS:   console.error("err")
来源：http://hn.lnxyls.cn

TS:   console.error("err")
来源：http://xx.hahajie.cn

Java: System.err.println("err")
来源：http://kf.szxytkj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hn.szxytkj.cn

Ruby: warn "err"
来源：http://qe.muxihuayi.cn

C#:   Console.Error.WriteLine("err")
来源：http://op.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://cp.bookmarksfly.cn

Py:   if __name__ == "__main__":
来源：http://wq.wgjwhj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zi.jianghongdianzi.cn

JS:   require.main === module
来源：http://go.newstarts.cn

TS:   require.main === module
来源：http://xg.colortex.cn

Java: public static void main(String[] args)
来源：http://mp.shxzskj.cn

Go:   func main()
来源：http://os.szsharing.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://as.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://dl.521024.cn

[M08] 获取系统与运行时信息
来源：http://ok.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://uh.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://xq.colortex.cn

JS:   process.platform;  process.version
来源：http://ph.shtwfgs.cn

TS:   process.platform;  process.version
来源：http://fw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bf.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xe.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dm.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bi.jianghongdianzi.cn

================================================================================
来源：http://vr.colortex.cn

N. 数据结构与算法
来源：http://sk.shxzukj.cn

================================================================================
来源：http://mc.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://zd.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pl.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aj.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qg.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pv.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xt.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://nw.szsharing.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dr.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bt.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://zo.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://cg.panjiajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mj.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zz.hnjuh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://za.colortex.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vi.shxzukj.cn

Go:   slices.Sort(arr)
来源：http://jv.huixiangedu.cn

Ruby: arr.sort
来源：http://yw.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bt.521024.cn

[N03] 快速排序（分治示例）
来源：http://go.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yk.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://zi.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mm.521024.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ar.chemitech.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yr.hnjuh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gn.nicolike.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qg.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dc.hnjuh.cn

[N04] 斐波那契数列
来源：http://bd.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zh.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ss.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oq.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qs.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qs.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sy.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uc.nszjky.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zl.szsharing.cn

[N05] 最大公约数
来源：http://qp.huanxung.cn

Py:   math.gcd(a, b)
来源：http://vf.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gz.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vv.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mz.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lh.shxzskj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oq.panjiajie.cn

Ruby: a.gcd(b)
来源：http://ty.521024.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fj.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://eq.asd995.cn

Py:   s == s[::-1]
来源：http://zw.9csxet.cn

PHP:  $s === strrev($s);
来源：http://ot.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://sj.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://gg.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hs.nszjky.cn

Go:   // 双指针从两端比较
来源：http://eb.szsharing.cn

Ruby: s == s.reverse
来源：http://ia.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mf.jctech888.com.cn

[N07] 两数之和（返回下标）
来源：http://fp.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rp.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fb.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pd.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://dm.gzmigu.cn

Java: // 手写 HashMap
来源：http://ro.lnxyls.cn

Go:   // 手写 map[int]int
来源：http://vb.yuexingan06.cn

Ruby: // 手写 Hash
来源：http://gu.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zw.panjiajie.cn

[N08] 生成全排列
来源：http://zc.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://ix.asd995.cn

PHP:  // 手写递归交换
来源：http://sd.newstarts.cn

JS:   // 手写回溯递归
来源：http://uv.shxzukj.cn

TS:   // 手写回溯递归
来源：http://wc.shxzskj.cn

Java: // 手写回溯递归
来源：http://ju.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://kk.huanxung.cn

Ruby: arr.permutation.to_a
来源：http://ji.nszjky.cn

C#:   // 手写回溯递归
来源：http://bp.muxihuayi.cn


<!-- 参考信息 -->