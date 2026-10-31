代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ue.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://da.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://bs.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yi.9csxet.cn

Go:   json.Marshal(obj)
来源：http://xk.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yc.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jh.hahajie.cn

[K02] JSON 字符串转对象
来源：http://nf.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ry.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://er.lnxyls.cn

JS:   JSON.parse(s)
来源：http://ij.muxihuayi.cn

TS:   JSON.parse(s)
来源：http://ia.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ad.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://hv.huanxung.cn

Ruby: JSON.parse(s)
来源：http://rp.asd995.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://da.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://vp.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xm.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ia.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vq.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dm.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xw.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ft.muxihuayi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jb.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mp.521024.cn

[K04] 读取 JSON 文件
来源：http://fk.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qo.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://al.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ut.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hb.huixinmuqiang.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cs.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oz.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://on.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wt.huanxung.cn

[K05] 深拷贝对象
来源：http://jb.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://bf.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://xc.nicolike.cn

JS:   structuredClone(obj)
来源：http://pc.lnxyls.cn

TS:   structuredClone(obj)
来源：http://qh.nicolike.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pk.bookmarksfly.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://os.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://za.9csxet.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rj.haigaiapp.cn

[K06] 解析 URL 查询串
来源：http://es.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xp.521024.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nh.huixinmuqiang.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ez.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fq.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ed.9csxet.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lr.huixinmuqiang.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gb.huixinmuqiang.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fs.muxihuayi.cn

[K07] 进制转换
来源：http://zh.bookmarksfly.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bn.panjiajie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ee.szsharing.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ba.shtwfgs.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uw.hnjuh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qm.panjiajie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zm.szsharing.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yw.colortex.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ar.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://xf.colortex.cn

Py:   pickle.dumps(obj)
来源：http://ww.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nn.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://ee.asd995.cn

TS:   v8.serialize(obj)        // Node
来源：http://co.shxzskj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vl.521024.cn

Go:   encoding/gob
来源：http://di.huixiangedu.cn

Ruby: Marshal.dump(obj)
来源：http://of.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bb.hnjuh.cn

================================================================================
来源：http://yb.colortex.cn

L. 网络请求
来源：http://rf.shxzskj.cn

================================================================================
来源：http://pa.jianghongdianzi.cn

[L01] 发送 GET 请求
来源：http://xk.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jr.521024.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://is.asd995.cn

JS:   await fetch(url)
来源：http://ik.asd995.cn

TS:   await fetch(url)
来源：http://xg.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pp.szxytkj.cn

Go:   resp, err := http.Get(url)
来源：http://ro.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rf.bookmarksfly.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xu.521024.cn

[L02] 发送 POST JSON
来源：http://vn.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fq.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://au.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dk.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gu.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ds.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ye.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yg.521024.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lu.muxihuayi.cn

[L03] 设置自定义请求头
来源：http://ab.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xb.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://al.asd995.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aq.nszjky.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://np.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cp.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iu.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://st.hnjuh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://un.szsharing.cn

[L04] 设置超时
来源：http://kr.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://qm.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rh.yuexingan06.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://il.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jw.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ne.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ve.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fc.bjjhwx.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tq.shxzskj.cn

[L05] 上传文件（multipart）
来源：http://wb.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qf.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oc.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wz.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oa.huanxung.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uv.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://is.nicolike.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://do.nszjky.cn

[L06] 解析响应为 JSON
来源：http://yf.hnjuh.cn

Py:   resp.json()
来源：http://he.521024.cn

PHP:  json_decode($body, true);
来源：http://uo.panjiajie.cn

JS:   await resp.json()
来源：http://ul.521024.cn

TS:   await resp.json()
来源：http://kx.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hu.hahajie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hc.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://mi.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gj.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://zf.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ep.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://da.huixinmuqiang.cn

JS:   resp.ok;  resp.status
来源：http://qy.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ry.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://mz.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://aa.newstarts.cn

Ruby: resp.code.to_i
来源：http://zi.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://ht.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://vk.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gz.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://np.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://de.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jc.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jn.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://as.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iu.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cb.szxytkj.cn

================================================================================
来源：http://ne.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://yi.hnjuh.cn

================================================================================
来源：http://lv.huixiangedu.cn

[M01] 读取命令行参数
来源：http://gd.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://wu.hnjuh.cn

PHP:  $argv;  $argc;
来源：http://fw.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://bf.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://an.asd995.cn

Java: args 数组（main 方法参数）
来源：http://nn.colortex.cn

Go:   os.Args[1:]
来源：http://nb.nszjky.cn

Ruby: ARGV
来源：http://md.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://tb.shxzukj.cn

[M02] 读取环境变量
来源：http://ii.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://pj.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rj.szxytkj.cn

JS:   process.env.HOME
来源：http://lz.panjiajie.cn

TS:   process.env.HOME
来源：http://yt.lnxyls.cn

Java: System.getenv("HOME")
来源：http://pn.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rs.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ff.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ni.wgjwhj.cn

