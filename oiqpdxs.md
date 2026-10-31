代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ks.newstarts.cn

Go:   json.Marshal(obj)
来源：http://bw.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uu.wgjwhj.cn

[K02] JSON 字符串转对象
来源：http://tz.haigaiapp.cn

Py:   json.loads(s)
来源：http://xt.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wo.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://ve.chemitech.net.cn

TS:   JSON.parse(s)
来源：http://wq.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qv.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://lj.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://ww.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zl.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://bz.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wq.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kz.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wr.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rw.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dc.szsharing.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ic.nicolike.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zm.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vd.nicolike.cn

[K04] 读取 JSON 文件
来源：http://lf.bookmarksfly.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jx.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tf.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xi.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oz.asd995.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vr.colortex.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gz.jianghongdianzi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mk.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pt.huixiangedu.cn

[K05] 深拷贝对象
来源：http://eo.bjjhwx.cn

Py:   copy.deepcopy(obj)
来源：http://xu.szxytkj.cn

PHP:  unserialize(serialize($obj));
来源：http://zh.bjjhwx.cn

JS:   structuredClone(obj)
来源：http://dn.9csxet.cn

TS:   structuredClone(obj)
来源：http://cc.szsharing.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ex.shxzskj.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bo.521024.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lv.hahajie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://to.huanxung.cn

[K06] 解析 URL 查询串
来源：http://nr.nszjky.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kv.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yv.huixiangedu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qj.panjiajie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cn.huixinmuqiang.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ho.chemitech.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ov.521024.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ji.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zn.521024.cn

[K07] 进制转换
来源：http://nw.jctech888.com.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mo.yuntaijiaju.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vp.lnxyls.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kr.9csxet.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qs.gzmigu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dr.shxzskj.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kc.haigaiapp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vu.huixiangedu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ru.shxzukj.cn

[K08] 二进制序列化（非 JSON）
来源：http://td.muxihuayi.cn

Py:   pickle.dumps(obj)
来源：http://uu.huanxung.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mn.wgjwhj.cn

JS:   v8.serialize(obj)        // Node
来源：http://hk.bjjhwx.cn

TS:   v8.serialize(obj)        // Node
来源：http://eo.newstarts.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bw.haigaiapp.cn

Go:   encoding/gob
来源：http://cg.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://ug.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tu.hahajie.cn

================================================================================
来源：http://fd.shxzukj.cn

L. 网络请求
来源：http://no.shxzskj.cn

================================================================================
来源：http://hp.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://dl.bookmarksfly.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://li.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rt.gzmigu.cn

JS:   await fetch(url)
来源：http://gs.jctech888.com.cn

TS:   await fetch(url)
来源：http://pg.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bz.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://io.nszjky.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rc.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tr.newstarts.cn

[L02] 发送 POST JSON
来源：http://rn.521024.cn

Py:   requests.post(url, json={"a": 1})
来源：http://as.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qn.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ym.9csxet.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sr.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ao.shtwfgs.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eg.szsharing.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hk.muxihuayi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oo.huanxung.cn

[L03] 设置自定义请求头
来源：http://dm.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xs.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sc.nicolike.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xd.nicolike.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://my.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jx.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sc.9csxet.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://at.muxihuayi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ew.bjjhwx.cn

[L04] 设置超时
来源：http://rd.szxytkj.cn

Py:   requests.get(url, timeout=5)
来源：http://gu.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qb.bookmarksfly.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jv.panjiajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tx.521024.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fr.nszjky.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://im.lnxyls.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bn.szxytkj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kn.nicolike.cn

[L05] 上传文件（multipart）
来源：http://tt.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fl.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rp.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uq.shxzukj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ag.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zi.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nh.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tq.shxzskj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ie.shxzukj.cn

[L06] 解析响应为 JSON
来源：http://lf.shxzukj.cn

Py:   resp.json()
来源：http://jg.colortex.cn

PHP:  json_decode($body, true);
来源：http://ut.hahajie.cn

JS:   await resp.json()
来源：http://xk.lnxyls.cn

TS:   await resp.json()
来源：http://cw.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qy.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tp.szsharing.cn

Ruby: JSON.parse(resp.body)
来源：http://wq.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wb.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://kp.wgjwhj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eu.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ld.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://lv.huanxung.cn

TS:   resp.ok;  resp.status
来源：http://vs.hahajie.cn

Java: resp.statusCode()
来源：http://wf.newstarts.cn

Go:   resp.StatusCode
来源：http://mq.colortex.cn

Ruby: resp.code.to_i
来源：http://hh.yuexingan06.cn

C#:   (int)resp.StatusCode
来源：http://at.shxzskj.cn

[L08] 并发请求多个地址
来源：http://va.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oq.haigaiapp.cn

PHP:  curl_multi_init() 系列
来源：http://pj.chemitech.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ww.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ah.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cw.chemitech.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fr.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dn.hnjuh.cn

================================================================================
来源：http://ag.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://vt.bjjhwx.cn

================================================================================
来源：http://zv.huixinmuqiang.cn

[M01] 读取命令行参数
来源：http://sd.nszjky.cn

Py:   sys.argv[1:]
来源：http://oz.muxihuayi.cn

PHP:  $argv;  $argc;
来源：http://ez.521024.cn

JS:   process.argv.slice(2)
来源：http://wi.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://zu.521024.cn

Java: args 数组（main 方法参数）
来源：http://kt.huanxung.cn

Go:   os.Args[1:]
来源：http://xe.hnjuh.cn

Ruby: ARGV
来源：http://yo.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://uf.huanxung.cn

[M02] 读取环境变量
来源：http://yq.521024.cn

Py:   os.environ.get("HOME")
来源：http://jk.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fe.jctech888.com.cn

