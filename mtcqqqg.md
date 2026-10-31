代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xo.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wh.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dg.panjiajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vw.jianghongdianzi.cn

================================================================================
来源：http://tf.panjiajie.cn

K. JSON 与序列化
来源：http://pc.newstarts.cn

================================================================================
来源：http://oe.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://uh.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nh.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tu.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://py.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://sq.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://es.521024.cn

Go:   json.Marshal(obj)
来源：http://li.newstarts.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eg.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hy.huanxung.cn

[K02] JSON 字符串转对象
来源：http://zh.shtwfgs.cn

Py:   json.loads(s)
来源：http://ok.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rw.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://ju.szxytkj.cn

TS:   JSON.parse(s)
来源：http://gp.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rs.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://uc.newstarts.cn

Ruby: JSON.parse(s)
来源：http://fe.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vg.muxihuayi.cn

[K03] JSON 美化输出（带缩进）
来源：http://pw.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sf.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ae.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sj.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://na.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yu.muxihuayi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lo.asd995.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zk.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hm.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://hk.szxytkj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ub.bjjhwx.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vq.jianghongdianzi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://by.521024.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pz.jianghongdianzi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cp.panjiajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ua.newstarts.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jy.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wh.shxzskj.cn

[K05] 深拷贝对象
来源：http://re.shxzukj.cn

Py:   copy.deepcopy(obj)
来源：http://qy.haigaiapp.cn

PHP:  unserialize(serialize($obj));
来源：http://dd.yuntaijiaju.cn

JS:   structuredClone(obj)
来源：http://ao.asd995.cn

TS:   structuredClone(obj)
来源：http://vj.wgjwhj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uq.haigaiapp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://il.muxihuayi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hd.shxzukj.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zl.521024.cn

[K06] 解析 URL 查询串
来源：http://ea.szsharing.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fa.bookmarksfly.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jt.shtwfgs.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qb.9csxet.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uo.yuexingan06.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://li.haigaiapp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ww.shxzskj.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ch.yuexingan06.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kn.jianghongdianzi.cn

[K07] 进制转换
来源：http://gq.yuntaijiaju.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wu.asd995.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gw.bookmarksfly.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sy.521024.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://af.panjiajie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oj.huixinmuqiang.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ag.lnxyls.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sh.lnxyls.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wq.shtwfgs.cn

[K08] 二进制序列化（非 JSON）
来源：http://kr.panjiajie.cn

Py:   pickle.dumps(obj)
来源：http://wb.bookmarksfly.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bb.jctech888.com.cn

JS:   v8.serialize(obj)        // Node
来源：http://cg.haigaiapp.cn

TS:   v8.serialize(obj)        // Node
来源：http://fd.panjiajie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gp.gzmigu.cn

Go:   encoding/gob
来源：http://me.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://yk.haigaiapp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ub.huanxung.cn

================================================================================
来源：http://hh.9csxet.cn

L. 网络请求
来源：http://vl.shxzukj.cn

================================================================================
来源：http://ku.huixiangedu.cn

[L01] 发送 GET 请求
来源：http://zz.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yh.hahajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zu.9csxet.cn

JS:   await fetch(url)
来源：http://dn.muxihuayi.cn

TS:   await fetch(url)
来源：http://db.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://av.asd995.cn

Go:   resp, err := http.Get(url)
来源：http://rw.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://at.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yn.asd995.cn

[L02] 发送 POST JSON
来源：http://ew.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://up.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pr.yuexingan06.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yf.wgjwhj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eg.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ad.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gb.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fs.9csxet.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sv.shxzskj.cn

[L03] 设置自定义请求头
来源：http://np.bookmarksfly.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ae.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sv.huanxung.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nr.huixinmuqiang.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zs.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lr.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ax.shxzskj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xw.gzmigu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xp.shxzskj.cn

[L04] 设置超时
来源：http://dd.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://dw.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jd.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rp.szxytkj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cp.bookmarksfly.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cl.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fj.9csxet.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pa.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rl.szxytkj.cn

[L05] 上传文件（multipart）
来源：http://fs.chemitech.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zy.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ps.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uo.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yo.9csxet.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dt.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rh.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bg.szsharing.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://us.521024.cn

[L06] 解析响应为 JSON
来源：http://wj.colortex.cn

Py:   resp.json()
来源：http://oq.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://gg.bookmarksfly.cn

JS:   await resp.json()
来源：http://id.lnxyls.cn

TS:   await resp.json()
来源：http://kn.hnjuh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kj.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fr.haigaiapp.cn

Ruby: JSON.parse(resp.body)
来源：http://ls.haigaiapp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mq.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://ks.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xy.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ls.jctech888.com.cn

JS:   resp.ok;  resp.status
来源：http://xp.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://ma.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://gz.lnxyls.cn

Go:   resp.StatusCode
来源：http://pf.jianghongdianzi.cn

Ruby: resp.code.to_i
来源：http://vg.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ms.chemitech.net.cn

[L08] 并发请求多个地址
来源：http://iy.hahajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dc.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://cc.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ma.haigaiapp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cm.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mt.chemitech.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yr.yuexingan06.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sw.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xk.huixiangedu.cn

================================================================================
来源：http://xf.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://st.lnxyls.cn

================================================================================
来源：http://rv.panjiajie.cn

[M01] 读取命令行参数
来源：http://ax.lnxyls.cn

Py:   sys.argv[1:]
来源：http://gi.nszjky.cn

PHP:  $argv;  $argc;
来源：http://kq.yuntaijiaju.cn

JS:   process.argv.slice(2)
来源：http://my.muxihuayi.cn

TS:   process.argv.slice(2)
来源：http://ha.colortex.cn

