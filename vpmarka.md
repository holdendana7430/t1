代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://zo.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lv.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mk.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oy.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rj.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cw.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kv.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zy.yuexingan06.cn

================================================================================
来源：http://wi.9csxet.cn

K. JSON 与序列化
来源：http://hw.shtwfgs.cn

================================================================================
来源：http://rl.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://ov.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wp.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qp.asd995.cn

JS:   JSON.stringify(obj)
来源：http://wu.asd995.cn

TS:   JSON.stringify(obj)
来源：http://uh.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vx.shtwfgs.cn

Go:   json.Marshal(obj)
来源：http://pj.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jw.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ap.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ag.yuexingan06.cn

Py:   json.loads(s)
来源：http://bg.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ia.hnjuh.cn

JS:   JSON.parse(s)
来源：http://hv.asd995.cn

TS:   JSON.parse(s)
来源：http://bh.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iq.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://cy.hahajie.cn

Ruby: JSON.parse(s)
来源：http://ze.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yw.yuexingan06.cn

[K03] JSON 美化输出（带缩进）
来源：http://xn.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vf.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kd.haigaiapp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yx.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hl.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bn.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rf.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ir.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yl.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://pb.shxzskj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tf.panjiajie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yq.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ol.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dk.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yk.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jk.szsharing.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lo.wgjwhj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hh.szxytkj.cn

[K05] 深拷贝对象
来源：http://ts.jianghongdianzi.cn

Py:   copy.deepcopy(obj)
来源：http://uc.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://ma.9csxet.cn

JS:   structuredClone(obj)
来源：http://wh.colortex.cn

TS:   structuredClone(obj)
来源：http://vi.yuntaijiaju.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mw.shtwfgs.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jw.huixiangedu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vr.panjiajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wg.nszjky.cn

[K06] 解析 URL 查询串
来源：http://ec.521024.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bc.muxihuayi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://my.huanxung.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vd.shxzukj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wp.huixiangedu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pb.jianghongdianzi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jh.yuntaijiaju.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cw.nszjky.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fh.huanxung.cn

[K07] 进制转换
来源：http://qq.huixinmuqiang.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gg.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vg.shtwfgs.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://js.newstarts.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ev.shxzukj.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mi.bjjhwx.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ae.shtwfgs.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://re.521024.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yc.chemitech.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://ev.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://xw.huixinmuqiang.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ml.nicolike.cn

JS:   v8.serialize(obj)        // Node
来源：http://bn.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://af.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wf.shxzskj.cn

Go:   encoding/gob
来源：http://gf.haigaiapp.cn

Ruby: Marshal.dump(obj)
来源：http://dv.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pp.panjiajie.cn

================================================================================
来源：http://qg.yuexingan06.cn

L. 网络请求
来源：http://iw.huixiangedu.cn

================================================================================
来源：http://eh.jctech888.com.cn

[L01] 发送 GET 请求
来源：http://cu.nszjky.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wf.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mw.hnjuh.cn

JS:   await fetch(url)
来源：http://kr.hahajie.cn

TS:   await fetch(url)
来源：http://cj.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cd.chemitech.net.cn

Go:   resp, err := http.Get(url)
来源：http://ik.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bx.nszjky.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vi.9csxet.cn

[L02] 发送 POST JSON
来源：http://wt.nicolike.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qq.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mj.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fr.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tn.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mw.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nb.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qx.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eg.hahajie.cn

[L03] 设置自定义请求头
来源：http://zy.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fe.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tx.huixiangedu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mo.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uq.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ve.shxzukj.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qf.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ge.shtwfgs.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sb.szsharing.cn

[L04] 设置超时
来源：http://ix.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://il.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wj.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dk.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xk.asd995.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pe.szxytkj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ur.wgjwhj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dd.huixinmuqiang.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lz.9csxet.cn

[L05] 上传文件（multipart）
来源：http://lu.shxzukj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://no.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qa.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qs.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bt.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://io.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ds.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://au.hahajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wz.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://du.newstarts.cn

Py:   resp.json()
来源：http://bv.newstarts.cn

PHP:  json_decode($body, true);
来源：http://yu.wgjwhj.cn

JS:   await resp.json()
来源：http://fx.bjjhwx.cn

TS:   await resp.json()
来源：http://xx.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ch.szsharing.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ek.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://db.muxihuayi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bs.colortex.cn

[L07] 处理 HTTP 状态码
来源：http://my.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hr.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tn.gzmigu.cn

JS:   resp.ok;  resp.status
来源：http://iz.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://gx.9csxet.cn

Java: resp.statusCode()
来源：http://cp.hahajie.cn

Go:   resp.StatusCode
来源：http://yo.shxzskj.cn

Ruby: resp.code.to_i
来源：http://bs.newstarts.cn

C#:   (int)resp.StatusCode
来源：http://cw.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://sv.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gb.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://bq.huixinmuqiang.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zn.szxytkj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://it.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fe.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ao.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vf.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ta.chemitech.net.cn

================================================================================
来源：http://lt.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://mt.huixinmuqiang.cn

================================================================================
来源：http://qk.wgjwhj.cn

[M01] 读取命令行参数
来源：http://hg.gzmigu.cn

Py:   sys.argv[1:]
来源：http://lh.szsharing.cn

PHP:  $argv;  $argc;
来源：http://sr.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://yn.bookmarksfly.cn

