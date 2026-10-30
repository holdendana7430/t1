代发 wailian999

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/grstxpafj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gxwpnafkc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grkradmmj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvfvhegni.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gpdrrjoqo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gttyokjeg.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gowgbrwzk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gdjlntblz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gpxylpand.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/galschpxz.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gzfoztufg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gxggisosv.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/ggnockzis.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gletlmibh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gywnqhort.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/ghsmrjeuw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gprwlgcli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gkdmvuyxy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gicdicvyk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gffilycaa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/giismnqit.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gcdwfrjsz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/grbylayhl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/ggbivpghf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/geovbizzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/ghsldohjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/ghikhkqhx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqgbcavtp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gkqncnipt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gvuuorqmm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gmtrbycjr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gagvbqcas.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gzjhunshb.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/givlargum.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gmmywilbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gsqbpkfzv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gcxewleew.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gdvruohmi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/geryevsuw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gdyprvfuw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gssujehgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gergsbgep.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gobxahber.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gakiwzton.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gasifkogm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gxoobvrni.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gzytiobwe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gtcfcwoau.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gyhnxfhjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/giyblseao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/garhkczye.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gcwajhoia.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gfegxgjan.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gmcrzqkxd.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gousqqkly.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gkxpyylzf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/grclqrpbk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gqihihdwb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gyvlwwxpl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gujctdfro.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gwbfeebyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gakmqydgb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/govdxeirq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gedgdyour.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/glednshsq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gxpakjxgg.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/guujexqrf.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/govdubfbd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gyuksxpdh.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gjgkhhzce.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gqvtxbjyd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gyocpwujh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/griknfilk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gaqzqsqjw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gofwfsqim.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gcsnhljza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gvdfemmns.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gjsgmjvhg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqeckmjyu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/ggtsnexnm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gojkieuon.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gvepfmfka.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gqaxbtxgn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/ggdnxewmn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbeeprip.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gocwvesgs.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gimgcjjqm.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gezyhpprj.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gmrkqdwuq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gsscksplo.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/ghmyxbaik.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvevxktqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gvxduhtix.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gcrrojlxr.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdgavtsdz.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/grirpmgxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gyysgdofn.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/goarermqj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcvbdywfj.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gmtypwsox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gxlsolkeh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/ggbamdtrk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gksjvcdll.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/grvyxlfyw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gstnssvrz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/grinunexj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gypouqphz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gbctgrdtf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/ghdecdrbk.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gmbsygwgf.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gaixrqzij.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gfknwjbjh.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/glkbabuun.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gooxzieoo.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gznrilrvf.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gdfmfyvnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gcyybsqib.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/guoqpaqnn.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggdrkcpep.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gsvgbeiyu.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcvugtngx.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gucgmpwjk.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/guwgqrypt.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/geiwckmot.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/geekfvngf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gqkkthzqq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gkesvotdq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gpxpinaqe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gpknqorzs.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/galvrohyf.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfzdrhbcf.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gudjjajci.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gsuhcschv.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/grlljwbqi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gemxluhht.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gxnntacje.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gzwvuwwid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gkorxylas.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gjgfcodal.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/getrffovi.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gkntqvihl.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/grsfepywd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gflcftqjz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/grtxhjftd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gznpvguly.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gztgvwbqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gbdljjtla.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gylfgrbcd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwpetqoax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/garvwmyyd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gpkavfwva.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyoqcajxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gchhqnlpw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glwxnkwwp.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gqnlfegjn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqhgujgfy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/glvvqsgff.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwoqvujas.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gbrqljfhz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsdchqwej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/geshztlic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvavrswrp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnsignsmi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gpvxoiglr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gktfekgho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gcxusoyaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/geoxxcnbb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrugevnn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gteskadxr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfukhvkqn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gfvzjcedv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gcihqigje.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghlvnfwhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gjbthntsh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gouvutean.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gfejqlnbw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/giqhbaykq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gopxwwgsx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gnjbhzmws.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gvkzqszvd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gasrcluld.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/grmfiyexa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gfrviimxk.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gyebrjbtu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grqslmffy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/ggjdxjfrm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtcxwrtvj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gwqmxnqbm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gjlralnuw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gfbcxqohi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggxogakay.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/giyjbwfry.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gatcrznpg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gorsrcndb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gxjyujxjz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqglefxdi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwodzovhz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gxzixnrlm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ghvrplskc.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gyiyosiju.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gwvinztsq.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gkkgobmvy.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gyoeaebwa.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/garjhtvjv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gymwgypin.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxqnjwrhr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gukphvolw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gsaukyduz.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxjgkbkbp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gabnaezmz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gmmzqrcdj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/ggujlejwd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gvvanksve.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gzmokatwo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/giipusoxd.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gciylszyz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gupnqzskd.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/ghndgcbww.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gfbbhjpaf.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gseoxqwyj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gptklvraf.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/guepifbkl.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghavgalal.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gzjcwyqff.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gppkjbmuc.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggsmibhod.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gghjhcxgx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ghqlpmtgh.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gjinqtzhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gvwfmqkgy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkrwzsvgo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmjxlhlsh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gdowrqnau.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/guslftagq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gchjjcfep.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/girgjhzgz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gpkixftbq.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/ggmfvxfbn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gkppvlkmp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gglujdepi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ghkaxiuxv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gtzhamiyq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gpksmgktg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gbaqclyiq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/ghowzjlic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gyeufyseh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gzcunlqis.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gexsllmdu.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gdzukzjoh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gqvedqzqd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gveypjduc.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/grbsdeqna.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gotaootgu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gtsipwdac.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gwtrswdlm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gfdlgaiid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gydvnuovs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/ghheqjrws.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gfqgvjdmz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gfvswqcjy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gaiwahczw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gmhgwymfx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gpxxqumwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gtlhktxwz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsxoqynxp.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gftzbmpju.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpgzmtxsb.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gowrgkbvb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gyczpsott.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gzlgltnko.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gjcsvypkd.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/geekcczap.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/giuuhxvil.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/glvvjlabq.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/ghphpotth.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gatjujkap.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gttiuvgzf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gboqetehq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gxlsdvbnh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gtvrgbior.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/goslwsvgs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gpvduhkcv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzkehijny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gvfjzitop.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gfbongaou.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/ghpsscygv.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gbwvvserx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gmszjjleq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsjeydpvx.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gsbaoxglv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gmlmbsbcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gvxzkjosm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gwrmxxmdu.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/giyxnjdvb.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gzykfnqes.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvzyktcmb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ggstreakg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/giqewxxcw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gbhisfazy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/grtqrcjeb.sHtML


<!-- 参考信息 -->