JS:   process.env.HOME
来源：http://mj.haigaiapp.cn

TS:   process.env.HOME
来源：http://wm.huixiangedu.cn

Java: System.getenv("HOME")
来源：http://uk.haigaiapp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gy.hahajie.cn

Ruby: ENV["HOME"]
来源：http://vw.lnxyls.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gm.shtwfgs.cn

[M03] 执行外部命令
来源：http://ay.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rb.hnjuh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hx.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dv.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sk.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mm.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ee.colortex.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zv.szxytkj.cn

C#:   Process.Start("ls", "-l");
来源：http://gz.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://gr.shxzukj.cn

Py:   os.getcwd()
来源：http://pw.lnxyls.cn

PHP:  getcwd();
来源：http://sx.colortex.cn

JS:   process.cwd()
来源：http://ag.shxzukj.cn

TS:   process.cwd()
来源：http://ue.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://ym.szsharing.cn

Go:   os.Getwd()
来源：http://iu.bjjhwx.cn

Ruby: Dir.pwd
来源：http://me.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cg.newstarts.cn

[M05] 设置退出码
来源：http://zs.bookmarksfly.cn

Py:   sys.exit(1)
来源：http://ut.haigaiapp.cn

PHP:  exit(1);
来源：http://ar.bjjhwx.cn

JS:   process.exit(1)
来源：http://vv.9csxet.cn

TS:   process.exit(1)
来源：http://nw.panjiajie.cn

Java: System.exit(1)
来源：http://gm.lnxyls.cn

Go:   os.Exit(1)
来源：http://cs.hnjuh.cn

Ruby: exit 1
来源：http://ru.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mq.muxihuayi.cn

[M06] 向标准错误输出
来源：http://go.nszjky.cn

Py:   print("err", file=sys.stderr)
来源：http://in.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jf.szxytkj.cn

JS:   console.error("err")
来源：http://jg.wgjwhj.cn

TS:   console.error("err")
来源：http://ml.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://zl.gzmigu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://km.wgjwhj.cn

Ruby: warn "err"
来源：http://jj.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://sz.huixinmuqiang.cn

[M07] 判断是否为主入口
来源：http://ga.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://hr.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xb.shtwfgs.cn

JS:   require.main === module
来源：http://oq.bjjhwx.cn

TS:   require.main === module
来源：http://tj.szxytkj.cn

Java: public static void main(String[] args)
来源：http://ix.haigaiapp.cn

Go:   func main()
来源：http://lk.wgjwhj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eq.newstarts.cn

C#:   static void Main(string[] args)
来源：http://kw.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://me.gzmigu.cn

Py:   platform.system();  platform.python_version()
来源：http://kz.muxihuayi.cn

PHP:  PHP_OS;  phpversion();
来源：http://gq.lnxyls.cn

JS:   process.platform;  process.version
来源：http://hc.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://ee.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ow.521024.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lq.szxytkj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bg.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xi.shtwfgs.cn

================================================================================
来源：http://yz.yuexingan06.cn

N. 数据结构与算法
来源：http://hl.9csxet.cn

================================================================================
来源：http://ul.huixinmuqiang.cn

[N01] 二分查找（有序数组）
来源：http://yk.9csxet.cn

Py:   bisect.bisect_left(arr, x)
来源：http://my.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ot.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://la.huanxung.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://po.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fe.shtwfgs.cn

Go:   sort.SearchInts(arr, x)
来源：http://om.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://re.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rj.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://fv.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pe.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nn.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sw.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ln.shtwfgs.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xk.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://ua.hnjuh.cn

Ruby: arr.sort
来源：http://qy.szsharing.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://om.asd995.cn

[N03] 快速排序（分治示例）
来源：http://na.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://da.szsharing.cn

PHP:  // 递归实现，或用 usort
来源：http://wg.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bs.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bp.jianghongdianzi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ur.gzmigu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ka.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ya.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://er.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://pz.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ot.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ly.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mi.huixinmuqiang.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ts.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tt.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fg.szsharing.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xb.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qr.hnjuh.cn

[N05] 最大公约数
来源：http://hu.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://jv.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kc.yuexingan06.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eu.yuexingan06.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kk.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://an.nszjky.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oo.gzmigu.cn

Ruby: a.gcd(b)
来源：http://yb.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lt.shtwfgs.cn

[N06] 判断回文字符串
来源：http://gr.bjjhwx.cn

Py:   s == s[::-1]
来源：http://gx.shxzskj.cn

PHP:  $s === strrev($s);
来源：http://wk.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://rm.huixinmuqiang.cn

TS:   s === [...s].reverse().join("")
来源：http://hv.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wa.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://tr.newstarts.cn

Ruby: s == s.reverse
来源：http://gx.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zd.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://ag.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ww.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hu.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bx.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://si.shxzukj.cn

Java: // 手写 HashMap
来源：http://xr.9csxet.cn

Go:   // 手写 map[int]int
来源：http://aw.shxzskj.cn

Ruby: // 手写 Hash
来源：http://cc.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://az.wgjwhj.cn

[N08] 生成全排列
来源：http://gx.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://mb.shxzukj.cn

PHP:  // 手写递归交换
来源：http://qb.asd995.cn

JS:   // 手写回溯递归
来源：http://fe.521024.cn

TS:   // 手写回溯递归
来源：http://gq.shxzukj.cn

Java: // 手写回溯递归
来源：http://aj.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://bo.521024.cn

Ruby: arr.permutation.to_a
来源：http://tf.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://df.hnjuh.cn

[N09] 栈与队列
来源：http://xs.colortex.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lq.jctech888.com.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ne.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://or.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mq.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sg.yuexingan06.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ac.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mr.huixinmuqiang.cn


<!-- 参考信息 -->