代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qg.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fa.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ln.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ys.haigaiapp.cn

================================================================================
来源：http://un.jctech888.com.cn

K. JSON 与序列化
来源：http://ix.jianghongdianzi.cn

================================================================================
来源：http://rl.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://la.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dw.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vo.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://rr.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://wx.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ns.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ep.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yw.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jg.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://pn.muxihuayi.cn

Py:   json.loads(s)
来源：http://gk.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tw.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ak.colortex.cn

TS:   JSON.parse(s)
来源：http://wg.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cr.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://rl.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://nz.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://st.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yu.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uj.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bp.bjjhwx.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yx.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wn.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gk.521024.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ba.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ew.yuntaijiaju.cn

[K04] 读取 JSON 文件
来源：http://rg.lnxyls.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wd.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ub.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qu.shtwfgs.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gd.hahajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vu.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jk.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cl.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hw.muxihuayi.cn

[K05] 深拷贝对象
来源：http://nn.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://lv.nicolike.cn

PHP:  unserialize(serialize($obj));
来源：http://gk.nszjky.cn

JS:   structuredClone(obj)
来源：http://ia.jctech888.com.cn

TS:   structuredClone(obj)
来源：http://hv.bjjhwx.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jf.yuexingan06.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ww.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gz.szsharing.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ch.lnxyls.cn

[K06] 解析 URL 查询串
来源：http://jf.chemitech.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dt.jctech888.com.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ja.hnjuh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://im.muxihuayi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gn.panjiajie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bu.colortex.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ut.hnjuh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ji.hahajie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ma.huanxung.cn

[K07] 进制转换
来源：http://lh.gzmigu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ih.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bz.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oj.szxytkj.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tb.szxytkj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jl.wgjwhj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bd.jianghongdianzi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ut.panjiajie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wy.hahajie.cn

[K08] 二进制序列化（非 JSON）
来源：http://bk.hahajie.cn

Py:   pickle.dumps(obj)
来源：http://vb.newstarts.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bn.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://he.jianghongdianzi.cn

TS:   v8.serialize(obj)        // Node
来源：http://qk.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sh.szsharing.cn

Go:   encoding/gob
来源：http://op.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://bt.jianghongdianzi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yv.chemitech.net.cn

================================================================================
来源：http://yd.colortex.cn

L. 网络请求
来源：http://gx.shtwfgs.cn

================================================================================
来源：http://ym.panjiajie.cn

[L01] 发送 GET 请求
来源：http://rb.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gw.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nv.muxihuayi.cn

JS:   await fetch(url)
来源：http://md.jianghongdianzi.cn

TS:   await fetch(url)
来源：http://qc.colortex.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nc.nicolike.cn

Go:   resp, err := http.Get(url)
来源：http://ao.wgjwhj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cy.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sy.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://rw.newstarts.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nv.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gm.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://co.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://im.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yz.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zi.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wh.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kc.jianghongdianzi.cn

[L03] 设置自定义请求头
来源：http://cg.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ky.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qq.huixinmuqiang.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ow.yuexingan06.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ju.haigaiapp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://my.wgjwhj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xt.colortex.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://la.colortex.cn

[L04] 设置超时
来源：http://wo.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://pk.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mh.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fa.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gu.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sm.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://my.yuntaijiaju.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xw.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://np.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://hu.jianghongdianzi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tw.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gw.bookmarksfly.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ol.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ng.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://un.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rr.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ux.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://om.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://qu.nszjky.cn

Py:   resp.json()
来源：http://oh.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://kn.hnjuh.cn

JS:   await resp.json()
来源：http://zj.yuexingan06.cn

TS:   await resp.json()
来源：http://wk.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rn.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bp.yuntaijiaju.cn

Ruby: JSON.parse(resp.body)
来源：http://vm.szxytkj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zk.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://lm.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dq.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rq.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://ve.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://sv.bjjhwx.cn

Java: resp.statusCode()
来源：http://qn.lnxyls.cn

Go:   resp.StatusCode
来源：http://dv.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://dr.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ld.521024.cn

[L08] 并发请求多个地址
来源：http://fv.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wi.521024.cn

PHP:  curl_multi_init() 系列
来源：http://dl.gzmigu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ii.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wx.chemitech.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jw.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nl.huanxung.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xy.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fr.asd995.cn

================================================================================
来源：http://gi.521024.cn

M. 命令行 / 进程 / 环境
来源：http://tc.jctech888.com.cn

================================================================================
来源：http://bo.szsharing.cn

[M01] 读取命令行参数
来源：http://yf.yuexingan06.cn

Py:   sys.argv[1:]
来源：http://ef.panjiajie.cn

PHP:  $argv;  $argc;
来源：http://ek.szxytkj.cn

JS:   process.argv.slice(2)
来源：http://hy.asd995.cn

TS:   process.argv.slice(2)
来源：http://oq.newstarts.cn

