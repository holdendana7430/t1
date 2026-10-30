代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gribxbnrq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghdikzmoc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gdxespgpv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gnkndmiod.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gasfmriby.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtecgmwhx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/geloawqry.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gijdqebbv.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gaayfbxbu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gukifjhcm.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gcwrkyygr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gerhssauj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/giavozohi.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gzfyowros.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gvwnriymb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gjypufzwx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gtibaskjr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gzwmxfthj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gjmjfxqke.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/geypwjhfi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gmbclvjuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gqofsheoz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gcfxfbkwl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/grmlwepxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gheixirzn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gipjzxvyo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gkfrbypnd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gmcxhljrp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gptdkvjrk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gzayzlvay.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gejsbkylz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gybngdapb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gqwfesnvw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gkxnvhzhe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ghocgcqmc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gewsdttkl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gofvddvkm.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gcfuixucn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gzazfpzdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/ggqnesasr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gnfyyzzvy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gaomndvwz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gfbwbjtvz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gczunnvtq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gzeelbwtv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/ghqrxelpj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gwjsalwxg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/galrlgpnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gomepecvv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/guozedivy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/garnomcrh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gakbuqaga.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gprcfhkoo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gkfacgcim.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/givfurhma.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtbawbehn.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/grruwpuib.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/grintbfgc.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gqlieodjj.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ggsbxywsx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gespduqsd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gvertnnun.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gjhnksjrw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gknmkayxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnjkcudaf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gybnvgqyf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gmbpcmguv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/ghmkmohvu.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gdiuvjcxs.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gppflcsnp.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gwjbszxaf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gsymjrnnz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/ggxmiuijx.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/ghxllvtbw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gckyetnxh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gikrrsvzh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gwmodtlzl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnjcgqjic.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gfaexgllh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gacrhghak.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gjdkcjzoi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gwtxzmxnb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnrqukulq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gmuapblhq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghzrxiqsn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggnjriqib.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gvboxhuvg.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gktmlkdio.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gnitkuwht.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/ggpujdzxf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gmbnxbvyc.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gnzvkytcp.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gubdfdtty.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzdmszeau.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gueuftomk.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gbkcimtem.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/guzcmgtyd.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gnfifyatx.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gairlxnlt.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gndsuxqtt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gouqcdpoo.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gtcluiqdv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gapomcnsc.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gxbczulrx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gbtdxxcpd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/ghkebahhe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/goxchxakt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gzqzmndqf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gkaxuolpg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ghcjkfukv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gztaovdva.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gpddmvovw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/glktbujhx.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/giemvmdvl.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gzcvjdqvb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gcrfgxxik.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gkoizmfra.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gjmcczzlt.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gmcempdoy.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gwkfgfcwv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/giftjhhqk.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gkrqkgrfq.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnwozpqlx.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/ggpuvrdig.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grmkgjfbv.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gadxjabol.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gprztjjxq.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsczaojjw.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gizhdcsqc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gwmmehzck.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gkefzlyuj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gcianaias.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/geexncysl.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gauiuzaqu.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/grxlxglen.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gchblxfqr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/glfkdoxqq.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gupfxzbja.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gaczevtam.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gfctayxzu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gggkkbbqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gozmnzirm.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gdneoyutx.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glecwsmks.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/goygtcokk.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gnulpgmfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ggfdfrwkm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/grvsgwmml.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/guzipvfxi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gsveqtpyj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gzfwajyfp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/giiomszcg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gcnxhfhfl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gwpupnktq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gjqcqvres.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gmnebukmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gisavizkz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtjsgqpzb.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gdfioqkxu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gitbrzzkm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/ggcbuzdlw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbnjzuznk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gjeadhpmf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gcmsctvsf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gyxwdvdsv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggzeowjny.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/garmiiwxl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gmguypgeo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnuzxolqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/girbkjwjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ganouzitn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/ghyxhzint.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcujylayv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/garcpmqrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gnfrwlxoz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gnpbomola.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/goaugtmnj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gyigksumz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gwffmsunx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gwdffymjs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gglrtssxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gtnhxbjgx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ghwjkxlwp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/glagijojg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/ggezpfvmx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/govhoiyju.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gifevvgyc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gxmvjuvjz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gfsbxmcol.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwqzxgmqa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbnsxgego.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcricnexj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzkwjghvk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gmlagpdve.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnaqgxvsa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvkzzrhek.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/ghthsfdxt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gpjxlnefb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gmqnbioft.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcqxqwpwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/goqoahwgr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gxgegdktc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gsokzgbwp.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gthkrjffu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/grqowfswj.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gcrjfgawc.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gngzcwpsa.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gntlvocqc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/geryvqbrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gsewhosmw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gypwvgsos.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gkzpyvour.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gxrlabdut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gcgrbjgje.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gvvtxelra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gjgpfbvcq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gkprawkkz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gewudjbzr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gxkxyahae.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gvftgxdsp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gidgyulkg.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gnpbsbkeg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gsrvqhksy.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/glejsoexa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gunbhouex.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/ghkqitbfu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gevrumudr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkwxhhtdg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkpvdxdjg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gumwbdeek.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gcbgwatde.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsexhuqat.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gbwfjqbch.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gpmemgioh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtwwvihyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ggmtsunpq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gdokawmxl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/ggftufmrb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gzirgmdxv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gljurpmnc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gtfgkbvab.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/glrbdtcxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gazzyclan.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gqfiigwex.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/guaxhcktk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gefitzxdd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gejhqbinv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gmedjkdce.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gdrrohzhp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/glucbzwgh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gyiwukbix.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gijbkdpmu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gcewiskub.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gwggbnxjy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gjgdbdyvf.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gphjbnxyx.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gskidbfex.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gmlmxjwuk.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/grleyqdcl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gohawgyyu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gfcuidkot.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gsboldfuj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvmywlxga.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/glsxhjejb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gxhmikmgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/giabgscpt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gsfyzbhom.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gbysakvdy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmvalysfy.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gftfdyuye.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwwnravsg.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gfbdtizwl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gtrdtvvhf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gaqapmklf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gxfcwlqax.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmewgovfi.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gyssypjff.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gxlxanxrw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/ghockcajp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/grxwslxev.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gtnglbhfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gdhinfuoz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gmswoyrms.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gomkxzbwp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gqmgbiwwc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gpomsyfek.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gsfmfzeii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/guxrwqlud.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gedvgrdvq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gskrtvcwk.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gksfsnpul.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gnuuluqyo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gziflxjuc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gnrboseja.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gsqjctewu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gvuchzluf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/glinwcoml.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/googmvlij.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gvddhgsdr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gpykkpstk.sHtML


<!-- 参考信息 -->