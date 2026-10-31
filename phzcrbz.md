代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qt.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vb.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wo.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zz.huixinmuqiang.cn

================================================================================
来源：http://cq.yuexingan06.cn

K. JSON 与序列化
来源：http://aa.hnjuh.cn

================================================================================
来源：http://qi.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://hb.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rm.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rt.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://cp.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://dm.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xz.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://ls.huixiangedu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ec.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kb.szsharing.cn

[K02] JSON 字符串转对象
来源：http://xt.bjjhwx.cn

Py:   json.loads(s)
来源：http://ty.haigaiapp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jd.lnxyls.cn

JS:   JSON.parse(s)
来源：http://oa.nicolike.cn

TS:   JSON.parse(s)
来源：http://oa.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hv.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://va.wgjwhj.cn

Ruby: JSON.parse(s)
来源：http://dw.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oj.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://xw.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xu.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ei.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nc.jctech888.com.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uv.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yd.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://et.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cu.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tl.newstarts.cn

[K04] 读取 JSON 文件
来源：http://xj.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://in.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ht.shtwfgs.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tl.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rs.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pe.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ng.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sl.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://np.muxihuayi.cn

[K05] 深拷贝对象
来源：http://nr.szxytkj.cn

Py:   copy.deepcopy(obj)
来源：http://uh.newstarts.cn

PHP:  unserialize(serialize($obj));
来源：http://wl.muxihuayi.cn

JS:   structuredClone(obj)
来源：http://wf.huanxung.cn

TS:   structuredClone(obj)
来源：http://qe.hnjuh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dz.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mn.9csxet.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ak.bookmarksfly.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://er.szxytkj.cn

[K06] 解析 URL 查询串
来源：http://eg.wgjwhj.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tp.hnjuh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ar.jianghongdianzi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://id.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mw.nszjky.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uw.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ip.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pl.szsharing.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ox.wgjwhj.cn

[K07] 进制转换
来源：http://qb.szxytkj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pb.jctech888.com.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fk.huixiangedu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bk.lnxyls.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xf.521024.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://js.muxihuayi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jx.shxzskj.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ko.newstarts.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pz.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://yc.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://cw.asd995.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ev.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://cb.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://rs.wgjwhj.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zn.hnjuh.cn

Go:   encoding/gob
来源：http://vj.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://vf.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cs.asd995.cn

================================================================================
来源：http://al.nicolike.cn

L. 网络请求
来源：http://ce.bookmarksfly.cn

================================================================================
来源：http://fs.gzmigu.cn

[L01] 发送 GET 请求
来源：http://wy.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vg.yuexingan06.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jl.huanxung.cn

JS:   await fetch(url)
来源：http://jk.huixiangedu.cn

TS:   await fetch(url)
来源：http://ce.shtwfgs.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://je.newstarts.cn

Go:   resp, err := http.Get(url)
来源：http://mp.colortex.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lm.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mw.gzmigu.cn

[L02] 发送 POST JSON
来源：http://yq.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tk.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nx.huanxung.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yq.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fd.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lz.asd995.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oj.jianghongdianzi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kt.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hx.shxzukj.cn

[L03] 设置自定义请求头
来源：http://wh.yuexingan06.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://va.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qm.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vh.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dd.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cz.nszjky.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://un.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xg.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ef.szxytkj.cn

[L04] 设置超时
来源：http://uk.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://as.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rq.jctech888.com.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bv.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oc.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xo.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vz.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mk.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fm.9csxet.cn

[L05] 上传文件（multipart）
来源：http://vs.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yg.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://im.521024.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rm.huixiangedu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cg.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ry.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fy.jctech888.com.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yn.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lq.asd995.cn

[L06] 解析响应为 JSON
来源：http://ke.jctech888.com.cn

Py:   resp.json()
来源：http://qg.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://qg.asd995.cn

JS:   await resp.json()
来源：http://lv.bookmarksfly.cn

TS:   await resp.json()
来源：http://ay.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dv.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dt.shxzukj.cn

Ruby: JSON.parse(resp.body)
来源：http://zq.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sn.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://cn.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xu.shxzskj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://st.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://yv.asd995.cn

TS:   resp.ok;  resp.status
来源：http://jh.jctech888.com.cn

Java: resp.statusCode()
来源：http://yy.wgjwhj.cn

Go:   resp.StatusCode
来源：http://mr.gzmigu.cn

Ruby: resp.code.to_i
来源：http://ok.521024.cn

C#:   (int)resp.StatusCode
来源：http://la.jctech888.com.cn

[L08] 并发请求多个地址
来源：http://jr.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mj.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://oj.newstarts.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xs.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sh.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gx.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://md.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vj.huixiangedu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ae.bjjhwx.cn

================================================================================
来源：http://il.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://dg.haigaiapp.cn

================================================================================
来源：http://il.haigaiapp.cn

[M01] 读取命令行参数
来源：http://gm.9csxet.cn

Py:   sys.argv[1:]
来源：http://jd.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://oo.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://um.asd995.cn

TS:   process.argv.slice(2)
来源：http://cg.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://eq.huixinmuqiang.cn

Go:   os.Args[1:]
来源：http://zr.yuexingan06.cn

