代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xj.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cv.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ih.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vf.nszjky.cn

================================================================================
来源：http://yy.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ut.huixiangedu.cn

================================================================================
来源：http://ur.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://mt.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fv.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fq.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ur.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://ba.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nj.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://vr.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gj.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yv.colortex.cn

[K02] JSON 字符串转对象
来源：http://px.hnjuh.cn

Py:   json.loads(s)
来源：http://un.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yw.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://kg.colortex.cn

TS:   JSON.parse(s)
来源：http://wa.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://in.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://wp.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ow.lnxyls.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ey.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://jd.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xi.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jp.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nd.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qn.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://av.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://az.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ci.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://at.nszjky.cn

[K04] 读取 JSON 文件
来源：http://ok.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jj.szxytkj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qy.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ep.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://td.szsharing.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zk.9csxet.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tt.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rd.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pc.szxytkj.cn

[K05] 深拷贝对象
来源：http://nh.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://vi.panjiajie.cn

PHP:  unserialize(serialize($obj));
来源：http://oo.chemitech.net.cn

JS:   structuredClone(obj)
来源：http://fc.hnjuh.cn

TS:   structuredClone(obj)
来源：http://pz.asd995.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fe.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jr.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jl.yuexingan06.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gy.hnjuh.cn

[K06] 解析 URL 查询串
来源：http://bq.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hq.bjjhwx.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gu.muxihuayi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vn.szsharing.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://so.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qb.muxihuayi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xb.lnxyls.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xw.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jh.szxytkj.cn

[K07] 进制转换
来源：http://rr.nicolike.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pc.yuexingan06.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gt.haigaiapp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gt.hahajie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ky.haigaiapp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mq.lnxyls.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tk.521024.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://it.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sb.hnjuh.cn

[K08] 二进制序列化（非 JSON）
来源：http://rx.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://gl.szxytkj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ge.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://lu.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://gl.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lm.yuntaijiaju.cn

Go:   encoding/gob
来源：http://nu.shxzukj.cn

Ruby: Marshal.dump(obj)
来源：http://lu.shxzukj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ai.newstarts.cn

================================================================================
来源：http://ds.gzmigu.cn

L. 网络请求
来源：http://ys.huixinmuqiang.cn

================================================================================
来源：http://lp.521024.cn

[L01] 发送 GET 请求
来源：http://cx.jianghongdianzi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uo.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cm.nszjky.cn

JS:   await fetch(url)
来源：http://lt.bjjhwx.cn

TS:   await fetch(url)
来源：http://ct.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xw.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://lv.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lx.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kc.szxytkj.cn

[L02] 发送 POST JSON
来源：http://qn.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fi.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rx.jianghongdianzi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uk.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ob.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ei.gzmigu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tk.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nr.shxzskj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rj.521024.cn

[L03] 设置自定义请求头
来源：http://rx.nicolike.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mk.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bh.szsharing.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wx.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uy.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vq.hahajie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jd.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lh.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dw.muxihuayi.cn

[L04] 设置超时
来源：http://ia.huanxung.cn

Py:   requests.get(url, timeout=5)
来源：http://ep.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nm.huixinmuqiang.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.asd995.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oe.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qz.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://le.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://as.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aa.haigaiapp.cn

[L05] 上传文件（multipart）
来源：http://so.huixiangedu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ej.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kc.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lg.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vm.huixinmuqiang.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ji.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cy.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tf.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kh.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://gg.huixiangedu.cn

Py:   resp.json()
来源：http://tr.jctech888.com.cn

PHP:  json_decode($body, true);
来源：http://ff.huixiangedu.cn

JS:   await resp.json()
来源：http://ci.bookmarksfly.cn

TS:   await resp.json()
来源：http://uh.521024.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bg.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nq.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://bb.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ca.szsharing.cn

[L07] 处理 HTTP 状态码
来源：http://nr.bjjhwx.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hn.newstarts.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ps.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://wu.colortex.cn

TS:   resp.ok;  resp.status
来源：http://ey.shtwfgs.cn

Java: resp.statusCode()
来源：http://dv.521024.cn

Go:   resp.StatusCode
来源：http://ez.jctech888.com.cn

Ruby: resp.code.to_i
来源：http://wr.jctech888.com.cn

C#:   (int)resp.StatusCode
来源：http://br.hahajie.cn

[L08] 并发请求多个地址
来源：http://rk.asd995.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://du.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://gr.bookmarksfly.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gg.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cg.shxzukj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rq.hahajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zr.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fa.yuexingan06.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ck.jctech888.com.cn

================================================================================
来源：http://jy.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://wv.panjiajie.cn

================================================================================
来源：http://tv.shtwfgs.cn

[M01] 读取命令行参数
来源：http://ke.hahajie.cn

Py:   sys.argv[1:]
来源：http://uk.chemitech.net.cn

PHP:  $argv;  $argc;
来源：http://if.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://to.huixiangedu.cn

TS:   process.argv.slice(2)
来源：http://bj.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://ac.szsharing.cn

Go:   os.Args[1:]
来源：http://cl.521024.cn

Ruby: ARGV
来源：http://sd.nicolike.cn

C#:   args 数组（Main 方法参数）
来源：http://yo.hnjuh.cn

[M02] 读取环境变量
来源：http://lu.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://vd.shtwfgs.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cx.jctech888.com.cn