Java: args 数组（main 方法参数）
来源：http://bv.huanxung.cn

Go:   os.Args[1:]
来源：http://ue.521024.cn

Ruby: ARGV
来源：http://sh.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://hx.lnxyls.cn

[M02] 读取环境变量
来源：http://mp.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://mg.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jf.bjjhwx.cn

JS:   process.env.HOME
来源：http://zn.bjjhwx.cn

TS:   process.env.HOME
来源：http://te.nicolike.cn

Java: System.getenv("HOME")
来源：http://fe.bjjhwx.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lk.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://ov.huixinmuqiang.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ui.shxzukj.cn

[M03] 执行外部命令
来源：http://ck.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://su.asd995.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cj.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pl.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xp.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mb.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ko.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vl.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://ph.colortex.cn

[M04] 获取当前工作目录
来源：http://we.521024.cn

Py:   os.getcwd()
来源：http://py.shxzukj.cn

PHP:  getcwd();
来源：http://jp.huixiangedu.cn

JS:   process.cwd()
来源：http://hm.jctech888.com.cn

TS:   process.cwd()
来源：http://ny.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://cf.hnjuh.cn

Go:   os.Getwd()
来源：http://hn.szsharing.cn

Ruby: Dir.pwd
来源：http://vv.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lc.colortex.cn

[M05] 设置退出码
来源：http://xz.asd995.cn

Py:   sys.exit(1)
来源：http://pc.muxihuayi.cn

PHP:  exit(1);
来源：http://tp.panjiajie.cn

JS:   process.exit(1)
来源：http://au.yuexingan06.cn

TS:   process.exit(1)
来源：http://oh.nicolike.cn

Java: System.exit(1)
来源：http://bm.huanxung.cn

Go:   os.Exit(1)
来源：http://wo.shxzskj.cn

Ruby: exit 1
来源：http://oq.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cp.yuexingan06.cn

[M06] 向标准错误输出
来源：http://kt.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://gc.huanxung.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yp.yuntaijiaju.cn

JS:   console.error("err")
来源：http://di.bjjhwx.cn

TS:   console.error("err")
来源：http://qv.chemitech.net.cn

Java: System.err.println("err")
来源：http://cc.huixinmuqiang.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ij.huanxung.cn

Ruby: warn "err"
来源：http://uy.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://oe.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://am.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://ue.9csxet.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mk.szsharing.cn

JS:   require.main === module
来源：http://od.muxihuayi.cn

TS:   require.main === module
来源：http://mp.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://eb.bookmarksfly.cn

Go:   func main()
来源：http://if.nszjky.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://of.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://mq.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://yq.yuntaijiaju.cn

Py:   platform.system();  platform.python_version()
来源：http://mg.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://yd.haigaiapp.cn

JS:   process.platform;  process.version
来源：http://cd.huanxung.cn

TS:   process.platform;  process.version
来源：http://ej.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ik.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bw.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zu.shtwfgs.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sh.huanxung.cn

================================================================================
来源：http://mb.chemitech.net.cn

N. 数据结构与算法
来源：http://of.bookmarksfly.cn

================================================================================
来源：http://qz.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://tg.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pb.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dd.wgjwhj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vc.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gb.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iu.yuntaijiaju.cn

Go:   sort.SearchInts(arr, x)
来源：http://yv.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gi.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vs.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://rg.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://ex.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://it.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qx.lnxyls.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ax.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uj.szxytkj.cn

Go:   slices.Sort(arr)
来源：http://tt.panjiajie.cn

Ruby: arr.sort
来源：http://pi.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sf.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://rd.521024.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ks.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://xu.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://co.szsharing.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hr.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nz.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oe.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kk.shtwfgs.cn

[N04] 斐波那契数列
来源：http://jb.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cj.lnxyls.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wg.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vm.wgjwhj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fm.9csxet.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mw.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://en.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ti.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jv.szsharing.cn

[N05] 最大公约数
来源：http://vu.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://rk.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rl.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://er.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fx.yuntaijiaju.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nj.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zs.colortex.cn

Ruby: a.gcd(b)
来源：http://yx.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://um.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://tk.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://zn.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://zm.yuexingan06.cn

JS:   s === [...s].reverse().join("")
来源：http://xf.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://dn.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ss.newstarts.cn

Go:   // 双指针从两端比较
来源：http://zl.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://oz.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ve.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://ea.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dr.9csxet.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ov.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xo.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://ck.szxytkj.cn

Java: // 手写 HashMap
来源：http://ds.nszjky.cn

Go:   // 手写 map[int]int
来源：http://bu.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ix.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bw.szsharing.cn

[N08] 生成全排列
来源：http://hp.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://tc.shtwfgs.cn

PHP:  // 手写递归交换
来源：http://nt.asd995.cn

JS:   // 手写回溯递归
来源：http://fg.newstarts.cn

TS:   // 手写回溯递归
来源：http://vw.nicolike.cn


<!-- 参考信息 -->