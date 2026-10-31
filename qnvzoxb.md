代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nq.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ej.521024.cn

JS:   JSON.stringify(obj)
来源：http://bd.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://jx.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hq.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://ks.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hn.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://li.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://xd.yuexingan06.cn

Py:   json.loads(s)
来源：http://tl.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xi.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://ul.lnxyls.cn

TS:   JSON.parse(s)
来源：http://rc.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rd.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://bx.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://vg.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rj.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://cu.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jj.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sa.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wm.yuntaijiaju.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rc.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jv.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ow.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cx.newstarts.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ep.nszjky.cn

[K04] 读取 JSON 文件
来源：http://rl.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jc.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gc.szxytkj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kv.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yr.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ki.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pe.9csxet.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aj.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nj.hahajie.cn

[K05] 深拷贝对象
来源：http://im.521024.cn

Py:   copy.deepcopy(obj)
来源：http://bi.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://hg.521024.cn

JS:   structuredClone(obj)
来源：http://ls.szsharing.cn

TS:   structuredClone(obj)
来源：http://lc.jctech888.com.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uu.wgjwhj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gu.asd995.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pu.bjjhwx.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ck.gzmigu.cn

[K06] 解析 URL 查询串
来源：http://lf.panjiajie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vq.shtwfgs.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oy.gzmigu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ct.hnjuh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cs.nicolike.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jk.huixiangedu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hr.shxzukj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bn.9csxet.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dd.huanxung.cn

[K07] 进制转换
来源：http://ik.asd995.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://np.521024.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pz.hahajie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iy.gzmigu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://va.huanxung.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bv.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pn.bjjhwx.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://he.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kx.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ml.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://nb.shxzukj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ma.bookmarksfly.cn

JS:   v8.serialize(obj)        // Node
来源：http://lg.yuntaijiaju.cn

TS:   v8.serialize(obj)        // Node
来源：http://cm.szsharing.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wh.asd995.cn

Go:   encoding/gob
来源：http://nk.nicolike.cn

Ruby: Marshal.dump(obj)
来源：http://su.huixiangedu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lm.asd995.cn

================================================================================
来源：http://lt.panjiajie.cn

L. 网络请求
来源：http://pa.hnjuh.cn

================================================================================
来源：http://vh.asd995.cn

[L01] 发送 GET 请求
来源：http://xi.asd995.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yj.colortex.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sc.gzmigu.cn

JS:   await fetch(url)
来源：http://ia.9csxet.cn

TS:   await fetch(url)
来源：http://nj.hnjuh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mo.9csxet.cn

Go:   resp, err := http.Get(url)
来源：http://xv.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dc.hnjuh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ik.nszjky.cn

[L02] 发送 POST JSON
来源：http://rb.asd995.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ex.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lh.newstarts.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yw.szsharing.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qk.muxihuayi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ee.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cd.yuexingan06.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hc.haigaiapp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pb.hnjuh.cn

[L03] 设置自定义请求头
来源：http://sz.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://al.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://si.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yx.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cz.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vm.jctech888.com.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ph.shtwfgs.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vv.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gy.jctech888.com.cn

[L04] 设置超时
来源：http://el.nszjky.cn

Py:   requests.get(url, timeout=5)
来源：http://wf.colortex.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ve.shxzukj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qu.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ck.yuntaijiaju.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://om.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ls.hahajie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nw.shxzskj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://by.szsharing.cn

[L05] 上传文件（multipart）
来源：http://zg.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mi.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pe.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yg.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sp.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gf.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jw.shxzskj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://us.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ki.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://vx.jianghongdianzi.cn

Py:   resp.json()
来源：http://vs.521024.cn

PHP:  json_decode($body, true);
来源：http://rh.jianghongdianzi.cn

JS:   await resp.json()
来源：http://sm.muxihuayi.cn

TS:   await resp.json()
来源：http://ya.newstarts.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dr.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://an.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://hg.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://um.jctech888.com.cn

[L07] 处理 HTTP 状态码
来源：http://tl.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wl.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nn.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://mx.wgjwhj.cn

TS:   resp.ok;  resp.status
来源：http://cl.bjjhwx.cn

Java: resp.statusCode()
来源：http://ux.huanxung.cn

Go:   resp.StatusCode
来源：http://vg.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://dm.nicolike.cn

C#:   (int)resp.StatusCode
来源：http://oo.nszjky.cn

[L08] 并发请求多个地址
来源：http://pg.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ln.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://bi.jctech888.com.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.nszjky.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sq.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sf.huixiangedu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wn.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yk.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ov.huanxung.cn

================================================================================
来源：http://xz.colortex.cn

M. 命令行 / 进程 / 环境
来源：http://id.huixinmuqiang.cn

================================================================================
来源：http://ta.colortex.cn

[M01] 读取命令行参数
来源：http://lf.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://md.newstarts.cn

PHP:  $argv;  $argc;
来源：http://fo.asd995.cn

JS:   process.argv.slice(2)
来源：http://pn.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://if.shxzskj.cn

Java: args 数组（main 方法参数）
来源：http://wd.shtwfgs.cn

Go:   os.Args[1:]
来源：http://wd.shxzukj.cn

