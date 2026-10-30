代发 wailian999

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gjssvlcsa.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/guqqflpgd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gcmpgbcwm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/govdmjoxd.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gkbwhpzjn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghqekaogx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gzjlguhik.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gadfdvbcb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gydtzlzmm.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gsznrednc.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gmpvmdzny.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gaikuzeat.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gcjbfofjk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/glnzttssw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gakhcjify.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwkaxgxbu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gdvgxjgjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gnhsyncol.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ggdztljmq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/guqjhdrds.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gdnhtuphl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gnhjkavqm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gagworlcw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gbsczaafd.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gprclbber.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gqdfdauyb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/givjyfrak.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvhsqyavd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvdrbssag.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/guwzwlmaf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gxwxczokz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gnxtpvpwe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/greaqlexa.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/ghhmhowog.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gydzyieny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjftdnjvy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gfewvtblw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjyyfevbb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gmoklnmjm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gkkqcgmit.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gajocwbdn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gddvcdnqk.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gfoyaktzp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gywjhgaam.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gkuabbdwm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gejzdpyvy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gvmzadupq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gekvsbkzu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/giirhgelz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gvsuewtcj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/glaaqycoe.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gqksikqai.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gpxkbxudz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gjluvsqrw.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gnxmcjdco.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/glcuotyay.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gsycapimu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gamgwsofu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjkiyrftc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/ggfpnpngc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gjnmvnsex.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/ghngovrgm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gpomcliyo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gwojzfavk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gfmdcxkkv.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/ghpugwyyz.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/grvbmezmr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gbsbqgrvu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glgjelnyy.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/giybpmamw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gdzpsoqma.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/ganwjpxlz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gbmkhsqdb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gtzrebfvk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/giflvbymg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/ghrzmowpf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gflxyjseg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gidfwuacj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganarmwji.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gsnfzlgqw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvwvycdmg.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gzmwpzfek.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/ggticnmxp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/goavbxxyo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gpmwwsklf.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gahcjuiai.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gdhzadqzl.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gpklseihh.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gvmrzvupr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/grmpcxupj.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gufgfndlb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gbcdzxowh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gparndxdu.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gkclybits.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzuapdzda.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gzlwktqkd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gcvndsgtf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gieslkrkq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gswoyfpmq.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gurzxqcfz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gxfkjsuex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gqlhgmlhi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gqodnmxtb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdmwsqcxr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gnzpcssxg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gzozjrdyg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gyscnlwhb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gdaylbvhq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gjfdgrzvr.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ghgnnvckl.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gaxdizioh.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghrnwjpeq.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxqpshfud.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/guwzjkswh.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gufauvqel.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/ghnpezqbx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gfwqljbdk.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/glochyles.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtnpnomod.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/ghuhyegoi.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gegycpqmb.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqdvrcest.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gecpevzju.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvylzzzc.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gtmxoqwyd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gucnaseqn.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gujemgiva.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/galkfwkiy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gnewlqlaf.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gzlcmlozq.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghngexzqc.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gdwmnziib.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gbpnvbfbw.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/goqjwrdyy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/grkddwaff.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/guvctnjcd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/ggyylhbrz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gbhesaxwr.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/ghmdwbkzc.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjbsgecvp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gvydivygy.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ggsfykimz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gyvsnbeuk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gzikvwoip.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gtrkldtyw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gsvyjzlhx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gtbksjnhk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gppjlpnwh.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gwpepxmqr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gttnuufuy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gjutqejnh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gsjobireh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/galqoutte.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpihpmjkr.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/ggaahizwn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdxedlcxy.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gruupppts.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnbqibyzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gchjsqqny.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbdphsuyv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gnkfzpzxn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gnkikaqqe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyselwgrz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/ghrhqxyaa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggoulgkiz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gdrtyihlx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmlngllfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gzzpthcsm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gmeqlwmrx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdaiqvtje.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gpsszmyvo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gvqtnouct.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gnkwjxtpq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gypvmgcpf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/goxrohmws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/grjnofhli.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gpbsqbpds.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/ghxpeecng.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gpvqobvij.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/guvrmrrzr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gzrissmma.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gvhymegtg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/ghldylktb.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gvommwjpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gsmlnuxwf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ghmemkxjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gtccierwe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwwxjcgng.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gryytjdjv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gwgigmanx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/giuhovwad.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gctsoewxi.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gdtznpdeg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gsdmqacjv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbsolnrsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqtsdecgh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gwiqwutla.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gnbedcjxh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gkzezelav.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gxacqswtm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/guymorccr.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gfhakwpwe.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gulforpmf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gymabkeww.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gulloyjrc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghqpeglnl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gqimwqkdk.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/glddapyhm.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gunvtcvqq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gtvidercr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gedidtuix.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gelmhnmgr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gzhtiqvlc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gtgterovh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gpblkcgma.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzbsozi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gkfzyfzim.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/glixashdo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gqduugblz.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gtvqrnlwd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gmpnnwykf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gywwbhbwu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gtcyqctwn.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkyhqdgsk.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/giemggebj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbzezfj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gqdgtzkww.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbdduxhob.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpjmvmjxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkebcrmin.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gqdtvsmxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gztyvpukn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gnzdbgzvs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gslxkbdhg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gjunustxz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfqiradjv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/glapaeaxd.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gzakxjbpt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gdnvlcstw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gqjzyizdp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/geimqymxm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gjxuspolw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gyubujsfs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gqdqotwdx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gavxaiflt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gopgmcyto.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/grkmhpbbs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gxkulmoea.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gdkpkwydf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gocmoxctf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gqdicedpb.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gizuxizqc.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ggirjkpvx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gwndkwmul.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gzttolwce.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gzxrcaiyz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/glzqnmiqp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gcfdhkqdo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gnxrjpxar.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gpasetcgr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcdnjtrzz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gprnjzmva.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gpyqvtzru.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gdkrfsbjq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmwohhpha.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gntmthojf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzedymwfi.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gbwlqsfre.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gpttxfjxv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/ghvgkgasz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gocnbzovk.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gclsmkkkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gzoqfhokr.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gumrjeaxp.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gfjhazjek.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gjnzcuxee.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/ggribctts.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gealfubqu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbcktep.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggivgwzdz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gjylxktuf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gvbdmqnxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gqpoxhgkf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gkcuxnkpc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gdalywskv.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gdmmqlsei.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gmxcownxy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gbvqxybzt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gsikjdfqa.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/grtibzyaw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/grxfmwzdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gywifhnjq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gmatputrx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/glqghkrmu.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gdlftepyh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gfdwlfuol.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gshvetlpl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gbfrranmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gyctmcinw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gnzogtkux.sHtML


<!-- 参考信息 -->