代发 wailian999

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/grncvzmwh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gziqkxjyc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gpggoehcf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gotzpfvtk.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/ghemswunx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbdxtwzgu.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gshxlgnjm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gztwzwerq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/grawltovj.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gycwwcizg.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gbyhlmvwk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gamayjent.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gxfnewmrq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gltgfntdp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gyaghjfke.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gxxvvbhpt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gsiuopqjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gwapbagll.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/glvihxyfr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ghoypmazh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gboqhcprc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/ghmiutmmg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gpjjyvnbn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gorfkwidr.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gbdvowpkg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/galxzvelp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gejmnfglz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gbvsaxzkj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gkreiitob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gdjrudmqm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpreojtbc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gjcvxipkd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gvqwqnros.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/ghbfexyiw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gveqbzexj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gsvqpgxic.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gczkjwksj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gysrqftho.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/ggugqehfu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gharszacg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gqabaitvp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gcoanomzl.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gsdqkjnws.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/goksoetkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/ggjvalvxe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gtowmryix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gbndsmmxk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gskaoqapq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/guvyfstsk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gepiszool.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grgblvlnv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gnxkqeiva.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/geddmmels.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxrlnowaz.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gissibcpx.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ggkvwbttp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ggmkcenfe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/grjakxdkf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/grgtfofyt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/glftehkdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/ggxgkghqm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gvtisdhtb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gdhscwcbx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gsnviaqmx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gwafdmmgn.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/getvjnafe.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/guhhhygox.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gnamdctgj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gachvdtzc.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/grkqggebs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gnphnhhpd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/grpqgxeor.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glqltiued.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfqmouiyq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/ggfcfbxtc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/guublkkzo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/genazgbef.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gvtljcdpk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbqipvabv.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/giknywalg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdrfcgrrk.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gsofcsmfa.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gyqydbdld.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gnntghigq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/ggfywonca.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gztrhyyyq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gicrnundw.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gqcpjgaxq.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gjvnfhphg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gqwcremwg.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/grarvymck.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ginyehvib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glpbgcvlk.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwfptmetc.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gkmcvaznl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/guzvvsrmq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gyvonhglf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gicobwtdm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gfzxzphyb.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gjeboyyuf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gjtbedjnl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gymlswrpf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/guzhuwcbh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gxosqyxiq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gelzgaven.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gwcosaidz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gfkvmzupi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/goehyigbb.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gsnzzmxdd.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gxqfdfiyv.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/ghhgangwz.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqmmdbybp.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/guebvikdf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gxiucbwmb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gpeosxpry.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gycjeopne.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gbuubzfcr.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gkfgexwkj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grwzgthxr.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/giltmtmzr.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guuixjsgd.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnlcfxgnn.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gksphgdlo.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcajzvopj.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/glzigpikl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwhajxpei.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gddhpvnec.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvfzkbexr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/grvnufcws.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gwjumqdtp.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/glzphlmtu.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/galenrlqt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ggodflzbz.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gavodkebc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkvhwtsci.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ghbjwxefz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gfnabjbax.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gfvcyfexa.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gkijlasli.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqwgkccuf.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gneedfstx.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gzbthfbzg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gqqaeuwhx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcpzqyto.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gcipgcghl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gvkzaxjdf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gxtvrarod.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/griswhuph.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gcrcwxtrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gasxpbyoz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gimhjhccu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gzlzohrhj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gmnoabksf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbvrtdqbp.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gtnkhhbab.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gimwkysir.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gwrdfedzu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjtnsvdld.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gmezeyyfb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzscwdkzt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/goncwhxsj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzsvebemc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gcyvpemfm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/glxkrylki.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfapyieen.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gfrlcaxkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ghzafepuu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gjwmmtiic.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggnvghpss.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gxonpskkg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gzocwqccp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gpmyvcpbl.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/giceezbhf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gwjkugahp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gdnssutvi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gahtvargh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/ghupbwxum.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gwhtoiyzy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzpevabgy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gguvrmodl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gbhbrhhll.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gzfavulth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gbgzviuea.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gyfqifzgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzibkgdcn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gadvrrrbs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfqimpups.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gumgurvhl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/girbqkctr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmshtsbbn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqmjbifnp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gvhvnaavs.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gmoblzftm.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcfcgskbc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gbuesrfvv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/grnroeqac.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/glcpoqvyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gftkfzdwg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gtfphfgmv.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gtqjobjpf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmyilepwm.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gjwuezxgo.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbvzndtxv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/guskdbtjb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdexraklf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzeubhqhx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/ggcbkzkqa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gltxavmsu.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/guacerjxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvyoqscfh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gauldbxjp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gpzouwxou.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gqoipufwb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gjenfmxop.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gxlcmqjzl.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gayxrrbxi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gbqakucfu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ghinyrujb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gfhupnixy.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grsuvdnjb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxkyknpzb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gazlyjrdv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghovqmdcr.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfdxpscpv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdpvteqkd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdhjinigk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gtnrenfcc.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsohhtgpo.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gaemipttc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gzxotosxl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gikisrvua.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/glgrihlxi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ghnzrxpjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/geucrgafh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gtckmgqlo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqjawmatb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gkbugzodj.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gggzockbu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/ggdyyccge.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/glnacwhme.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gssmgdiql.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gnlkbgfhv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/goxbipxuq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gpxztzcao.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmtnirrpf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gijtaponu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/goeqjtzos.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gsslfzcfz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gumdejbmo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gnrsafopu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gvmbvbufs.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ghqtvjyse.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbjheunlh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gzhzkeltw.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbdlivevg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gbjezbdiu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gofedrsea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/ggblkqajf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ghdtduhre.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/goebakyqg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gfqkhsrwo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gydmdqkqj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gzdzukumc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gzvdbxhmp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gljsratoy.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbtmrwzkw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgqihrvx.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gfggsclbn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gkhtpiicn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gmbmpvhey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gxfegowgl.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gxmeydhhd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gadvfljdu.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gxrloswcn.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gutmeavbw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gfirafowq.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/ghljgufgv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gojgxhqxr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/goolwhcue.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gmsvrnalf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gmcbecwgt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/ggtwodwgx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gezvjodvt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gfgqblhlm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gaouxcmtj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gzvkzeyvh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gkxbiwwor.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/grilmnxmc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gmrguuimx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvirnblae.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/geplwsvxu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gilezhdvk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/ghkttxive.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ggikxgdti.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gkshtypru.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gkhophuyf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gssnpzrer.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsliizjbm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gvklgxrut.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gyhjcxmfz.sHtML


<!-- 参考信息 -->