TS:   process.argv.slice(2)
来源：http://ym.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://fm.jianghongdianzi.cn

Go:   os.Args[1:]
来源：http://bk.hnjuh.cn

Ruby: ARGV
来源：http://oe.wgjwhj.cn

C#:   args 数组（Main 方法参数）
来源：http://al.asd995.cn

[M02] 读取环境变量
来源：http://uq.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://de.nicolike.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ib.bjjhwx.cn

JS:   process.env.HOME
来源：http://rz.huanxung.cn

TS:   process.env.HOME
来源：http://cf.bjjhwx.cn

Java: System.getenv("HOME")
来源：http://qb.9csxet.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zu.nszjky.cn

Ruby: ENV["HOME"]
来源：http://vj.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dd.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://hi.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kw.shtwfgs.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jl.yuntaijiaju.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cs.szxytkj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fv.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cr.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bw.muxihuayi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xv.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://df.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://sh.yuntaijiaju.cn

Py:   os.getcwd()
来源：http://dx.szxytkj.cn

PHP:  getcwd();
来源：http://kt.521024.cn

JS:   process.cwd()
来源：http://by.hahajie.cn

TS:   process.cwd()
来源：http://wl.newstarts.cn

Java: Path.of("").toAbsolutePath()
来源：http://ul.wgjwhj.cn

Go:   os.Getwd()
来源：http://ir.nszjky.cn

Ruby: Dir.pwd
来源：http://az.gzmigu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dz.newstarts.cn

[M05] 设置退出码
来源：http://rp.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://wk.newstarts.cn

PHP:  exit(1);
来源：http://sq.bookmarksfly.cn

JS:   process.exit(1)
来源：http://at.hahajie.cn

TS:   process.exit(1)
来源：http://lo.9csxet.cn

Java: System.exit(1)
来源：http://yi.hnjuh.cn

Go:   os.Exit(1)
来源：http://ri.hnjuh.cn

Ruby: exit 1
来源：http://vd.wgjwhj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ul.szsharing.cn

[M06] 向标准错误输出
来源：http://ln.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://gi.9csxet.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hx.asd995.cn

JS:   console.error("err")
来源：http://dr.shxzukj.cn

TS:   console.error("err")
来源：http://uj.jctech888.com.cn

Java: System.err.println("err")
来源：http://fe.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uo.hnjuh.cn

Ruby: warn "err"
来源：http://uz.huixiangedu.cn

C#:   Console.Error.WriteLine("err")
来源：http://pe.yuntaijiaju.cn

[M07] 判断是否为主入口
来源：http://uw.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://wj.huixinmuqiang.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://du.panjiajie.cn

JS:   require.main === module
来源：http://lj.lnxyls.cn

TS:   require.main === module
来源：http://hy.szsharing.cn

Java: public static void main(String[] args)
来源：http://zw.huixiangedu.cn

Go:   func main()
来源：http://dn.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tv.bjjhwx.cn

C#:   static void Main(string[] args)
来源：http://pe.haigaiapp.cn

[M08] 获取系统与运行时信息
来源：http://fn.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://nm.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://tl.szxytkj.cn

JS:   process.platform;  process.version
来源：http://bu.asd995.cn

TS:   process.platform;  process.version
来源：http://xm.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cm.yuntaijiaju.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gx.newstarts.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gb.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://re.hahajie.cn

================================================================================
来源：http://yu.nicolike.cn

N. 数据结构与算法
来源：http://ty.nszjky.cn

================================================================================
来源：http://xx.colortex.cn

[N01] 二分查找（有序数组）
来源：http://lt.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ei.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jy.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bt.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uv.lnxyls.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hf.szxytkj.cn

Go:   sort.SearchInts(arr, x)
来源：http://xr.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://li.9csxet.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zc.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://yc.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://to.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rv.szxytkj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kt.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uk.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pq.bjjhwx.cn

Go:   slices.Sort(arr)
来源：http://xj.colortex.cn

Ruby: arr.sort
来源：http://gw.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qj.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://io.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ld.asd995.cn

PHP:  // 递归实现，或用 usort
来源：http://ij.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nz.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ea.yuexingan06.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sx.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oz.gzmigu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://un.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jr.shxzskj.cn

[N04] 斐波那契数列
来源：http://gh.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xq.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sr.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zj.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ai.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bk.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fn.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://id.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nq.bjjhwx.cn

[N05] 最大公约数
来源：http://xa.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://rs.jianghongdianzi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pc.shtwfgs.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zd.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ta.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://er.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bk.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://qh.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hr.nicolike.cn

[N06] 判断回文字符串
来源：http://va.9csxet.cn

Py:   s == s[::-1]
来源：http://jm.asd995.cn

PHP:  $s === strrev($s);
来源：http://go.jctech888.com.cn

JS:   s === [...s].reverse().join("")
来源：http://ac.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://mm.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zp.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://mw.huanxung.cn

Ruby: s == s.reverse
来源：http://qa.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kj.wgjwhj.cn

[N07] 两数之和（返回下标）
来源：http://cr.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xw.nicolike.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://is.chemitech.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jf.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://xt.wgjwhj.cn

Java: // 手写 HashMap
来源：http://if.yuntaijiaju.cn

Go:   // 手写 map[int]int
来源：http://qg.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://nr.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ax.bjjhwx.cn

[N08] 生成全排列
来源：http://nc.newstarts.cn


<!-- 参考信息 -->