Java: args 数组（main 方法参数）
来源：http://ih.huanxung.cn

Go:   os.Args[1:]
来源：http://yt.haigaiapp.cn

Ruby: ARGV
来源：http://nr.bookmarksfly.cn

C#:   args 数组（Main 方法参数）
来源：http://mp.wgjwhj.cn

[M02] 读取环境变量
来源：http://ff.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://wq.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ta.haigaiapp.cn

JS:   process.env.HOME
来源：http://tx.newstarts.cn

TS:   process.env.HOME
来源：http://ob.gzmigu.cn

Java: System.getenv("HOME")
来源：http://xt.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lw.521024.cn

Ruby: ENV["HOME"]
来源：http://gz.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zt.nicolike.cn

[M03] 执行外部命令
来源：http://az.521024.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xp.szsharing.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yp.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kn.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://en.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://un.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ff.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ji.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://xv.shxzskj.cn

[M04] 获取当前工作目录
来源：http://gd.wgjwhj.cn

Py:   os.getcwd()
来源：http://nx.shxzskj.cn

PHP:  getcwd();
来源：http://dw.asd995.cn

JS:   process.cwd()
来源：http://px.hahajie.cn

TS:   process.cwd()
来源：http://py.lnxyls.cn

Java: Path.of("").toAbsolutePath()
来源：http://qp.shxzskj.cn

Go:   os.Getwd()
来源：http://gm.szxytkj.cn

Ruby: Dir.pwd
来源：http://mb.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wn.szxytkj.cn

[M05] 设置退出码
来源：http://mn.9csxet.cn

Py:   sys.exit(1)
来源：http://de.yuexingan06.cn

PHP:  exit(1);
来源：http://rs.bookmarksfly.cn

JS:   process.exit(1)
来源：http://gx.huanxung.cn

TS:   process.exit(1)
来源：http://gr.9csxet.cn

Java: System.exit(1)
来源：http://ys.asd995.cn

Go:   os.Exit(1)
来源：http://lu.huixiangedu.cn

Ruby: exit 1
来源：http://ta.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nl.hahajie.cn

[M06] 向标准错误输出
来源：http://fa.colortex.cn

Py:   print("err", file=sys.stderr)
来源：http://wi.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fb.yuntaijiaju.cn

JS:   console.error("err")
来源：http://gd.muxihuayi.cn

TS:   console.error("err")
来源：http://io.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://so.muxihuayi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fw.jctech888.com.cn

Ruby: warn "err"
来源：http://my.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://yb.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://dq.szsharing.cn

Py:   if __name__ == "__main__":
来源：http://rk.gzmigu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hc.panjiajie.cn

JS:   require.main === module
来源：http://ze.huixinmuqiang.cn

TS:   require.main === module
来源：http://os.9csxet.cn

Java: public static void main(String[] args)
来源：http://tv.jianghongdianzi.cn

Go:   func main()
来源：http://wk.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yu.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ug.colortex.cn

[M08] 获取系统与运行时信息
来源：http://ar.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://rc.yuntaijiaju.cn

PHP:  PHP_OS;  phpversion();
来源：http://qx.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://ge.lnxyls.cn

TS:   process.platform;  process.version
来源：http://om.nszjky.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mf.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gz.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qi.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ph.yuexingan06.cn

================================================================================
来源：http://av.newstarts.cn

N. 数据结构与算法
来源：http://do.hnjuh.cn

================================================================================
来源：http://be.bjjhwx.cn

[N01] 二分查找（有序数组）
来源：http://fv.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jz.szsharing.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uk.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mw.panjiajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bt.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fm.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://zf.shtwfgs.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nl.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gq.hnjuh.cn

[N02] 排序（工程实践用内置实现）
来源：http://cb.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.bjjhwx.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zw.bookmarksfly.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://io.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gt.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lc.asd995.cn

Go:   slices.Sort(arr)
来源：http://fm.jianghongdianzi.cn

Ruby: arr.sort
来源：http://jy.haigaiapp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rz.jctech888.com.cn

[N03] 快速排序（分治示例）
来源：http://la.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://na.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://vw.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kv.9csxet.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vd.bookmarksfly.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ki.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://os.bjjhwx.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zc.huanxung.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uj.jctech888.com.cn

[N04] 斐波那契数列
来源：http://cg.nicolike.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cn.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pe.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://du.gzmigu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yv.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yr.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ea.9csxet.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mp.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lg.colortex.cn

[N05] 最大公约数
来源：http://af.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://vs.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://im.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wj.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ec.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xc.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eq.nszjky.cn

Ruby: a.gcd(b)
来源：http://tn.huanxung.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ka.yuexingan06.cn

[N06] 判断回文字符串
来源：http://if.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://vi.bookmarksfly.cn

PHP:  $s === strrev($s);
来源：http://pr.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://ur.hahajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ro.newstarts.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sx.hahajie.cn

Go:   // 双指针从两端比较
来源：http://fo.shtwfgs.cn

Ruby: s == s.reverse
来源：http://as.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ol.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://cq.asd995.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zl.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yr.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rg.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://ju.shtwfgs.cn

Java: // 手写 HashMap
来源：http://tu.asd995.cn

Go:   // 手写 map[int]int
来源：http://ie.shtwfgs.cn

Ruby: // 手写 Hash
来源：http://ug.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ns.9csxet.cn

[N08] 生成全排列
来源：http://zk.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://gi.huixiangedu.cn

PHP:  // 手写递归交换
来源：http://yu.521024.cn

JS:   // 手写回溯递归
来源：http://yx.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://do.hnjuh.cn


<!-- 参考信息 -->