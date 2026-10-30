代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gmlkufcnp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gtjihodzj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gyurvlrtz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/grwhilzye.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gwgaeinrh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gctiltajo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gtidrmwoe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpgrezgvh.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gvnbsofmc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghpolgcbu.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gmfgukuav.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/ghbypqtuf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gcumhiswv.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gxxpbmqte.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gumnwqaue.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gjveyzvxa.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/ggcdfdbeu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gubdbevpe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gsqteuojp.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gftqldifc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gbwgzeqnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gzuuwtlaw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gutqvxktf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gwugdmwvm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gmjdmqmek.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gcidvlryb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/getnpfyru.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gkxzoqqhf.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/giivrdizz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gpukfzoyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfoiythag.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gvealnnfm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gjcpkmdwo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gxudogyik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/guutbdgzn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gjtzuwdsa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gwuaofiyf.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/goesbtwuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gqdnwpasi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gkeaqhgcy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gswnjmptg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gcsngbcwx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/glvhjaxgu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gvzuuvhzb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gnypehjvy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gritvexcu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gkxtkkixi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/goizicyfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gvlipecyy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gxuswghuy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gzjdgbhgn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gkuywwjha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gwadorgmb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gcciwycvp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gckrrvvvo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gqflugzuw.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gcpsqwozi.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/ggbtekvlh.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gldzsugqk.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzicaftbr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/guewagang.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gvlxdbapd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gsrhvzarc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gedxkkydf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gilrqzbih.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gwjncrhkh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gaflpeghk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gnigvokzu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gysdndrjg.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gldvozfns.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gdcduqtpi.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gczmixrvo.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghzykrbav.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gfgyjzwil.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gmlputlzj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gcunfbway.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gfhamhtum.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/guqsgdibn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gtkxfqgrv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gwsiqhexu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjjdgxezy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdtsyeglh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpspqfdv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gclboxpfe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbzszgxpp.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gejlmlazb.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/glgxmnwad.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gxovlrymc.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gwdoqjnuv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/ghscqdzcy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gxmiidlcb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gwiwjknrv.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gsinmyabo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/geydheesf.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gcsqtkpzw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqfjzdhdt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdgwiwr.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghjgtgpoc.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gohdxqhbd.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gslftyrcq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghmqjlfic.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ggzhshinu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqekywoes.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gbybjrpef.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gccvgxfis.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gdwfbkgsn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gmwnuetms.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gygrzqgwy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gotwojsxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ghzlsbscv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/giksldizg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gyufdkyas.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gnyewnukj.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gthyhbfri.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gyhudsrbr.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvsrtxqam.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gjtazqwec.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/glxpgwfzh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gebomwfjb.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gvxqofmwu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/giahcbkzs.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ggguqxoho.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goaybdryx.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gqfkvgvul.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/girmeqcbw.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ganyfoegp.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjcfhqvnj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjadwiac.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gxnbamajo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/giayimkqu.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gxpjxgocn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gffynjrqv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ghoybufca.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdtnerwet.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gbntbbxrx.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gjohgphxx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/guycdhiwp.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gbclchqqj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gezqpeyne.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gnvttsdaa.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gxvvreowy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gzpkzkfsr.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ggjrnbakt.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjtwlijws.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gkxnhvsjz.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gaqxwgwww.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gpqlomtml.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/godxqqxef.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gpmmjceef.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gbdwbtdxa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghedzccqq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/getsfbpcl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gssyoqzvd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gprdrrtmo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gvofknfjx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gbguzvlzf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gwqrjzafd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqhcctooo.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/ghoopkrtr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjjtgudta.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gxwtclhem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjzbhnowe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/goyzaawip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdtvlla.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gmqwioriy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbzqphako.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gidbvgwpp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gpkmfofdb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbsywharz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gdtbmiekz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/guwiqzzbc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gokekovdj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gulbjftwq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gvkhpyxwl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gpuecvdlr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gchokdwda.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gxtyakzib.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gkkylaztx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gvknfujxa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gaunqwhoa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gxpcxqzbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gftlqujer.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gguqwhckb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmmgwemif.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gsjpqbtmd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/geycaghsr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/ghhsgstde.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gxtnwudyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gkresrpti.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/goqxillqx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gecvdlstd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gyglgnegh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gecsjqmyd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gqpfoxrmt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ghweqjawq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gayfcakdm.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gjipgxeoj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gflqgimmw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gweiebcug.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdvvwvzbk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbadtzfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gftiikyvl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gbzlobqds.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gylsetxjs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gdumlkynz.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gmofmbeeo.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gvoldrsia.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gfaacueed.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gujhulxrr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grzlgyjrm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gxyfrqzva.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/ghfvbydmn.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzadxbjsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gkifyezgl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gjjrofwxd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gmkwlsprt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gkxyetegr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gppjsradh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gwmbuneqi.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/grjuwzfut.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gfpieujmz.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gtirbnkou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gyftmfplr.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gjgvnpima.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gwjwlznsr.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/ghfgypnsc.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxasrahfh.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gluzsjjdh.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdtsrebyz.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gurrmmjtg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxedwvker.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnrygfwxr.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gccyvgnky.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gdtbqnwks.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghzaictxq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqqxdgjdx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gijwbzhdj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gohxwsznv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gchwhhuqm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gzrzpiocv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/geroioius.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gbyxzvvvr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/ggxgsapnk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqpgqkeg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gseeglwbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gygkkprhp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gpzggfbkj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gafrsdnnb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gtlkocjcm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/glefvirni.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjhjfoo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gaahlehlw.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gltvxvsat.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gyvrkkfwb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwmxesxii.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gfegkvbqn.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gckhmywen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/geudkuxcc.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqytomdmf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gunepoqxj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gzcfgcxym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/ghxvtbfuq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghckzxude.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/goirwpswg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkfvbueac.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gmyltgyxf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gsouhueia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gqhykjvaw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goydibydg.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gnwpbtlsz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnkwosufr.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ghjimunan.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gcofokqwe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gdgmlpkfv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gxrumnonw.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gmjfvpmqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gcedubuxg.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gvpccpijw.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gdtiajofl.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gmudiizlf.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbcnmmecj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gsrbxwnfj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gakpxqfqa.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gqvwcewik.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkitcrrxd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gckpduryd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gdlclyucx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/ggmkhqhbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/graezwbfh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/grweiqlfm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gjvgxhiho.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gamqhuyrb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gfuynpdwi.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gandemnrh.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gxztexzsi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gwqjludte.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/glwiviwan.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gudvwmlmw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gfxtpxiec.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gbhlmahwg.sHtML


<!-- 参考信息 -->