JS:   process.env.HOME
来源：http://wk.nicolike.cn

TS:   process.env.HOME
来源：http://nx.gzmigu.cn

Java: System.getenv("HOME")
来源：http://lb.wgjwhj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bk.shxzskj.cn

Ruby: ENV["HOME"]
来源：http://qz.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gz.hnjuh.cn

[M03] 执行外部命令
来源：http://ov.jianghongdianzi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://or.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ik.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dl.bjjhwx.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sk.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://or.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cm.hnjuh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ph.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://xl.yuexingan06.cn

[M04] 获取当前工作目录
来源：http://kl.huanxung.cn

Py:   os.getcwd()
来源：http://sm.huixiangedu.cn

PHP:  getcwd();
来源：http://fn.newstarts.cn

JS:   process.cwd()
来源：http://bc.521024.cn

TS:   process.cwd()
来源：http://al.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://us.hnjuh.cn

Go:   os.Getwd()
来源：http://qn.szsharing.cn

Ruby: Dir.pwd
来源：http://ow.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rc.yuntaijiaju.cn

[M05] 设置退出码
来源：http://pb.521024.cn

Py:   sys.exit(1)
来源：http://xf.panjiajie.cn

PHP:  exit(1);
来源：http://ey.jctech888.com.cn

JS:   process.exit(1)
来源：http://rp.nicolike.cn

TS:   process.exit(1)
来源：http://gr.shtwfgs.cn

Java: System.exit(1)
来源：http://kk.hnjuh.cn

Go:   os.Exit(1)
来源：http://tb.lnxyls.cn

Ruby: exit 1
来源：http://cr.jianghongdianzi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tn.jctech888.com.cn

[M06] 向标准错误输出
来源：http://pc.huixiangedu.cn

Py:   print("err", file=sys.stderr)
来源：http://if.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://io.yuexingan06.cn

JS:   console.error("err")
来源：http://xw.szsharing.cn

TS:   console.error("err")
来源：http://hj.shtwfgs.cn

Java: System.err.println("err")
来源：http://yr.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yt.haigaiapp.cn

Ruby: warn "err"
来源：http://el.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://mi.521024.cn

[M07] 判断是否为主入口
来源：http://wt.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://kb.colortex.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qc.asd995.cn

JS:   require.main === module
来源：http://kg.nicolike.cn

TS:   require.main === module
来源：http://jc.wgjwhj.cn

Java: public static void main(String[] args)
来源：http://zd.yuntaijiaju.cn

Go:   func main()
来源：http://hd.colortex.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kp.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://kl.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://sx.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://sr.9csxet.cn

PHP:  PHP_OS;  phpversion();
来源：http://xl.yuntaijiaju.cn

JS:   process.platform;  process.version
来源：http://xa.shxzukj.cn

TS:   process.platform;  process.version
来源：http://zs.muxihuayi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wf.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xm.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kk.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dv.hnjuh.cn

================================================================================
来源：http://bb.shxzukj.cn

N. 数据结构与算法
来源：http://ym.bookmarksfly.cn

================================================================================
来源：http://oq.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://oo.yuntaijiaju.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pp.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mh.shtwfgs.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ca.yuexingan06.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jm.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xo.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://jb.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bt.yuntaijiaju.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pn.newstarts.cn

[N02] 排序（工程实践用内置实现）
来源：http://az.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://so.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jz.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pf.shxzskj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ks.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eb.szsharing.cn

Go:   slices.Sort(arr)
来源：http://ws.yuexingan06.cn

Ruby: arr.sort
来源：http://he.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sh.wgjwhj.cn

[N03] 快速排序（分治示例）
来源：http://su.colortex.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qw.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://mg.lnxyls.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zg.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dg.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://je.bjjhwx.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rf.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wh.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dr.shxzskj.cn

[N04] 斐波那契数列
来源：http://vg.haigaiapp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bv.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://km.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://up.nszjky.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hj.huixinmuqiang.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lo.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bc.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oa.hnjuh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hi.hnjuh.cn

[N05] 最大公约数
来源：http://sc.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://ky.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kt.szsharing.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jv.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fc.muxihuayi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yb.szxytkj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dx.panjiajie.cn

Ruby: a.gcd(b)
来源：http://ho.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yf.newstarts.cn

[N06] 判断回文字符串
来源：http://dg.asd995.cn

Py:   s == s[::-1]
来源：http://qt.hahajie.cn

PHP:  $s === strrev($s);
来源：http://ud.colortex.cn

JS:   s === [...s].reverse().join("")
来源：http://kp.9csxet.cn

TS:   s === [...s].reverse().join("")
来源：http://iv.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://te.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ad.shtwfgs.cn

Ruby: s == s.reverse
来源：http://xr.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cs.9csxet.cn

[N07] 两数之和（返回下标）
来源：http://jp.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ix.asd995.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tx.szxytkj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bk.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://vm.newstarts.cn

Java: // 手写 HashMap
来源：http://xv.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://ws.lnxyls.cn

Ruby: // 手写 Hash
来源：http://fy.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zp.9csxet.cn

[N08] 生成全排列
来源：http://ms.wgjwhj.cn

Py:   itertools.permutations(arr)
来源：http://eo.hahajie.cn

PHP:  // 手写递归交换
来源：http://wt.asd995.cn

JS:   // 手写回溯递归
来源：http://wi.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://bk.lnxyls.cn


<!-- 参考信息 -->