代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/glwfbxsxi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkysslswt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gvyhikrfp.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gtqdwdlxm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gfpzyaqhk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ggzodchaq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gicjxqxyl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gwyzqxwtv.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/geqfsswlt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gqypbhtau.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdpuvvqec.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnjsprplv.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gvfmvinbz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggynppaap.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gdokecjao.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/guwaqkrim.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/grvvgsnwv.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/giowdvfhn.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gcfhfbdya.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gmrlfohpx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gepuglirf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gbtwodxgf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/glelxivew.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gikyqzbhh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gcweykyjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gvufoexio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gaddhvscz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gzhnsvzlp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gmxpzfnkt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gqsncejwy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gjrkatsfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/ghybgwvck.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gmgzvxgoc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gzzrttefx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghnatehzj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gmhajofpu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/giytcfttx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gxwrxmxjx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gkfnaazue.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gfltyoyjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gcmjwqkbv.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gtqejjlhz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/grgpetntx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/guawobsuz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gnsjvnejt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/ggqbudrjs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gtszqmohe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gcquvsvxa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gemdiwpyt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gkctycagy.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gmhpxoenm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gkxczdelw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gjjmsrokn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gyhaemyuc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gwddibeme.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gzfjnhjls.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gpejoioll.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gtpnuqvrc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggjumywil.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gzslaxhdn.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggvphpczq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gathgadsd.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/ghbplzdjw.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/grhdlmloe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gzcjxkltl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gqkfhrumq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gewfcbaip.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/glmqgkusg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gpuudktbp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gonzslxhg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gbxertukw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gbuamfvzy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gfamhgwpm.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grgwkscdd.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gfsfitzqb.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gdkqmtbis.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gotxwdlsf.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gomcotohg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gznnrolkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gdqizddou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwavbcwwk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gcqcyuzbm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gviskibnl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gbojrxusn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gdufjgjep.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gooeaunii.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/govqkijiu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gcinkhspm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gysedwvmq.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gbadvnncw.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gnfnvckjr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gtaxsdoyg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbnvbiinq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqaixruvb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/goqpiyean.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/giczugkxh.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gjcgwsxgo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gkjfeqftj.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/glzltckwc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmplyaobd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gueclvcui.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/guwomfgtc.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gyzzdrrth.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gplnugexn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gykksdawm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gcszyftwa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gczisztno.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/ggcieunje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gppfzswhv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gogkbrpwe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/ghykdfjef.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gdtgwqxmr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/giqvoqote.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/grggdgete.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gpfcmpnzk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gcmjowqdo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gdwspccul.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gmpetdcww.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gpuxqcpyj.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gsoutormo.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gtvswzlqi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gffubdyjn.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grgzgcamb.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gnqhpzmij.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gbzpinezb.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gxqiyohth.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gnsxixpbw.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhzjlrpm.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gesbzrqat.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfxdiwqfr.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gcodfauct.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glbxbkgup.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gxegzyuwt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gxxxadfnf.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gswedfjac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gerzucgxa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gqdwrlfzc.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gseieuetw.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gqmioqdpn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gocjmoare.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gwbuztmfn.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gynpytfzu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gxurpigjs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdbqpojdw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/glamsfuzz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/garzjyqqr.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/guergiknr.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/glztvvaui.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gkokofpco.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gisbtjjjb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ghwququle.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gxdltjice.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gjmqtywnl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gajwulghn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/giuvjvwbi.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/guaexqwdt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gpkhcuprb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/ghbwuxopo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gafrrsezo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gobibuesw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gbcfpeazs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gelotlynp.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gpuuubwwu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gctypfrjv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gsgpkrbsi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gyppwjwdo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtkcwbbvj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxayuhptt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjdgziqea.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdznnsrep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxhefsiec.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gtroucytt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggumhlrtm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/ggmhaqgwl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gtawjopds.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gtkburaxq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gmssvnqpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ghawsoupo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gtuxksowc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gntnriirm.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gapcrphyv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcprsnqw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/ghejuhahr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gadnlniwr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gbaximlhh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtofoplgb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gppwiulzy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gagianytw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gdiddkoit.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gqzqghgut.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzurzmsjh.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gnqlvsjbz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/garkxypar.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gwiwserly.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gpvdgatwa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjnjhqufa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gumeomxvr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ghvwygnkq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghgktbblq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gmpzmmisg.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/govhfxrci.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/glogjrxqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqqvcuxl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gstulwuks.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gazvonapn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gmckqhsjf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gpfebapzi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gdrkbfdrl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gilliedyw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gayywcisp.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gljsvlxac.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghkuoddrq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbwzqzcnz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gbfmqpfhd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gcuaqpwqh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gdugdieoi.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/glclxczql.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gwjqjibtu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gdsfiukua.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gcbwkxmtl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gehzcqfov.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/ginarxalx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gwaqdxypu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/glhyhmabe.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnbjtqysn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gjzukjheh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gqonukcew.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gdjwgowob.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyvekbfln.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gduektcvr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdxlqmigo.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnfsjskkj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gryuyfkze.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/goinmncto.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gvfgbdlgm.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcipmmjyd.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gsegtrncu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gkzbgahxs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghckyaaai.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdejfiysx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gmodaetjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gfafuorkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/ggqhiomge.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwlifachm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gclngkygw.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gflrcdkri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gjjlcomgf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gcbscobeq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gxrjfjcsz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gwyiytiez.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gykuetlhq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gogtvhllj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/grafsajjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/glmdgixim.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/guqwzrwbd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/ghetxikuu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gcuphuzie.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gvigzmxon.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gkebugflv.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmmhpyxyr.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ggtblpjvf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gsddnlgno.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grwfrsqfe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gwjsruajb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gklbwiupc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gspwdhvpy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjftvtyei.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gcdvbbsna.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ghnsidydp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gkjdtryha.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gxcvlzajc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gtxdqguje.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gprfsexdj.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbwzfcjuk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsppviy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gyfhmdrsl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ghforntdo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/ghjveiray.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/guutcgixh.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gfbrakzcx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gzftoaclv.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjhwynzjn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gwynakqai.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gdbjiwlzk.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gwziflndv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gazbedmwj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gbrooktbe.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnezbotdz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gjrlifapi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gczasiixt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/ggepstski.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ggrnphscv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/grgoxsscv.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gotcdcrda.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnjtmylde.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gaqcekewr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gboapurbq.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ggokxrnkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gtbswwixv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gxralnyxz.sHtML


<!-- 参考信息 -->