Ruby: ARGV
来源：http://ak.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://fn.nszjky.cn

[M02] 读取环境变量
来源：http://vi.wgjwhj.cn

Py:   os.environ.get("HOME")
来源：http://iv.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yd.muxihuayi.cn

JS:   process.env.HOME
来源：http://pd.yuexingan06.cn

TS:   process.env.HOME
来源：http://tw.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://ln.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qa.hahajie.cn

Ruby: ENV["HOME"]
来源：http://uo.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tc.muxihuayi.cn

[M03] 执行外部命令
来源：http://yp.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xk.muxihuayi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qy.yuexingan06.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zo.nszjky.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vc.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qg.huixinmuqiang.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eo.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dm.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.gzmigu.cn

[M04] 获取当前工作目录
来源：http://kj.huanxung.cn

Py:   os.getcwd()
来源：http://if.jianghongdianzi.cn

PHP:  getcwd();
来源：http://qp.nszjky.cn

JS:   process.cwd()
来源：http://hn.nszjky.cn

TS:   process.cwd()
来源：http://kk.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://yi.gzmigu.cn

Go:   os.Getwd()
来源：http://hy.huixinmuqiang.cn

Ruby: Dir.pwd
来源：http://jv.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jn.hnjuh.cn

[M05] 设置退出码
来源：http://py.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://fp.newstarts.cn

PHP:  exit(1);
来源：http://rl.huixiangedu.cn

JS:   process.exit(1)
来源：http://fa.lnxyls.cn

TS:   process.exit(1)
来源：http://cc.hnjuh.cn

Java: System.exit(1)
来源：http://zw.nszjky.cn

Go:   os.Exit(1)
来源：http://ai.jctech888.com.cn

Ruby: exit 1
来源：http://ec.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://it.shtwfgs.cn

[M06] 向标准错误输出
来源：http://cm.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://kz.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vm.bjjhwx.cn

JS:   console.error("err")
来源：http://pg.huixinmuqiang.cn

TS:   console.error("err")
来源：http://sr.haigaiapp.cn

Java: System.err.println("err")
来源：http://zz.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iz.huixinmuqiang.cn

Ruby: warn "err"
来源：http://gp.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://wy.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://lj.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://zi.chemitech.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xy.521024.cn

JS:   require.main === module
来源：http://wm.muxihuayi.cn

TS:   require.main === module
来源：http://xj.panjiajie.cn

Java: public static void main(String[] args)
来源：http://nq.muxihuayi.cn

Go:   func main()
来源：http://ok.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ua.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://rn.jctech888.com.cn

[M08] 获取系统与运行时信息
来源：http://fy.muxihuayi.cn

Py:   platform.system();  platform.python_version()
来源：http://sx.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ms.huanxung.cn

JS:   process.platform;  process.version
来源：http://gi.wgjwhj.cn

TS:   process.platform;  process.version
来源：http://nv.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sr.colortex.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nv.shxzukj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gl.wgjwhj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://av.shxzskj.cn

================================================================================
来源：http://tg.nicolike.cn

N. 数据结构与算法
来源：http://fx.newstarts.cn

================================================================================
来源：http://er.shxzukj.cn

[N01] 二分查找（有序数组）
来源：http://fm.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sv.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uh.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ns.9csxet.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eh.shtwfgs.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fw.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://tw.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cc.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ds.nszjky.cn

[N02] 排序（工程实践用内置实现）
来源：http://mi.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://bc.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uv.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tv.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dn.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ta.yuexingan06.cn

Go:   slices.Sort(arr)
来源：http://ek.wgjwhj.cn

Ruby: arr.sort
来源：http://zf.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zd.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://km.9csxet.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://et.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://ud.chemitech.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ik.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dh.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xr.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wh.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ut.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pn.shxzukj.cn

[N04] 斐波那契数列
来源：http://qa.chemitech.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uv.shtwfgs.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://go.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gl.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://en.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ky.muxihuayi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://la.bookmarksfly.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rg.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ds.shxzukj.cn

[N05] 最大公约数
来源：http://jh.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://zj.szxytkj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ah.haigaiapp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://al.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bx.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vj.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uz.hnjuh.cn

Ruby: a.gcd(b)
来源：http://ys.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dp.newstarts.cn

[N06] 判断回文字符串
来源：http://se.haigaiapp.cn

Py:   s == s[::-1]
来源：http://zr.newstarts.cn

PHP:  $s === strrev($s);
来源：http://pq.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://yk.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://nr.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mb.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://ms.szxytkj.cn

Ruby: s == s.reverse
来源：http://lu.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fl.szxytkj.cn

[N07] 两数之和（返回下标）
来源：http://ji.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lg.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lz.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oy.bookmarksfly.cn

TS:   // 手写 Map<string, number>
来源：http://zq.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://ig.shxzukj.cn

Go:   // 手写 map[int]int
来源：http://xq.jianghongdianzi.cn

Ruby: // 手写 Hash
来源：http://fw.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pw.asd995.cn

[N08] 生成全排列
来源：http://al.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://di.hnjuh.cn

PHP:  // 手写递归交换
来源：http://we.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://ib.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://vy.shxzukj.cn


<!-- 参考信息 -->