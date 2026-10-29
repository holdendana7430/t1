代发 wailian999

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gfjeuhdqh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbchykluf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdqmjtbuo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbynanepb.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gtpvaytfk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjxxzlpin.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gkqfqntut.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gpofzgajx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gjqzbsgrv.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdnvtydno.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gpcswhapd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/ggjwttwvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gmlzfytfs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/golvufxdq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gcitqsczz.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gvjccxsmk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gzpkrgqmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gvpckejls.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gvzpzgtnq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gfvazueed.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/giacxddce.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gclxrekpj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gtbnigjav.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gpswarias.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gxlneqjiy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gjfrciprm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gkbrohlxc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gpppzngnd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gcuytvpoz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gfopwrvll.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gvzdaszmg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gplpeplvr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjhsmlk.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gbmejjdon.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gdhwfuyzw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gpditucbx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gxvwfkaee.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gzknjbbih.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/glprjwcfl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/golwwmtkd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/grorumyfc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gtdabjwpc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gorgmgwkj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gthrllvzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gfdxrhznl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gjrdfcvag.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gtceuumpe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gonubleby.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gbdmicjsn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gxofchdpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwlwdhmru.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gqxyxwdeg.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/glgloimnn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/glltygetr.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/genwqxzcs.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqunbipbw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gibwkbkyk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gsbdrbqlr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gptlrgfor.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gwbyypwie.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gjdeuyqge.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gihcopfmz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gcuieqrqt.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gmamhjhya.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gpgyeghwn.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/glfqxnykf.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gmyevyguf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gjjupdylf.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcshjqxmh.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gjntbdxeq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gtvfovnuy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gqbvcdlce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpouhjelx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gaubdysck.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/ggevzjadx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gexizgpzw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gmncwcxhg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnwvvmbjw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjnveycbw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gzqwxdnhr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gesemkojz.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gpjmbjvpw.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gfguakgzl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gacyohtdk.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gkdblivnt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gcdbzwlnh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnhrumtgh.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/grzmfuiws.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gidpbhedf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gxwsrabhk.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gqeztlzsf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gaqntflhe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gwppxmmou.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gbbuszbwn.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gsccmaafp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/givmnexda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfewoehko.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gjnwcmkyy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwuzfiajv.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gohberojq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gwspcjimf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/glbdjjajn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gyqjnwgdd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gimimleti.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gygwwrzdv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gkdebjznt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gebaghkmt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gevgrkrsg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gyydjhhga.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/glauxynpo.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gbfzwobkc.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gswgdmyio.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gopnrwmlc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gjiecdnuz.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gwkyxklyq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gzthelcyj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gcswlxexf.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gurwqdrlu.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxwojpmho.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gupzqhbko.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzzyjcjep.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/guruibuem.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmivnytsc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzltjneuw.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gwngkoimr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gneaxrfhi.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gsbqwubvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gqrdlggfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/ggyzxncec.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gikfykoob.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gkafoekra.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gtxjguqgm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gufintwke.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gzbedazkx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gdtdvgndp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/geuczbpfq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gdfqpituu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gxkmwqsrl.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gdavxelba.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gvpiysnfa.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gqfegqmbl.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/ghkbdcfmx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gvnaoivmf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gpitgfykc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gayhxadgc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gdjpvapct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gmplgyipw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnjqfwpnw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gjjshowlk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gqpmqunvk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gmxhioeec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gxxgdxuca.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gesllgzpn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcclpxjrp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gudorttad.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gplhjhcvv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gbhdncyrz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaavodwee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gtcpnebzn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjjwgplya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gsklabfun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbblbiekj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsgzraxbz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gxgpgsjqq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzawrdzcp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gplmxwjyp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/giattkwhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gfnhzffho.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gjqaumufm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gozcqitau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/grwvmxnvq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gmwqnanim.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/giigbuskv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gxxjrbcpr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gpdcffkgw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gzpeuswyt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gkrtifezi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggrsauswr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbeuepklp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gditrrnth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/grtddnamk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gskgpyzzc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gajnftydf.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gvpcsnflt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gshkanlqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gczkonoue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghxhbipxx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/grluhgtvc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gjovhkzjb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gzvmucbry.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gwwcutewp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gwlafbhfs.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gmwtivapx.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gsastcpey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gljjitigy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gbzrwpiwd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gdjwsexxq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gqbnmvosf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gvkjjxxjm.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gdudhgacx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gewfrlxuv.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gzsddqawp.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkwobgoae.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gorwvtqvq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfjvvjguv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbbajbybd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gwgtyagqa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gvccwacao.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gndkljhzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmxxylmgg.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gtaeoviuz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/grniamncf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gkjthrdjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gzkiidbem.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gizjjhxhp.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gokwyhphl.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gmjxfwcma.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gbxnudgtd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gcoclkzaq.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gixgvsnqo.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gzioctcud.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gdyfcwjzc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggdebgtpi.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnfaejxrh.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grrqrvafv.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggstquyfg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gozzazkcr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtohrophl.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gkmdroqtr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gxsskgwxj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gdaejpcev.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/godxnypwi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gpxpucucs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/ggietqheo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcgbudyvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glietqhnr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gyhmcemxd.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gtdblnqfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gisbmhyoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gmgaxcrxw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gqppiaqnk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gyietvttx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gyiuyddmg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gemochkbs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gywcosqsr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gpclrcliz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gcdufrjfr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/guraohrox.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gmereljqy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gzbzwpaqp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ggbiruqnf.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gevtfwchh.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpemjoidh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gaevgaqms.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/givpdmjpe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gwbngekcw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gjfauogux.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gkoqqirxb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghdtkjsij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gnwrozwni.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gsgzraeaa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gangvxous.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/guhvefsoc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gpviftgur.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gryzeymgt.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gimafduom.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsbzigvmy.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gzpexvqxv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/goktkkxkp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/ghspcfunt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gwaawnyej.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gssfmsrkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gwziksqnp.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/ggdpesgmr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gjbaqotll.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gybsaqdlk.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gyxxrtsms.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/grfwpdmhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gzcsfrrvn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gregmrlxa.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gsuerdwgk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gumvieolw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gzpfwcawz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gelqtxnrt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gihndvzcp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gvtlpkfyy.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gxnxjxkkv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gsmqufjta.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grtdrvxis.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gbvvyzjxt.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gntfaficr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gqxngjoir.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gtskyxmvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glkqpnzfa.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gmjwqbpvx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gqvkgvxhm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gpqkbxbqj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gockmsohj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gowgesyfe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ghrmjbaar.sHtML


<!-- 参考信息 -->