[M03] 执行外部命令
来源：http://pp.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ik.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ar.gzmigu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hb.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fo.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xk.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nx.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kf.jctech888.com.cn

C#:   Process.Start("ls", "-l");
来源：http://sw.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://gn.huixiangedu.cn

Py:   os.getcwd()
来源：http://zq.jctech888.com.cn

PHP:  getcwd();
来源：http://yy.wgjwhj.cn

JS:   process.cwd()
来源：http://bt.shtwfgs.cn

TS:   process.cwd()
来源：http://bv.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://tw.shxzskj.cn

Go:   os.Getwd()
来源：http://bi.jctech888.com.cn

Ruby: Dir.pwd
来源：http://zd.shxzskj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pa.nicolike.cn

[M05] 设置退出码
来源：http://qo.9csxet.cn

Py:   sys.exit(1)
来源：http://mf.jctech888.com.cn

PHP:  exit(1);
来源：http://jd.jctech888.com.cn

JS:   process.exit(1)
来源：http://kn.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://wj.yuntaijiaju.cn

Java: System.exit(1)
来源：http://tg.jctech888.com.cn

Go:   os.Exit(1)
来源：http://sf.huixinmuqiang.cn

Ruby: exit 1
来源：http://vh.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://km.bookmarksfly.cn

[M06] 向标准错误输出
来源：http://rn.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://zx.huixinmuqiang.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://py.wgjwhj.cn

JS:   console.error("err")
来源：http://uc.nicolike.cn

TS:   console.error("err")
来源：http://dw.9csxet.cn

Java: System.err.println("err")
来源：http://ci.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wk.9csxet.cn

Ruby: warn "err"
来源：http://if.yuexingan06.cn

C#:   Console.Error.WriteLine("err")
来源：http://hv.asd995.cn

[M07] 判断是否为主入口
来源：http://fj.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://sp.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wo.colortex.cn

JS:   require.main === module
来源：http://re.huixinmuqiang.cn

TS:   require.main === module
来源：http://of.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://cc.9csxet.cn

Go:   func main()
来源：http://aw.jianghongdianzi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rd.colortex.cn

C#:   static void Main(string[] args)
来源：http://od.lnxyls.cn

[M08] 获取系统与运行时信息
来源：http://yi.huixiangedu.cn

Py:   platform.system();  platform.python_version()
来源：http://qi.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://nn.shxzskj.cn

JS:   process.platform;  process.version
来源：http://le.lnxyls.cn

TS:   process.platform;  process.version
来源：http://sq.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mu.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vj.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fg.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tw.jctech888.com.cn

================================================================================
来源：http://zh.haigaiapp.cn

N. 数据结构与算法
来源：http://ic.jianghongdianzi.cn

================================================================================
来源：http://op.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://di.huanxung.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uc.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pw.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yr.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sa.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fq.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://zl.yuexingan06.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yv.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jp.panjiajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://qc.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://fu.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vw.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xs.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mr.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pt.huanxung.cn

Go:   slices.Sort(arr)
来源：http://ef.shtwfgs.cn

Ruby: arr.sort
来源：http://vp.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ix.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://xj.hnjuh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kg.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://ou.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kv.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zm.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xk.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qv.yuexingan06.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dk.szsharing.cn

C#:   // 手写递归，或 Array.Sort
来源：http://on.yuexingan06.cn

[N04] 斐波那契数列
来源：http://go.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jm.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sk.bookmarksfly.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ld.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ic.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wy.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zu.nicolike.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ns.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hd.bjjhwx.cn

[N05] 最大公约数
来源：http://kb.yuexingan06.cn

Py:   math.gcd(a, b)
来源：http://ef.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ta.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jq.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://su.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jr.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://px.521024.cn

Ruby: a.gcd(b)
来源：http://qj.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://su.colortex.cn

[N06] 判断回文字符串
来源：http://em.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://vn.huanxung.cn

PHP:  $s === strrev($s);
来源：http://vc.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://um.jctech888.com.cn

TS:   s === [...s].reverse().join("")
来源：http://oc.9csxet.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nf.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://xc.colortex.cn

Ruby: s == s.reverse
来源：http://ux.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mj.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://qu.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xs.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zp.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yw.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://di.521024.cn

Java: // 手写 HashMap
来源：http://ir.colortex.cn

Go:   // 手写 map[int]int
来源：http://xd.asd995.cn

Ruby: // 手写 Hash
来源：http://cz.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rf.chemitech.net.cn

[N08] 生成全排列
来源：http://ql.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://uy.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://pe.hahajie.cn

JS:   // 手写回溯递归
来源：http://yq.nszjky.cn

TS:   // 手写回溯递归
来源：http://rf.szsharing.cn

Java: // 手写回溯递归
来源：http://qs.shtwfgs.cn

Go:   // 手写回溯递归
来源：http://uf.yuexingan06.cn

Ruby: arr.permutation.to_a
来源：http://qx.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://pm.haigaiapp.cn

[N09] 栈与队列
来源：http://uc.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sn.jianghongdianzi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uk.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oq.yuntaijiaju.cn


<!-- 参考信息 -->