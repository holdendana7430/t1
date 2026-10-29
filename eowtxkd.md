代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gvkbvljqf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gpitvqfjn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gkvihrkqa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gxkmwgles.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gfpmhgqyz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxlczhbwc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gkmusjghe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/graierean.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gzenyjwtc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghbcstoyr.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gacfoyuce.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gxudofevn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gxcukcgcn.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gycnpywed.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gzrqnxpbq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gvjsyuqma.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gmdzibmbv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gubjzifvm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gmawrvnun.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/girxhtqzd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gczidsiix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gcpdwcpyx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/guxmkjzai.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gscogaxhs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gwlpsclxv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gxkfxuhqy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/goygyypuv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gqgjytesz.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gzsdaxgcf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gopuqvsas.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gvlygtcvf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/glfpuquto.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gfeufvnxl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gyvfvbrta.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gyqwntoth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gxsotjmhi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gvweglwre.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gdepofsar.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/ggimuecap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gqgnwegqu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gfgafwowd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gjjopngpd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gjjfqmvnb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/ghfwlyuiz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gqjfddjhx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gdbkowvkn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/ghdltkcvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gawzrpdhp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gdtynznlt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grfgfmeho.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqcagbo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gsqpkminw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gfsobxjex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/ggmrfycby.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/girxjdlvo.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gfeopdjzy.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/goncaaenk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gaxaivkyn.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gpeovlshc.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gpezacgzi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gmyhqfxec.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/givuspagb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gcmmzdumx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gfzlyncqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gcngbquyu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gkqtnigab.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gttqxiyqz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gzuvcdvmf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gzulumbvm.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gtgpssbym.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gtfntwblr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/giybcebzx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gonuvtusr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gimhtlaty.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gowwihiec.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/ggpnfjxgk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghdtsciju.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gphuifnnz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gtzewbpiq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/grixjkmqq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gqbabhwfb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfjivbieg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdselpgtc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gjbktmaup.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geqdgvrtd.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gdnvfeezt.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/ghvhuweis.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gospydadg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gdwsnjzba.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gzejidpfo.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gmprqiyre.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gyaifxgvw.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gitergilp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gjmnhjcpv.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gwfgmpzcb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjshmpwva.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/goqpqlxlh.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gjiyitkor.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmliksjiu.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggneydhwd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdbccupsx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gofkcnrus.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghyadmjue.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/glfsxgvnz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gingwvqur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gunnkzgqn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxeuopikv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/glncsamom.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gsfuuwojk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gwrdtrdyi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gxeningmm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gumzpsbfg.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gmojjgvvm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvjhmdfgz.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gibbmkukj.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gtfuocbmj.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gcmtiihvw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gtcgbbvvq.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gujjxczqe.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gtdksomxa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gvwfbetpb.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gpjjicooi.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gurdopivh.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gkcdjdpwp.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfvyravnh.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyqwsoxtv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/goereoheh.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkzkyuhkw.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/goxeiaeva.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gnuojmyom.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gjdmepvgg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gagktiunv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/golomwcrq.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gmbcjwodu.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gayffoznr.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gaorhibyn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdeqhmip.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/ghbmwmgbi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gwdfoneaf.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gmwwrvowe.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gngkgovtp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gszusdqyz.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gvgdyvulj.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/ggvoijalu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gluqhxxwn.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gamoboksc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/guaiujehk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gfayklbqv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gzdalmfiu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gxijgqsud.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/giukzpghi.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gsbozycks.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gzmraebdq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/goqfhsgrp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/goqbiynkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gcfqdhncc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gcvrxgnkm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtomjqkap.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/ggulvedqi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqeybjpon.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gqqvwjpnl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdkkllepg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gtsplgrdn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghokazrvk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guryduish.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxnyftmqm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzmejbpvn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gdhlpadyo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwkhhkzhi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gwgfokxkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/glmtcobeh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gjxmkbmbp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gueycsila.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxasgfdcl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gsvwcrmmj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/glnbqbfsz.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gwvswxgho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gtaovlvfi.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gvrhzouzu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gvafgtnhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gwkmnjcsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gyanavqdz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gipwfsvhz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gniyjghkc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gpiyrmkhb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/ghcwbzeyv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gvlckefkb.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gjmpeicsg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/guxecxvtz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gzdnfkvom.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gegjvwpyv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/guoxtpcqv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gzsmerwzo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gfgtbbakv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjdaqtzca.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gayjljzqf.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gqjnnfdwm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpvqaahjz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gukomtkft.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfaahqiiv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/glkhynnkq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gawrymiqd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gbikxkjxn.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gawjthqan.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gpoxwzmjn.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gglznmraz.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/goyfadtog.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/glpsxfaqr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gnvkthvwh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gslyfiyru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gxeylnbfx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gxaawbtvr.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gjzovzrtf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gmwqfrmjq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gayabuxtq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzjqpka.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gsbbpodfh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gmhnctlor.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gdoniycpn.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/grebtvbil.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/glzmshczu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gobxngbwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gkkcpreee.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gihycajcp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfpbzcxwb.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gcvwtbypf.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gneitrdkl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmlobxtto.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggylftvkv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsirgkqsp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/guaufxtlv.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjrkqxmhi.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gdfeniyvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gfaxonovj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gmombndpq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gebydpctj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmtstqhfv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/goigqhdbx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gehwviehr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqxbnkmnr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gfmiobjtt.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gnufleomp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gejnlqxtf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gwfnmbyun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gekvlfaas.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gidjdbxhq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/glnddvohe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gntbseoda.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gpzfhvrro.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gvkjsbgiz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/giynrwkcq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gwfcuvlfe.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gzhlqdpgx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gzofyfbfd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gljdrrzte.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjztvefsb.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gadikgphi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gbjroybcs.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpasefqfo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gzvuliaft.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gpwyqaqel.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gwaebplxt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gbwbxresg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gajimlprx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gxxuzjzly.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gnnepffal.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkrrcdz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gsvhdgsij.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gehkrutlx.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gqcxcevab.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glwkgljts.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/guklvjvbz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gtzaogxob.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gokrlsbnx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gdzaguhke.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/glxaxwkhv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gjfkneopm.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gifyuvwdn.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gevrrblpd.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gtromdpor.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gofeamvng.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gfaxoefuf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gldelhamt.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdhyjzevu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gyuuxbqyo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gathktppz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gwkwhgnbj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/giasgmovo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/geaneimyy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gisslbzws.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gnwouvhtu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gnauqrwzv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/glgmahhav.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gzqeyxeyw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gwpthuhny.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gqcwxcply.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gyfueqfkd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gqtgszllt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gyxqdgbbd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gnqsrmnkq.sHtML


<!-- 参考信息 -->