代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ag.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://oh.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gp.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hu.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://lk.hahajie.cn

Py:   json.loads(s)
来源：http://dv.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qi.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://dm.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://nx.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qb.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://hf.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://ug.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uu.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://vk.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://si.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aw.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.521024.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ko.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qr.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://df.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qo.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rm.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://jw.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ka.huixinmuqiang.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vp.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kv.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ux.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yg.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://to.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://et.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wj.huixiangedu.cn

[K05] 深拷贝对象
来源：http://ih.bookmarksfly.cn

Py:   copy.deepcopy(obj)
来源：http://ct.yuntaijiaju.cn

PHP:  unserialize(serialize($obj));
来源：http://zn.nszjky.cn

JS:   structuredClone(obj)
来源：http://ak.nicolike.cn

TS:   structuredClone(obj)
来源：http://gr.9csxet.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mm.szsharing.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cj.haigaiapp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lw.nicolike.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bh.nicolike.cn

[K06] 解析 URL 查询串
来源：http://bl.gzmigu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ro.huixinmuqiang.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ra.yuntaijiaju.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oa.asd995.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uz.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rl.newstarts.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lu.jctech888.com.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yo.gzmigu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hr.huixiangedu.cn

[K07] 进制转换
来源：http://ia.wgjwhj.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ut.muxihuayi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ao.chemitech.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kg.hnjuh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ln.nicolike.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ei.bookmarksfly.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://az.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gy.muxihuayi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yi.9csxet.cn

[K08] 二进制序列化（非 JSON）
来源：http://ft.huixinmuqiang.cn

Py:   pickle.dumps(obj)
来源：http://vy.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gi.huixinmuqiang.cn

JS:   v8.serialize(obj)        // Node
来源：http://ts.huixinmuqiang.cn

TS:   v8.serialize(obj)        // Node
来源：http://vu.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sv.haigaiapp.cn

Go:   encoding/gob
来源：http://pk.jctech888.com.cn

Ruby: Marshal.dump(obj)
来源：http://jv.bookmarksfly.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ih.muxihuayi.cn

================================================================================
来源：http://ht.huixiangedu.cn

L. 网络请求
来源：http://tq.yuntaijiaju.cn

================================================================================
来源：http://hr.hahajie.cn

[L01] 发送 GET 请求
来源：http://kr.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hw.asd995.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yz.lnxyls.cn

JS:   await fetch(url)
来源：http://af.shxzukj.cn

TS:   await fetch(url)
来源：http://cf.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tf.521024.cn

Go:   resp, err := http.Get(url)
来源：http://vq.521024.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jy.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qg.bjjhwx.cn

[L02] 发送 POST JSON
来源：http://ry.colortex.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bi.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ev.hahajie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vv.colortex.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fe.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yz.haigaiapp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gv.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fx.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gx.nszjky.cn

[L03] 设置自定义请求头
来源：http://lu.asd995.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gi.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ar.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qn.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pb.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yy.muxihuayi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oi.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ug.huixinmuqiang.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ep.shtwfgs.cn

[L04] 设置超时
来源：http://wz.9csxet.cn

Py:   requests.get(url, timeout=5)
来源：http://et.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ts.lnxyls.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qe.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yz.haigaiapp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vj.huixinmuqiang.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ky.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xn.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fv.newstarts.cn

[L05] 上传文件（multipart）
来源：http://jo.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://un.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xu.hnjuh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vk.nszjky.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sn.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tp.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hw.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ny.jctech888.com.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ng.asd995.cn

[L06] 解析响应为 JSON
来源：http://ow.9csxet.cn

Py:   resp.json()
来源：http://xp.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://lz.huixinmuqiang.cn

JS:   await resp.json()
来源：http://vc.newstarts.cn

TS:   await resp.json()
来源：http://xx.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ds.521024.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://da.huixinmuqiang.cn

Ruby: JSON.parse(resp.body)
来源：http://ll.panjiajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yx.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://dm.gzmigu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vh.jctech888.com.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xg.shxzukj.cn

JS:   resp.ok;  resp.status
来源：http://dn.chemitech.net.cn

TS:   resp.ok;  resp.status
来源：http://ch.yuntaijiaju.cn

Java: resp.statusCode()
来源：http://bd.nszjky.cn

Go:   resp.StatusCode
来源：http://no.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://tm.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://fu.jianghongdianzi.cn

[L08] 并发请求多个地址
来源：http://nt.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ov.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://ox.yuntaijiaju.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xw.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dp.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eq.colortex.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xu.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ci.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xf.shxzskj.cn

================================================================================
来源：http://gb.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://mj.panjiajie.cn

================================================================================
来源：http://nw.shxzskj.cn

[M01] 读取命令行参数
来源：http://sy.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://gy.nicolike.cn

PHP:  $argv;  $argc;
来源：http://ym.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://um.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://pq.wgjwhj.cn

Java: args 数组（main 方法参数）
来源：http://as.gzmigu.cn

Go:   os.Args[1:]
来源：http://fn.lnxyls.cn

Ruby: ARGV
来源：http://gl.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://wo.haigaiapp.cn

[M02] 读取环境变量
来源：http://ov.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://at.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rt.nszjky.cn

