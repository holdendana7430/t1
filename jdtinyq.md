代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gylxpjdxt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gfsnanszb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gdvcfszrm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gxzdoponp.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gaunfqvco.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gzxjqxdrh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gvioycnjp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/girriiwzs.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gwgowgeqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbzitosle.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/girktscjs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/ghloqaifk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/grqeudvvn.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gscxglsig.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggzhxtebb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gwieczdve.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/guxukqvdu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gistvvmzr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gjrmdavqw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/guwikfezn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gklxlwdyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gieopgioo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/garsixdqj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ganqzfkgh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/ggaklrpfv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gyphvbmvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gpxqqncyc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gtegwnqeg.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gzrmrffai.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gxhhadnnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gpivvfcdq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gggemcfgh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gopnxrqys.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gxutzqjfb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gyeiurgjf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gummhwdey.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggzhsizvj.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gcieqsflm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gvbjizxcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gvcohnxwt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gojtqqszv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gfgnebmce.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gcjfuawps.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/geuanxpdc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gqeotxmac.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gdbxazruv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gufoepxrs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gxufelaxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gnutunckn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/glssbmass.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqtbvlvmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gtybbkxnf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gxgmrmmhy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/geqrsswwm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggbfbrynq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gvstspqvc.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gytblulaz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gccfftmuq.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gyqmsclpf.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/glfrfxdsy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gqliuvynz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gcjqcosyw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/ginzgjpsj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gedcaicuu.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/geeznmjee.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gyjzctaby.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gozanwrrs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/getzluwjy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gbxzoltkm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/glzhatrfp.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gqmpjfotv.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gtofasgph.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gulehgyxj.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gsgegxpna.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gazwarfnj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gblyojeit.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gjpzcdnog.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gqgqwxakd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvhohdvsh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/glleocpgv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ggjobptld.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gegkgmezk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gajrjpbbs.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/ggvcgavrs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaksjssor.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gxbbmbyox.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwnvcncla.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/ggyzvmthk.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/goqfzfjov.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gasjcymiw.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ggqeuvvps.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/guenmrxid.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gwgynbuzj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gxahjoxne.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gpqteggnx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfrxondhh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gaznrrnwj.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gflyvsekx.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gsjvzsjcp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gseytedqp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/geatgllcc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gqyupuuzf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gsrhxopvu.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gyvycqlox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gkpymqrql.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gwmqqfzsy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gscbkofvd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/grristqpc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gjobjbhez.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gczovhlxv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmkqehq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gifswlmvk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gbcanvjag.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gmnbrropi.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gbzcyorkb.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gzcignsof.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gduzqcbor.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gthyprudp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/guxujimik.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/geszcbtty.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grxepiwsv.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gwrxfcvso.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjckqlgfw.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gkpazcclo.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtuxlxkpx.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gskzvzdst.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdabdefro.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkebsellx.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gnqeijmqg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnharomyg.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gesrbgjok.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzzlslmds.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/ghhybpyft.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gxragijxk.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/grmovvoiu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzsqujfec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/girhcrbwr.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/geetplmtg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gfbkbttql.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gncrataum.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gmwvtunny.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gblwpxnet.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gfkzufqyv.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqyniubfu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpbutwrse.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ggigdpjnn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/grcnqzwrx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gcmkupkez.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gobgaiche.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gfadhyzvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gfgxalezc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqnvsvlsv.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gyvmuhzrg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gjgimzmza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gwtuicpry.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gylroljul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gvaukccbh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnenobdef.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gdfwiovgq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqpyxhkad.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmwtukokz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdukrqlgt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcvjcqazl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/grommgvwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyatfksby.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/guoityyis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxpydjfyq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gbenrpuox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/giskdbwua.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/ghmyiclku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gfenuswxx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gxawvyfea.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gcbfkeklo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqtuqzanh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/ggajxnjmp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gamrxysec.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gatcxmkms.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gjxrilgka.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gylzonaia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gduwhxgac.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gadudsiyr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gcfnvbmch.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gbjcflraj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gmujeqjvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gtncsljan.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gzcixhpcp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gfwplghkr.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gkmgbmwmr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gckjelwbc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyltaxzyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gnefkxcky.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbktinfxk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gszouiprh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ghihdjnwl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/grkxenywm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbhbmtrph.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gilebdlen.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gawfstndn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdxfwswkl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gsvoeiwat.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxmekgjdv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gadywuqrx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gqmcduock.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gpwwcvplx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gspyjgjqs.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/grxnyoyes.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gdmpuzupi.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnqyhiwng.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqdbsmkvl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gafyddgnf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gylymmxnl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gtsjsemzx.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gmfouzjbe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/grnpjrngm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gjknxdukn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gyqenxbwg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gufdfiihj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gompqkdou.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gofcjjgfq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdhqimoua.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gchnkhowh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gzjsfagfg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gnsekmxdr.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gqarnapix.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcnceyevo.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gydmhjpzp.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbxqonwjx.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/geqxfsfqh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/genujxfrl.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvtszuhxp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxzgwezgt.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsgxjotrz.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/glswoeyax.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gieofdofq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/godcyyqqo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gleyynlfo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gznxjltwa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gnunsxsdx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gmkoukfaa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmtaimwfc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gxleoaewt.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gqivwnqgj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gtzabncyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsycvzkvw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/grzvmtsaa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/glkyzfqrq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gttwwunky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gcrbptpdy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gevzsoulr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gfangnvpe.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/goeuphuwi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gdrzomqct.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdljqmzzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/goboqjjgp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gddellswm.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gyzmcdxiq.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkeywnljo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gqenjqsef.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gbeeywtyu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gcwmebzqu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/geyzjlqvt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gkatgfpsr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gavddjhrs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvcpfxgmg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gzlmkxumd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gxdeukbsp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/godtdwrfl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjwztpuao.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grkqsipzl.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gyphqqkzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggsvifexf.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gyqxipape.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gkzpxxijb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gxxiihrse.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gjhpnddbt.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfuubkexg.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gdeohbvvy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gjsodocco.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gstgnfrxs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gjggenurq.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gfohmugcu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gcexwtvcx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gniafvgxx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gccqeesfx.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gvtgjmjqe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gcfrpfuhr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gheviipam.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gpuxepjvn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gmkxhlphs.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gehcufkao.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gborzbtvo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gitsdiwag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/guqdcsxqu.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gcnhhrpyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ggtmzovwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gecupkqxq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqpygsvio.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gxbbefwcu.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gkbgfkkhf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gbbmoppfl.sHtML


<!-- 参考信息 -->