Ruby: ARGV
来源：http://jt.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://lq.wgjwhj.cn

[M02] 读取环境变量
来源：http://wk.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://be.yuexingan06.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ed.gzmigu.cn

JS:   process.env.HOME
来源：http://wv.nicolike.cn

TS:   process.env.HOME
来源：http://px.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://ff.asd995.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ki.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://xe.panjiajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dv.haigaiapp.cn

[M03] 执行外部命令
来源：http://kl.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uz.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vi.shxzukj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sn.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wl.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bz.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rs.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xm.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://jq.szxytkj.cn

[M04] 获取当前工作目录
来源：http://sq.szsharing.cn

Py:   os.getcwd()
来源：http://lz.9csxet.cn

PHP:  getcwd();
来源：http://iu.jctech888.com.cn

JS:   process.cwd()
来源：http://ua.nicolike.cn

TS:   process.cwd()
来源：http://gq.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://ks.bjjhwx.cn

Go:   os.Getwd()
来源：http://xn.szsharing.cn

Ruby: Dir.pwd
来源：http://lf.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hb.gzmigu.cn

[M05] 设置退出码
来源：http://ux.nicolike.cn

Py:   sys.exit(1)
来源：http://gg.muxihuayi.cn

PHP:  exit(1);
来源：http://yl.muxihuayi.cn

JS:   process.exit(1)
来源：http://mg.9csxet.cn

TS:   process.exit(1)
来源：http://gh.muxihuayi.cn

Java: System.exit(1)
来源：http://uh.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://bf.nicolike.cn

Ruby: exit 1
来源：http://fm.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gs.wgjwhj.cn

[M06] 向标准错误输出
来源：http://qz.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://id.newstarts.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dc.lnxyls.cn

JS:   console.error("err")
来源：http://un.huanxung.cn

TS:   console.error("err")
来源：http://bj.muxihuayi.cn

Java: System.err.println("err")
来源：http://zw.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tu.9csxet.cn

Ruby: warn "err"
来源：http://kh.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://nr.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://ag.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://zv.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dc.huixiangedu.cn

JS:   require.main === module
来源：http://ra.asd995.cn

TS:   require.main === module
来源：http://xi.huixinmuqiang.cn

Java: public static void main(String[] args)
来源：http://nc.szxytkj.cn

Go:   func main()
来源：http://al.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mw.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://xj.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://xl.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://ad.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://hm.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://am.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://xi.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://on.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pv.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nc.jianghongdianzi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ek.szsharing.cn

================================================================================
来源：http://zx.shtwfgs.cn

N. 数据结构与算法
来源：http://td.bookmarksfly.cn

================================================================================
来源：http://lu.nszjky.cn

[N01] 二分查找（有序数组）
来源：http://hi.bookmarksfly.cn

Py:   bisect.bisect_left(arr, x)
来源：http://as.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cb.panjiajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kl.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yl.9csxet.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eu.gzmigu.cn

Go:   sort.SearchInts(arr, x)
来源：http://qz.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tb.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://le.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://wf.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://no.hahajie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gi.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yk.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://go.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bo.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://bc.huanxung.cn

Ruby: arr.sort
来源：http://du.chemitech.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ux.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://at.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gm.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://py.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gy.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ja.huixinmuqiang.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bz.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ib.shxzskj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wf.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://og.panjiajie.cn

[N04] 斐波那契数列
来源：http://sq.bjjhwx.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tj.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nj.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dd.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uv.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://am.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oy.lnxyls.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gw.wgjwhj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oi.yuntaijiaju.cn

[N05] 最大公约数
来源：http://wx.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://lt.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dv.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sz.szxytkj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wn.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zn.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ny.huanxung.cn

Ruby: a.gcd(b)
来源：http://wl.szsharing.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rn.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://ny.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://xy.muxihuayi.cn

PHP:  $s === strrev($s);
来源：http://wv.newstarts.cn

JS:   s === [...s].reverse().join("")
来源：http://ln.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://pe.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rt.panjiajie.cn

Go:   // 双指针从两端比较
来源：http://uu.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ge.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yd.gzmigu.cn

[N07] 两数之和（返回下标）
来源：http://bf.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rw.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ku.colortex.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://am.panjiajie.cn

TS:   // 手写 Map<string, number>
来源：http://cf.huanxung.cn

Java: // 手写 HashMap
来源：http://ha.9csxet.cn

Go:   // 手写 map[int]int
来源：http://wq.hnjuh.cn

Ruby: // 手写 Hash
来源：http://iz.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hw.wgjwhj.cn

[N08] 生成全排列
来源：http://gg.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://su.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://jp.hahajie.cn

JS:   // 手写回溯递归
来源：http://qs.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://et.shxzskj.cn

Java: // 手写回溯递归
来源：http://gw.newstarts.cn

Go:   // 手写回溯递归
来源：http://wn.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://zq.521024.cn

C#:   // 手写回溯递归
来源：http://vh.yuexingan06.cn

[N09] 栈与队列
来源：http://vl.jianghongdianzi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pn.huixinmuqiang.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pp.gzmigu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pw.shtwfgs.cn


<!-- 参考信息 -->