JS:   process.env.HOME
来源：http://bh.9csxet.cn

TS:   process.env.HOME
来源：http://od.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://wv.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jn.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://rw.szxytkj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lz.shxzukj.cn

[M03] 执行外部命令
来源：http://yx.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zq.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yi.lnxyls.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eg.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zt.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gt.hnjuh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yc.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lo.asd995.cn

C#:   Process.Start("ls", "-l");
来源：http://rb.muxihuayi.cn

[M04] 获取当前工作目录
来源：http://cj.chemitech.net.cn

Py:   os.getcwd()
来源：http://fq.lnxyls.cn

PHP:  getcwd();
来源：http://ql.lnxyls.cn

JS:   process.cwd()
来源：http://ok.yuntaijiaju.cn

TS:   process.cwd()
来源：http://ek.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://zz.yuexingan06.cn

Go:   os.Getwd()
来源：http://nj.hahajie.cn

Ruby: Dir.pwd
来源：http://up.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://an.jctech888.com.cn

[M05] 设置退出码
来源：http://dp.yuexingan06.cn

Py:   sys.exit(1)
来源：http://ya.yuntaijiaju.cn

PHP:  exit(1);
来源：http://vi.lnxyls.cn

JS:   process.exit(1)
来源：http://uj.gzmigu.cn

TS:   process.exit(1)
来源：http://oh.gzmigu.cn

Java: System.exit(1)
来源：http://vb.nicolike.cn

Go:   os.Exit(1)
来源：http://dp.shxzskj.cn

Ruby: exit 1
来源：http://gi.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fa.chemitech.net.cn

[M06] 向标准错误输出
来源：http://kq.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://an.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sp.shxzskj.cn

JS:   console.error("err")
来源：http://mo.yuntaijiaju.cn

TS:   console.error("err")
来源：http://dw.huanxung.cn

Java: System.err.println("err")
来源：http://vs.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wo.wgjwhj.cn

Ruby: warn "err"
来源：http://ma.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://an.9csxet.cn

[M07] 判断是否为主入口
来源：http://nc.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://wf.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oo.bookmarksfly.cn

JS:   require.main === module
来源：http://tr.lnxyls.cn

TS:   require.main === module
来源：http://ix.9csxet.cn

Java: public static void main(String[] args)
来源：http://ii.huixiangedu.cn

Go:   func main()
来源：http://sn.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cu.hahajie.cn

C#:   static void Main(string[] args)
来源：http://it.hnjuh.cn

[M08] 获取系统与运行时信息
来源：http://xu.jctech888.com.cn

Py:   platform.system();  platform.python_version()
来源：http://vf.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://km.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://ok.haigaiapp.cn

TS:   process.platform;  process.version
来源：http://iu.colortex.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://me.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jc.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://er.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ov.shtwfgs.cn

================================================================================
来源：http://us.colortex.cn

N. 数据结构与算法
来源：http://er.colortex.cn

================================================================================
来源：http://sr.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://mi.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://el.colortex.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kb.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ik.szxytkj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sf.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://op.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://my.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wg.nszjky.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tl.muxihuayi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ih.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://yh.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ks.9csxet.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://us.chemitech.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fg.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zb.lnxyls.cn

Go:   slices.Sort(arr)
来源：http://bl.haigaiapp.cn

Ruby: arr.sort
来源：http://mw.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hm.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://xl.asd995.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://na.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://pt.521024.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xx.muxihuayi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wp.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pn.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hy.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rq.newstarts.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sj.chemitech.net.cn

[N04] 斐波那契数列
来源：http://qg.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bf.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ns.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vf.nicolike.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://as.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://af.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pi.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qv.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nj.yuntaijiaju.cn

[N05] 最大公约数
来源：http://ns.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://zp.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ap.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lx.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rd.huixinmuqiang.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ix.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://km.chemitech.net.cn

Ruby: a.gcd(b)
来源：http://yj.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wq.shxzukj.cn

[N06] 判断回文字符串
来源：http://js.shxzskj.cn

Py:   s == s[::-1]
来源：http://at.asd995.cn

PHP:  $s === strrev($s);
来源：http://mn.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://ux.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://rm.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tc.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://ci.hnjuh.cn

Ruby: s == s.reverse
来源：http://jh.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://et.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://oz.haigaiapp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gt.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bx.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kn.521024.cn

TS:   // 手写 Map<string, number>
来源：http://os.colortex.cn

Java: // 手写 HashMap
来源：http://ik.panjiajie.cn

Go:   // 手写 map[int]int
来源：http://xr.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://oo.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rk.newstarts.cn

[N08] 生成全排列
来源：http://en.yuexingan06.cn

Py:   itertools.permutations(arr)
来源：http://gk.panjiajie.cn

PHP:  // 手写递归交换
来源：http://cm.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://tb.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://jv.asd995.cn

Java: // 手写回溯递归
来源：http://gx.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://eb.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://ac.haigaiapp.cn

C#:   // 手写回溯递归
来源：http://bh.521024.cn

[N09] 栈与队列
来源：http://sd.newstarts.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fn.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rp.jianghongdianzi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ea.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bq.shtwfgs.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aj.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://md.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gb.shtwfgs.cn


<!-- 参考信息 -->